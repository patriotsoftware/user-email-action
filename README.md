# user-email-action

Returns an email address or committer string associated with the user


## Parameters

## Output

#### 'email'
Email address associated with the user. Default is ```committer``` string.

## Sample Use

```
  get-email:
    name: User Slack
    runs-on: psidev-linux
    outputs:
      email: ${{ steps.email.outputs.address }}
    steps:
    - uses: patriotsoftware/user-email-action@v1
      id: email
```