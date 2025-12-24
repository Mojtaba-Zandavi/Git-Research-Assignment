# What Happens Under the Hood When You Fork or Clone

### Fork (on GitHub)
- GitHub creates a new repository under your account.
- All commits, branches, tags, and files from the original repository are copied.
- A link to the original repository ("upstream") is maintained server-side.
- No local files are downloaded yet — everything happens on GitHub's servers.

### Clone (using Git)
- Git downloads the entire repository history (all objects from the `.git` database).
- A hidden `.git` directory is created locally containing the full commit graph, configuration, and references.
- A remote named `origin` is configured pointing to the repository URL.
- All branches and tags are fetched (though only the default branch is checked out initially).

Sources:  
- Fork: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/about-forks  
- Clone: https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository
