# Creating passwords for new accounts

A short online experiment for the course Applied Research Methodology at Vilniaus kolegija (group PI25E, Practical Work 2).

- Study page: https://divinesean.github.io/viko-password-study/
- Pilot link: https://divinesean.github.io/viko-password-study/?mode=pilot
- Test link (our own checks): https://divinesean.github.io/viko-password-study/?mode=test

## How it works

1. The participant reads the information and gives consent.
2. Task 1: a new password for a fictional study room booking portal.
3. The page shows either a short password guideline (group G) or a neutral text (group C) for 30 seconds (60 seconds before 10 November 2026). The group is chosen at random.
4. Task 2: a new password for a fictional e-book library service.
5. Two background questions: earlier password training and the device used.

Password strength is estimated in the browser with zxcvbn 4.4.2. The password text is never saved or sent. Only these numbers are sent to a Google Form that collects no names or email addresses:

```
mode,code,group,training,device,away,pasted,log_t1,log_t2,score_t1,score_t2,len_t1,len_t2,zxcvbn_version
```

`away` is `yes` if the participant left the page while reading the text, and `pasted` is `yes` if a password was pasted instead of typed.
