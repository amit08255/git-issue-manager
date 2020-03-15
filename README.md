# Git Issue Manager

Git hook scripts to handle issues with Redmine/Planio. 
This script will allow developer to automate workflow by enforcing adding issue number in commit and will automatically update issue with commit message.


* `prepare-commit-msg` -- Git hook to add issue number and link to commit message. If no issue is created, it will enforce user to create an issue and add its number in configuration.
* `post-commit` -- Git hook to update Redmine/Planio issue (if multiple issue number and links are added, it takes first one) after a commit with commit message, commit ID and commit URL.


## Git configurations

* `issue.number` -- update this issue if issue ID or number in config is not blank.
* `issue.project` -- redmine project name where issue will be posted.
* `issue.user` -- user ID to which you want to assign issue when it is created.
* `issue.apikey` -- Redmine API key to access API.
* `issue.host` -- Redmine site URL.
* `issue.commiturl` -- Commit URL. Example -- For https://github.com/name/project/commit/id it will be -- https://github.com/name/project/commit/
* `issue.isclosed` -- "true" if you want to close issue on post-commit

## Getting Started

Copy Git hook scripts in hooks folder `.git/hooks`.
Use below command to provide execute permission to script --

```sh
chmod +x script_file_name
```


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Amit Kumar - [@amit08255](https://twitter.com/amit08255) - amitcute3@gmail.com

Project Link: [https://github.com/amit08255/git-issue-manager](https://github.com/amit08255/git-issue-manager)

