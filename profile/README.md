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
    <img src="https://raw.githubusercontent.com/PrysmianGroup/.github/main/logo-prysmian-black.png" alt="Prysmian Group Logo">
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
          <li><a href="#limitations">Limitations</a></li>
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

| :exclamation:  To keep our GitHub organization structured, please respect the following rules   |
|-------------------------------------------------------------------------------------------------|

#### Limitations

Repositories created in the PrysmainGroup organization are for projects
directly related to fiber business. Projects outside this scope, including global initiatives, should
be stored elsewhere.

#### Naming Convention

 ```
 PlantCode_Technology_[TechSub]_[ArchiveYYYY]
 
 [] = Optional
 ```
  <table border="1" cellpadding="0" cellspacing="0">
  <thead>
    <tr>
      <th colspan="7">Examples</th>
    </tr>
  <tr>
    <td>PlantCode</td><td>_</td><td>Technology</td><td>_</td><td>[TechSub]</td><td>_</td><td>[ArchiveYYYY]</td>
  </tr>
  <tr>
    <td colspan="7">&nbsp;</td>
  </tr>
  <tr>
    <td>
 BRA = Brazil<br />
 CLA = Claremont<br />
 EIN = Eindhoven<br />
 ROM = Romania<br />
 SLA = Slatina<br />
 SOR = Sorocaba
    </td>
    <td>
    </td>
    <td>
      Wareflow<br />
      FTIR<br />
      LUTS
    </td>
    <td>
    </td>
    <td>
      Machine Type<br />
      Manufacturer<br />
      Inteface Software<br />
      OS Version<br />
    </td>
    <td>
    </td>
    <td>
      Archive2018<br />
      Archive2019<br />
      Archive2020
    </td>
      
  </tr>
</table>
 
 
Below is an Example of similar repos that vary by location, only using the required conventions:

```
CLA_Wareflow
SLA_Wareflow
SOR_Wareflow
```

Example of an old Claremont Wareflow repo that is no longer receiving updates
and should be archived.

 ```
 CLA_Wareflow_Archive2019
 ```

 Example of related repos within the same plant supporting the same technology.
 
 ```
 CLA_DrawTowerPLC_TypeA
 CLA_DrawTowerPLC_TypeB
 CLA_DrawTowerPLC_TypeC
 CLA_DrawTowerPLC_TypeD
 CLA_DrawTowerPLC_TypeE
 CLA_DrawTowerPLC_TypeF
 ```
<p align="right">(<a href="#top">back to top</a>)</p>
  
#### Description

Every project should have at least a one line description of the project to explain
the reason for the project's existance.

#### Topics

Adding topics to a repository is encouraged but not required. Topics allows our team to quickly search for related repositories. A single repository can be associated with many different topics.

<a href="https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics" target="_blank">Topics Documentation</a><br />

Example: To find all repositories that are tagged with both the "bench" and "measurements" topics you would simply search for:
 
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

2. Create a new folder to contain the repo, in it's new location.
  
3. Make sure you're in the parent folder of the folder that was created in step 2 before proceeding.
```
git clone --mirror <url of repo to be migrated> <new-local-folder-for-new-repo>
```
4. Navigate to the new-local-folder-for-new-repo
```
cd <new-local-folder-for-new-repo>
```
5. Remove the original origin remote
```
git remote rm origin
```
6. Add the new origin remote
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
