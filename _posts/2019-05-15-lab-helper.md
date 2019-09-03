---
title: Automated lab helper
layout: post
author: Jane Hsieh
categories:
  - projects
  - linting
summary: Code analysis and suggestions with PyLint and Beautiful Soup
thumbnail: posts/lab_helper.png
---

This project uses the Pylint package to scan source code for finding code that would potentially cause errors, warnings, and breaches of convention.

Intended to help students in Oberlin's introductory computer science course (CSCI 150), this tool provides immediate feedback given a Python file (in an order that the student chooses to display in) and recommends related websites based on error type.

Compatible OS: Mac and Ubuntu
- [Github repo](https://github.com/janeon/automatedLabHelper)

<img src="/assets/img/posts/recommendation.png" style="width:100%; display: inline; float: left;">

<table cellspacing="0" cellpadding="0" border="0">
    <tr>
        <td style="text-align: center;">
            <img src="/assets/img/posts/prevalence.png" style="width:100%; display: inline; float: left;">
            <br />
        </td>
        <td style="text-align: center;">
            To the left are distributions of errors when running on samples of 150 student sample code
            <br />
        </td>
    </tr>
</table>
