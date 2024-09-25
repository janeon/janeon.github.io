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

As lab helpers with multiple semesters of experience, my teammate and I would repetitively answer the same questions for different students over the course of a single lab session, not to mention across different weeks or semester. In efforts to reduce such redundancy and to provide better self help tooling to students in Oberlin's introductory computer science course (CSCI 150), this project provides immediate feedback and suggestions to a given a Python file. The suggestions can be customized to display in an order that the student chooses, and the tool also recommends related sites based on the various types of errors found within the file.

Compatible OS: Mac and Ubuntu
- Check it out from our [Github repo](https://github.com/janeon/automatedLabHelper)

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
