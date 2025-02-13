# How to Make a Pull Request for ASReview  

Contributing to ASReview is a great way to support open-source research. But before you push 
changes, keep in mind that others are working on the same code. You want to avoid merge 
conflicts. That’s why you should always work on your own branch and fork.  

## Step-by-step guide  

### Step 1: Fork the Synergy repository  

Go to the Synergy GitHub repository. Click Fork to create a copy in your own GitHub account.  

### Step 2: Include all branches  

When forking, uncheck 'Copy the main branch only' to include other branches like development/v2.  

### Step 3: Clone your fork  

Now, you have your own copy of the repository on git. Find the green Code button on GitHub, 
copy the URL. Clone it to your local machine:

```sh
git clone <your-fork-url>
```

### Step 4: Switch to the development branch  

You should never work directly on development/v2. But you do start by switching to it.

```sh
git checkout development/v2
```

Check if you are on the correct branch by running:

```sh
git branch
```

### Step 5: Create a new branch  

To avoid conflicts, make a branch for your changes (from development/v2):

```sh
git checkout -b branch_name
```

Give it a clear name, like add_dataset_name if you're adding a dataset.  

### Step 6: Make changes and commit  

Edit the files as needed. You can check the status of your changes using:

```sh
git status
```

Then, stage and commit your changes:

```sh
git add .
git commit -m "Add dataset name"
```

Start the commit message with a verb, describing what you did.  

### Step 7: Push your changes  

Push to your fork:

```sh
git push
```

If you use GitHub Desktop, this step is easier.  

### Step 8: Create a pull request  

Go to your fork on GitHub, click Compare & pull request, and submit it to development/v2.  
Be mindful main is the default.  

### Step 9: Add a title and description  

Clearly describe your changes. This helps reviewers understand your work.  

### Step 10: Request a review  

Click on your pull request, then Request reviewers.  

### Step 11: Address feedback  

Reviewers may request changes. Make edits, commit, and push again.  
Your pull request updates automatically with your new changes.  

### Step 12: Done!  

Once approved, your changes are merged into ASReview.  

## Want to make another pull request?  

Before starting, update your fork to prevent conflicts:  

1. Sync your fork on GitHub.  
2. Pull the latest changes locally:  

   ```sh
   git checkout development/v2 
   git pull upstream development/v2
   ```

3. Create a new branch from development/v2:  

   ```sh
   git checkout -b new_branch_name
   ```

Check your branch with:

```sh
git branch
```

Then, follow the same steps!  

Now, you're ready to contribute to ASReview. Happy coding! 🚀
