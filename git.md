# Local Environment Setup

- [x] [Github and Initial Setup](github.md)
- [ ] **Git**
- [ ] [Bash Configuration](bash.md)
- [ ] [Command Line Tools - Xcode (macOS only)](command_line_tools.md)
- [ ] [Rosetta Terminal (macOS only)](rosetta_terminal.md)
- [ ] [Homebrew](homebrew.md)
- [ ] [Node](node.md) 
- [ ] [VSCode](vscode.md)
- [ ] [Chrome](chrome.md)

## Code-Along: Git

**We will run through these steps together.**

---

Run the command below in your terminal.
**This script should be run from the root of this installfest repository.**

```bash
  scripts/git.sh
```

The script will prompt you for some information

1.  Provide your GitHub username
2.  Provide your GitHub email (email you signed up for your account with)
3.  When prompted, log into GitHub.com and go to [https://github.com/settings/ssh](https://github.com/settings/ssh)

4. Click the `New SSH key` button at the top right of the page

5. Enter a title for your SSH key (you can call it whatever you want)

6. paste in your SSH key. It should be copied to your clipboard already!

  *Help! My SSH key is no longer copied to my clipboard* (select your OS then run the below command in terminal)
  <details>
  <summary>macOS</summary>

  `pbcopy < ~/.ssh/id_rsa.pub`
  </details>

  <details>
  <summary>Linux</summary>

  `xclip -selection clipboard < ~/.ssh/id_rsa.pub`
  </details>

7. Click the `Add SSH key` button

8. In your terminal, press `[Enter]` to continue

    If you get a prompt along the lines of

    ```bash
    The authenticity of host 'github.com (xxx.xxx.xxx.xxx)'... can\'t be established.
    RSA key fingerprint is XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX:XX.
    Are you sure you want to continue connecting (yes/no)?
    ```

    Just type 'yes'. If everything's working, you should get a response like the
    following:

    ```bash
    Hi <your_username>! You\'ve successfully authenticated, but GitHub does not provide shell access.
    ```


**STOP! Make sure you did the final step before moving on.**

[Continue With Installfest](bash.md)
