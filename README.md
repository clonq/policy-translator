What
===
Translate for example

```
Allow everybody to retrieve anything from the public_documents s3 bucket
```
to

```
{
  "Version":"2012-10-17",
  "Statement":[
    {
      "Sid":"AddPerm",
      "Effect":"Allow",
      "Principal": "*",
      "Action":["s3:GetObject"],
      "Resource":["arn:aws:s3:::public_documents/*"]
    }
  ]
}
```
and back.