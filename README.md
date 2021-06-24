# Koslicki lab page documentation v1.00



<h2><font color="red">To be discussed </font></h2> 

- [ ] Add your introduction with an image (check below for the method)
- [ ] improve the outlook 


<h2><font color="blue">Documentation </font></h2> 

Contents:

1. [Basic](#basic)
2. [Operations](#operation)
   1. [update your personal file](#personal)
   2. [add a publication](#pub)
   3. [local preview of the lab page](#local)
   4. [navigation of editable files](#edit)
3. [Structure of the page](#structure)
4. [Some cool tricks](#trick)
   1. [github action: workflow](#workflow)
5. [Acknowledgement](#thanks)



### Basic <a name="basic"> </a>

Our [lab page](https://koslickilab.github.io/Koslicki-lab-PSU/) was built from [Github Page](https://docs.github.com/en/pages) with [Jekyll](https://jekyllrb.com/). Github Page grants you the feasibility to create and host a website directly from a Github repository while Jekyll is a "translator" to transform your plain text into static website. Based on these, we took advantage of a [lab-website template](https://github.com/greenelab/lab-website-template) developed by the Greene lab as well as the [Mangul lab page](https://github.com/Mangul-Lab-USC/Mangul-Lab-USC.github.io) that was originated from the template to customize our own lab pages.  <br>

The [source code of our lab page](https://github.com/KoslickiLab/Koslicki-lab-PSU) is hosted in the lab's Github account. Everyone in the organization can access and edit the contents in the repository to reshape the webpage. Please feel free to play with it : )



### Operations  <a  name="operation"></a>

Stepwise guide for "how to update the website"

###### 1. Update your personal file <a  name="personal"></a>

It's recommended to maintain a local copy of the repo so the steps below are much easier to do.

- go to the local [repo folder](https://github.com/KoslickiLab/Koslicki-lab-PSU)
- add your image (e.g. peter.png) to [images/team ](https://github.com/KoslickiLab/Koslicki-lab-PSU/tree/master/images/team) folder (all format works, jpeg, jpg, png, pdf, etc.)
- go to [_members](https://github.com/KoslickiLab/Koslicki-lab-PSU/tree/master/_members) folde, a simple way is to copy a current file as a template, for example you can do

```
cp shaopeng-liu.md  peter.md
```

- then open [peter.md](https://github.com/KoslickiLab/Koslicki-lab-PSU/blob/master/_members/shaopeng-liu.md) and change the information inside to yours
- finally, you can commit your edits and push to the repo



###### 2. add a publication<a  name="pub"></a>

It's recommended to maintain a local copy of the repo so the steps below are much easier to do.

- go to the local [repo folder](https://github.com/KoslickiLab/Koslicki-lab-PSU)
- open [_data/research-input.yml](https://github.com/KoslickiLab/Koslicki-lab-PSU/blob/master/_data/research-input.yml) file (this is the YAML file input for the autocite robot)
- follow the YAML format (key:value pair) to add your paper:
  - id: recommend DOI
  - image: an illustrative figure (whether local or from the web)
  - tag: arbitrary key words
  - repo: optional, this is where the bot obtain key words
  - description: a few sentences to be shown for the paper
  - extra-links: this is where you put various links such as github



###### 3. local preview <a  name="local"></a>

This is a guideline for those who wants to reshape the website at structure-level. I'd recommend try local viewing **if you want to build your personal website too**.

Skills you'll need:

- Carefully go through the [Github Page documentation](https://docs.github.com/en/pages) 
- Carefully go through the [Jekyll documentation](https://jekyllrb.com/)
- Get familiar with YAML syntax
- Get familiar with HTML and CSS syntax

Follow the steps below:

1. Clone the repo to your local machine
2. Install Ruby and Jekyll, check [here](https://jekyllrb.com/docs/installation/) for guidance
3. Go to the repo folder, run the following code:

```
bundle exec jekyll serve
```

4. Then you can view the website at `http://127.0.0.1:4000/`
   - Every change in files will immediately apply to your local view (unless you change the _config file)
   - Very handy way when you are building/editing the webpage




###### 4. navigation of editble files <a  name="edit"></a>

This is a guideline for the files that are corresponding to each specific part of the website.

| Section            | file                      | note                                             |
| ------------------ | ------------------------- | ------------------------------------------------ |
| Header row         | _includes/header.html     |                                                  |
| Research Page       | _data/research.yml        |                                                  |
| Publications Page  | _data/research-input.yml  | "research-output.yml" is automatically generated |
| Software Page      | _data/resources.yml       |                                                  |
| Team Page          | _members/                 | add markdown file inside the folder              |
| Media Page         | _data/resources.yml       |                                                  |
| Opportunities Page | oppurtunities/index.md    | no extra source file                             |
| Icon setting       | _includes/paper-link.html |                                                  |






### Structure of the page <a  name="structure"></a>

- Research: description of ongoing researches
- Publication: list of papers
- Software: list of developed softwares, useful links, other lab-related resources
- Team: members
- Media: teaching, outreach, news
- Opportunity: openings and fundings







### Useful tricks <a  name="trick"></a>

Some fancy functions that I found very helpful.



###### Github action: workflow <a  name="workflow"></a>

This is how the autocite works:

1. "manubot" is a Python API to pull publication information based on IDs (e.g. DOI) provided in our "research-input.yml" file
2. The [build-research.py](https://github.com/KoslickiLab/Koslicki-lab-PSU/blob/master/_data/build-research.py) file is a <u>Python wrapper</u> to call "manubot" to generate a YAML file that fits our lab pages
3. [Here is the trick](https://github.com/KoslickiLab/Koslicki-lab-PSU/blob/master/.github/workflows/auto-cite.yaml): everytime the "research-input.yml" (in master branch) is edited remotely, the Github workflow will be triggered to call the Python wrapper in step2 to update the YAML file. So we only need to maintain the "research-input.yml" file.
4. Google for more details







### Acknowledgement <a  name="thanks"></a>

1. This Github Page was generated from [`lab-website-template`](https://github.com/greenelab/lab-website-template) by the Greenelab.
2. Some improvements for the template above were cloned from [`the Mangul Lab`](https://github.com/Mangul-Lab-USC/Mangul-Lab-USC.github.io).

