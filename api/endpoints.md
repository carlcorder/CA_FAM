* `/json/account-settings/get`
* `/json/account-settings/set-individuals-v1`
* `/json/discussion/content/get`
* `/json/discussion/general/${forum_id}`
* `/json/discussion/question/${question_id}`
* `/json/discussion/post/vote`
* `/json/exam-generate`
* `/json/exam-validate`
* `/json/forum/user-questions/get`
* `/json/get-practice-dashboard`
* `/json/learn/get-user-schedule`
* `/json/learn/search-indexes`
* `/json/learn/update-content-visit`
* `/json/login`
* `/json/my-discussion/search`
* `/json/notifications/clear-unseen`
* `/json/practice/exam/get`
* `/json/practice/GetHistory/${exam_name}`
* `/json/practice/GetSectionReport`
* `/json/practice/score`
* `/json/practice/update`
* `/json/study/GetStudyNotifications`
* `/json/study/get-exam-dashboard`
* `/json/study/get/section-or-content`

Most endpoints require POSTing a JSON request payload E.g.

```json
{
  "id": "12345",
  "examName": "fam"
}
```

Some endpoints require in the request header
* `Refer(r)er: https://account.coachingactuaries.com/fam/xyz`

All requests will require cookie based authorization in the request header (hexadecimal string)
* `Cookie: .APAUTH=123456789ABCDEF;`
