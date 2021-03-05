
Hi there! This guide aims to teach people unfamiliar with Github how to suggest edits to the [Tanzu Agile Practices site](https://tanzu.vmware.com/developer/practices/). Follow the steps below to get started!


# Workflow overview

It takes many clicks to suggest an edit, but these are the 5 big steps you have to do.

1. **Prepare**: Type up your suggested edits 
2. **Fork**: Forking just means creating a copy of the practices site code for your GitHub account
3. **Edit**: Copy and paste suggested edits into the code in your copy of the practices site through the GitHub UI and save it in a branch
4. **Pull Request**: Pull Request is the technical term for submitting the suggested edits to be reviewed, approved by someone else and updated on the site
5. **Delete**: When the change is approved, delete your copy of the practices site.

Repeat steps when you want to suggest new edits to the site.

# Step by Step Instructions 

## 1. Prepare
1. Type up the changes you want to make for the Practices site. Any word editor will do for this, Microsoft Word, Google Docs, Notes on Mac.
2. Create a Github account, if you don’t have one. Login to your Github account, if you do.
3. If you’re doing this for the first time, set aside up to 30 minutes to go through these steps.

## 2. Fork (Create a copy of Practices site)
1. Go to the [VMware practices repository on Github](https://github.com/vmware-tanzu/tanzu-dev-portal/tree/main/content/practices) - this is where all the code for the site sits. It is also open to the public for contribution. 
2.  Click on fork

<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Click%20on%20Fork.png" />

3. Fork it to your own Github account
<img style="float: left;" width="300"  src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Fork%20to%20your%20own%20Github%20account.png" />

4. Click on Content

<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Click%20on%20Content.png"  />

5. Click on Practices. You’ll see a list of all the practices currently on the site.
<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Click%20on%20Practices.png" />

6. Click on the practice you want to add to. For this example, I clicked on design-studio.
<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Click%20on%20the%20practice%20you%20want%20to%20edit.png"  />

7. Click on index.md. You can now see what the page looks like in plain text
8. Click on the pencil edit icon. You can now see what the page looks like in markdown language. Don’t worry, markdown is a simplified HTML/CSS script. 
<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Click%20on%20Edit%20icon.png" />

## 3. Edit (Make Edits and save as branch)

1. Paste your edits into the right section. Just note that if you’re adding a ‘header’, ‘callout’ or any form of special formatted text, take a look to see how headers have been written, so you can copy the syntax. 

<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Edit%201.png" />

For example, I added a tip here. A tip is written like this:
 {{%callout%}}
My tip
 {{/%callout%}}

Try to also keep to the indentation format so that the text looks neat and readable.

Unfortunately, at this point in time, it is not possible to preview what it will look like on the actual website, but you can click on the Preview Changes tab to see if the edits show up in the right places. 

2. Scroll down to the Commit Changes section, and fill in the title. It defaults to ‘Update index.md’, but give it a short summary of **what you did** in less that 50 words
3. Fill up the extended description with the reason **why** the update was needed, or the context around the update.
4. Select ‘Create a new branch for this commit’
5. Create a name for the new branch that explains **what it is** 
6. Click Propose Changes. 

<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Edit%202-6.png" />


8. Do NOT click the ‘Create Pull Request’ button that appears in the next screen. Click instead on the Pull Requests tab. 

<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Edit%207.png" />

## 4. Pull Request (Submit edits for review)

1. Click ‘New Pull Request’. 
<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/PR%201.png" />

2. Make sure that your base repository is vmware-tanzu/tanzu-dev-po..., and the head repository is your account.
3. Change the dropdown for your “compare: main” to the name of the branch you have created. 
<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/PR2-3.png" />

4. Scroll down to check that text highlighted in green is the change you want to make. 
5. Click Create Pull Request
<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/PR5.png" />

6. Click Create Pull Request again. This will send the edits through some automated checks. 
<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/PR6.png" />
<img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/PR%207%20-%20checks.png" />

7. At this stage, you’re done! 
8. If you want to, you can keep the screen running until all the tests have passed, and click on the netlify row to preview how it will look on the site.
9. Otherwise, feel free to close GitHub and continue with your life. The checks will continue running even if you leave the page. Once the change passes through all the checks, it will land on the reviewers’s plate, and all you have to do is wait for it to be reviewed, approved and merged. 

> ## Short FAQ
>
> ### How will I know if the changes have passed the checks, been rejected, approved or merged?
> If there’s a change to the status of your pull request, Github will alert you via the email linked to your Github account, and add a notification to the  notifications icon of your Github account. 
> 1. Click on the notification icon.
><img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Notification%201.png"/>
> 2. Click on the notification with the name of the branch you submitted for pull request
><img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Notification%202.png"/>
> 3. Check out the status under the title! (Some possible statuses are: Open, Rejected, Merged, etc)
><img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/Notification%203.png"/>
> 
> ### How can I make a change to the pull request if it doesn’t pass a test, or there’s a request for edits from the reviewers?
> Go to your copy of the Tanzu Practices site, making sure that you are in the right branch to make the edits.
> <img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/MkChanges%201.png" />
> Click on the 'Content' folder, 'Practices' folder, the folder of the practice you edited, and then index.md. Click on the pencil icon to edit it.  
> When saving the edits, under Commit Changes, fill in the title and description for the change.  
> This time, commit directly to the branch. Do NOT create a new branch. This updates your pull request with your latest edits.   
> <img style="float: left;" src="https://github.com/Weimankow/tanzu-dev-portal/blob/Guide-for-Contributors-New-to-Github/Images%20for%20Guide/MkChanges%202.png" />
> That’s it!

## 5. Delete (delete repo)

Once you’re sure your edits have been merged, go to settings, and delete your copy of the repository. 
