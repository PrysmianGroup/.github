<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
<a href="https://www.linkedin.com/company/prysmian/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555" /></a>



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="#">
    <img src="https://raw.githubusercontent.com/PrysmianGroup/.github/main/README/.github/logo-prysmian-black.png" alt="Prysmian Group Logo">
  </a>

  <h3 align="center">Prysmian Group Fiber</h3>

  <p align="center">
    Supporting Prysmian Group's fiber business software and technologies.
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#creating-repositories">Creating New Repositories</a>
      <ol>
          <li><a href="#scope">Scope</a></li>
          <li><a href="#naming-convention">Naming Convention</a></li>
          <li><a href="#description">Description</a></li>
          <li><a href="#topics">Topics</a></li>
      </ol>
    </li>
    <li><a href="#migrate-existing-repositories">Migrate Existing Repositories</a>
    </li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#links">Links</a></li>
  </ol>
</details>

## Creating Repositories

| :exclamation:  To keep our GitHub organization structured, please respect the following guidelines   |
|------------------------------------------------------------------------------------------------------|

#### Scope

Repositories created in the PrysmainGroup organization are for projects
directly related to fiber business. Projects outside this scope, including global initiatives, should
be stored elsewhere.

#### Naming Convention

A repository name should only use lower case characters. This speeds up the work flow for those using the Git CLI.
Use an underscore "_" as a seperator between the sections as defined below:

```
 plantcode_technology_[techsub]_[archiveYYYY]
 
 [] = Optional
 ```
  <table border="1" cellpadding="0" cellspacing="0">
  <thead>
    <tr>
      <th colspan="7">Examples</th>
    </tr>
  <tr>
    <td>plantcode</td><td>_</td><td>technology</td><td>_</td><td>[techsub]</td><td>_</td><td>[archiveYYYY]</td>
  </tr>
  <tr>
    <td colspan="7">&nbsp;</td>
  </tr>
  <tr>
    <td>
 bat = Battipaglia<br />
 cla = Claremont<br />
 dou = Douvrin<br />
 ein = Eindhoven<br />
 sla = Slatina<br />
 sor = Sorocaba<br />
    </td>
    <td>
    </td>
    <td>
      wareflow<br />
      ftir<br />
      luts
    </td>
    <td>
    </td>
    <td>
      machine type<br />
      manufacturer<br />
      inteface software<br />
      os version<br />
    </td>
    <td>
    </td>
    <td>
      archive2018<br />
      archive2019<br />
      archive2020
    </td>
      
  </tr>
</table>
 
 
Below is an Example of similar repos that vary by location, only using the required conventions:

```
cla_wareflow
sla_wareflow
sor_wareflow
```

Example of an old Claremont Wareflow repo that is no longer receiving updates
and should be archived.

 ```
 cla_wareflow_archive2019
 ```

 Example of related repos within the same plant supporting the same technology.
 
 ```
 cla_drawtowerplc_typea
 cla_drawtowerplc_typeb
 cla_drawtowerplc_typec
 cla_drawtowerplc_typed
 cla_drawtowerplc_typee
 cla_drawtowerplc_typef
 ```
<p align="right">(<a href="#top">back to top</a>)</p>
  
#### Description

Every project should have at least a one line description to provide context.

#### Topics

Adding topics to a repository is encouraged but not required. Topics allows our team to quickly search for related repositories. A single repository can be associated with many topics.

<a href="https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics" target="_blank">Topics Documentation</a><br />

Example: To find all repositories that are tagged with both the "bench" and "measurements" topics you would search for:
 
```
org:PrysmianGroup topic:bench topic:measurements
```

#### Projects
* Any technology that exists in more than one location shall be related by the
 creation of a shared Project.
* Read permissions should be granted to all teams for all repos within a related
technology project.

## Migrate Existing Repositories
Below is a cheat sheet for migrating repos into the PrymaianGroup organization. If you'd like a more detailed explanation, please click <a href="https://www.atlassian.com/git/tutorials/git-move-repository">here</a>.
1. Create a new empty repo in the PrysmianGroup organization, see <a href="#naming-convention">guidelines</a> above.

2. Create a new local folder that will contain the new repo.
  
3. Clone the repo to be migrated into the new folder with the command below. (The --mirror flag will make an
  exact copy, including all branches and tags. Make sure you're in the parent of the folder that was created in step 2 before proceeding).
```
git clone --mirror <url of repo to be migrated> <new-local-folder>
```
4. Navigate into your cloned repo.

5. Remove the original origin remote
```
git remote rm origin
```
6. Add the new origin remote using th URL of the repo created in step #1. 
```
git remote add origin <url to NEW repo>
```
7. Push the repository (including all branches and tags) to the new repo.
```
git push origin --all
git push --tags
```
  
<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Organization Admin - Biagio Calo - Biagio.Calo.ex@prysmiangroup.com<br />
README creator - William Willett - William.Willett@prysmiangroup.com

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LINKS -->
## Links

* [Git Installation](https://github.com/git-guides/install-git)
* [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
* [Team Branching Strategies](https://www.gitkraken.com/learn/git/best-practices/git-branch-strategy)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Markdown Guide (README files)](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
* [Img Shields](https://shields.io)
* [GitKraken GUI Client](https://www.gitkraken.com/)


<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/company/prysmian/
[product-screenshot]: images/screenshot.png
