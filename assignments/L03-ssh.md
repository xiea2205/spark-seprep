## SSH Practice

Note: `directory` and `folder` are interchangeable in the following tasks.

0. Your `public SSH key` in [this document](https://docs.google.com/document/d/1In6AP09tpR55C3jno_HZntkNrDZtqnz-KJuZMI07E5I/edit?usp=sharing) should live on your system at ~/.ssh/id_rsa.pub.

1. Your username is your BU email address without the `@bu.edu`. Copy your public SSH key to the virtual machine at `34.66.148.30`

```bash
ssh-copy-id -i ~/.ssh/id_rsa.pub YOUR_NAME@34.66.148.30
# password: buedu
```

For windows,
```
ssh -i ~/.ssh/id_rsa.pub YOUR_NAME@34.66.148.30
# password: buedu
```

1. SSH into the machine running at IP address `34.66.148.30`. Your username is your BU email address without the `@bu.edu`.

```bash
ssh -i ~/.ssh/id_rsa YOURNAME@34.66.148.30
```

2. Create a new directory `~/commandline-practice`..

3. Write the output of the `date` command into a file named `output.txt` located in the directory you created in Step 2.

4. Run the following:

```bash
curl -o /home/YOURNAME/commandline-practice/joke.sh https://raw.githubusercontent.com/DS219/spark-seprep/main/joke.sh
```

5. Use chmod to make it possible to run the command `/home/YOURNAME/commandline-practice/joke.sh`

6. Run the script and append the joke to the file you created in Step 3. You can copy/paste _or_ use `>>` to redirect the output of the script to the file.

7. Copy and paste the contents of `/home/YOURNAME/commandline-practice/output.txt` in a comment below the `JOKE OUTPUT` heading [here](https://docs.google.com/document/d/1In6AP09tpR55C3jno_HZntkNrDZtqnz-KJuZMI07E5I/edit?userstoinvite=somalley@redhat.com&sharingaction=manageaccess&role=writer#heading=h.n8wi69lc5x1p)

**HAVE FUN and ASK QUESTIONS!!**
