<script lang="ts">
    import { onMount } from 'svelte';
    import { createEventDispatcher } from 'svelte';
  
    export let inputText = 'Default text'; // Default text if none provided
    const delay = 50; // Delay between each update (in milliseconds)
  
    let scrambledText = '';
    let isUnscrambled = false; // Track if the text has been unscrambled
    const dispatch = createEventDispatcher();
  
    // Function to scramble text by shuffling characters
    function scrambleText(text: string) {
      const shuffled = text
        .split('')
        .sort(() => 0.5 - Math.random())
        .join('');
      return shuffled;
    }
  
    // Function to unscramble and reveal text
    function unscrambleText() {
      let counter = 0;
      scrambledText = scrambleText(inputText); // Scramble initially
  
      const scrambleInterval = setInterval(() => {
        scrambledText = inputText
          .split('')
          .map((char, index) => {
            if (index <= counter) {
              return inputText[index]; // Reveal the correct character
            }
            return scrambledText[index]; // Keep scrambled characters
          })
          .join('');
  
        if (counter >= inputText.length - 1) {
          clearInterval(scrambleInterval); // Stop when full text is revealed
          isUnscrambled = true; // Set flag to true after unscrambling
        }
  
        counter++;
      }, delay); // Adjust the delay as needed
    }
  
    onMount(() => {
      scrambledText = scrambleText(inputText); // Scramble text on mount
    });
  </script>
  <div class="pt-2 whitespace-nowrap mt-2 flex justify-center"> <!-- Centering the entire block -->
    <div class="flex flex-col items-center"> <!-- Stacking text and button -->
      <div class="flex items-center">
        <span class="font-bold font-arial">Email:</span>
        <span class="font-mono text-lg ml-1">{scrambledText}</span>
      </div>
      <div class="flex justify-center mt-2"> <!-- Centering the button -->
        {#if !isUnscrambled}
          <button
            on:click={unscrambleText}
            class="px-4 text-yellow-500 font-arial rounded"
          >
            Unscramble
          </button>
        {/if}
      </div>
    </div>
  </div>
  