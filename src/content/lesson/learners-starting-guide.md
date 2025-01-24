---
description: >-
  Learn how to start coding with LearnPack! Discover interactive tutorials,
  setup guides, and troubleshooting tips to enhance your coding journey.
---
# How to Learn Coding with LearnPack

Getting started with Learnpack is straightforward. LearnPack is a tool that operates inside your coding environment (e.g. VSCode), enabling any repository codebase to become an interactive tutorial. Any repository compatible with Learnpack can serve as an excellent tutorial. You can check out some examples of LearnPack-compatible repositories [here](https://4geeks.com/interactive-exercises).

## Getting Started

1. **The 4Geeks.com Learning Library is the best place to find LearnPack tutorials**
   - Navigate to `Learning Library/Practice Interactively`.
   - Click on `Start Practicing`.
   ![Learning Library Navigation](https://github.com/breatheco-de/content/assets/107764250/a2b43a37-f294-4e99-aa68-d57a2479ccd9)

2. **Select a Tutorial:**
   - Pick a tutorial that interests you.
   - Click `Start exercise`.
   ![Start Exercise](https://github.com/breatheco-de/content/assets/107764250/b42f6559-dad4-4dca-9a6f-0e48b0e889e7)

3. **Open with LearnPack:**
   - If you are logged in, click the `Open with LearnPack` button.
   - If you don't want to log in, you can navigate to the GitHub repository by clicking on the repository link and referring to the section *Opening Directly on Github* below.
   ![Open repository button](https://github.com/breatheco-de/content/assets/107764250/6feb769f-a819-4d37-be2d-b9466e9fd60a)

4. **Choose Environment:**
   - Select `Codespaces` (recommended) or `Gitpod`. For this guide we are going to be choosing `Codespaces`.
   ![Choose Environment](https://github.com/breatheco-de/content/assets/107764250/6d9f5213-321d-41a3-bfcf-6f8c328fd09c)

5. **Create a Codespace:**
   - Click `Create codespace`.
   ![Create Codespace](https://github.com/breatheco-de/content/assets/107764250/788c0dad-2e56-49c4-ad64-c37d3101d756)

6. **Run LearnPack:**
   - LearnPack should now be running in your codespace (you can read more about [what is a Github Codespace here](https://4geeks.com/lesson/what-is-github-codespaces))
   ![Learnpack Running](https://github.com/breatheco-de/content/assets/107764250/2c3509d4-585d-469f-9cbe-22bbebaab543)

## Opening Directly on GitHub

*You can also open Learnpack tutorials directly from GitHub repositories compatible with Learnpack.*
These are some examples of LearnPack-compatible Github repositories you can open: 
[Javascript Arrays](https://github.com/4GeeksAcademy/javascript-arrays-exercises-tutorial)
[Javascript Beginners tutorial](https://github.com/4GeeksAcademy/javascript-beginner-exercises-tutorial)
[Python Beginner exercises](https://github.com/4GeeksAcademy/python-beginner-programming-exercises)

To open a new Learnpack environment, find the tutorial you want to take and go to its repository. I suppose you are already here; if not, refer to the previous section.

1. Click the `Code` button.

![Click the code button](https://github.com/breatheco-de/content/assets/107764250/413b2553-d452-4cb4-bb79-b2595e8e35be)

2. And `Create a codespace` on the main or master branch, depending on the case.

![Create a codespace](https://github.com/breatheco-de/content/assets/107764250/8c1da50c-81ed-4162-9359-d41f35aab8ab)

**Now you should have Learnpack set up and running in your Codespace!** 

## Local Setup

*To run Learnpack locally, ensure you have Node.js installed and the technology stack required for your chosen tutorial (e.g., Python for Python tutorials).*

1. First, you will need to install the correct dependencies in your system, depending on the setup.
For instance, I'll make an example of how to run Learnpack locally using Python and Node.
This is the example repo: [Python Beginner exercises](https://github.com/4GeeksAcademy/python-beginner-programming-exercises)

Use the following command from the `.devcontainers/devcontainer.json`. Just copy the `onCreate` command and run it in your computer.
In this case:
```
pip3 install pytest==6.2.5 pytest-testdox mock && npm i @learnpack/learnpack@2.1.30 -g && learnpack plugins:install @learnpack/python@1.0.0
```
Most Python exercises use a similar configuration, so ensure you have the dependencies installed.


2. Clone the repository in your local computer:
![example Learnpack repo](https://github.com/breatheco-de/content/assets/107764250/a87a1bdf-a50f-46ad-bdff-149e737f60bd)
```bash
git clone <repository-https-url>
```
![example of git clone](https://github.com/breatheco-de/content/assets/107764250/6545b2cf-97dc-4560-af20-8cefa90d8c62)

3. Navigate to the newly created directory:
```
cd directory-name
```
![Example of cd](https://github.com/breatheco-de/content/assets/107764250/3c059800-04c3-48b9-81a7-fe5684836eb8)

4. Open the directory in VSCode. You can either drag and drop the directory in VSCode or run:
```
code .
```
in your terminal when located in the right directory.

5. Run `learnpack start`
Now Learnpack should be running on your machine.
![learnpack in localhost](https://github.com/breatheco-de/content/assets/107764250/17316b6c-12fa-4cf8-ba5a-eab38de2afcc)

# Troubleshooting Learnpack Issues

### Learnpack Not Running
**Scenario A: Missing Instructions or CLI**
   1. Open a terminal.
   2. Type `learnpack start`.
   3. Press `enter`.

**Scenario B: CLI Running, No Instructions**
   1. Press `Ctrl` + `K`, then `W` to close all tabs.
   2. Run `learnpack start` again.
   3. If still no instructions:
      - Press `Ctrl` + `Shift` + `P`.
      - Select `Learnpack: Open instructions`.

**Scenario C: Error on `learnpack start`**
   1. Verify Learnpack installation:
      ```bash
      npm ls -g @learnpack/learnpack
      ```

*If issues persist, reach out to your instructor or the Slack community for assistance.*
---



