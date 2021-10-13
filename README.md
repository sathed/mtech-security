# Certbot

1. SSH into the AWS instance assigned to you (posted in chat).
    * `ssh ubuntu@<instance>`
    * Ask Clint for the password.
2. Run the script 'create_record_set.sh' located in the home directory and answer question.
    * Example:
      ```
      $ What is your first name? john
      Creating DNS record: john.mtec-hosting.net
      {
          "ChangeInfo": {
              "Id": "/change/C1041944DHHYZW6RQTN4",
              "Status": "PENDING",
              "SubmittedAt": "2021-10-13T02:21:39.164Z",
              "Comment": "CREATE/DELETE/UPSERT a record "
          }
      }
      DNS record created successfully.
        Domain: john.mtec-hosting.net
        Public IP: 18.236.252.37
3. Use the instructions found [here](https://certbot.eff.org/lets-encrypt/ubuntufocal-other) to create your certificates. Start with step #3.
    * Make sure you use the Domain from step two to create your certificates.
    * When you get to step #7, choose the first command.
