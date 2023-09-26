# Writing Good Documentation 

## Step 1 - Using Codeblocks. 

Codeblocks in markdown make it *very easy* for tech people to **copy, paste and share** code. 
A good Cloud Engineer uses codeblocks whenever possible. 

Beacuase it allows others to copy and paste their code to replicate or research issues. 

- Inorder to create codeblocks in markdown, you need to use three back-ticks ```
- Not to be confused with single quotation '''

```
# Define the provider (in this case, AWS)
provider "aws" {
  region = "us-east-1"
}

# Create an S3 bucket
resource "aws_s3_bucket" "example_bucket" {
  bucket = "my-example-bucket"
  acl    = "private"
}

# Output the bucket name
output "bucket_name" {
  value = aws_s3_bucket.example_bucket.id
}

```
- When you can you shoud also attempt to apply syntax highlighting to your codeblock.

```yaml
# Define the provider (in this case, AWS)
provider "aws" {
  region = "us-east-1"
}

# Create an S3 bucket
resource "aws_s3_bucket" "example_bucket" {
  bucket = "my-example-bucket"
  acl    = "private"
}

# Output the bucket name
output "bucket_name" {
  value = aws_s3_bucket.example_bucket.id
}

```
This is by a way of drag and drop an image on to github
![Terraform logo](https://github.com/mexuscloud/github-docs-example/assets/115909140/84f464ba-3202-40a8-b1a2-3363f208e64d)

You can re-size an image this way by using an html img tag and specifying a width and height for the desired img size. 
<img width="200px" height="200px" src="https://github.com/mexuscloud/github-docs-example/assets/115909140/84f464ba-3202-40a8-b1a2-3363f208e64d"/>

Good Cloud Engineers use codeblock for both code and errors that appear in the console. 
> Here is an example of using a codeblock for an error that appears in bash. 

```bash
Traceback (most recent call last):
    2: from /usr/bin/irb:23:in `<main>'
    1: from (irb):1
RuntimeError: This is a custome error message
```

## Step 3 - Use GitHub Flavored Markdown Task List 

Github extends markdown to have a list where you can check off items. <sup>[1]</sup>

- [x] Finish Step 1
- [ ] Finish Step 2
- [ ] Finish Step 3

## Step 4 - use emojis (optional)

GitHub Flavored Markdown (GFM) supports emoji shortcodes. 

## Step 5 - How to create a table

``` md
| Name | ShortCode | Emoji
| --- | --- | --- |
| Cloud | `:Cloud:` | ☁️
| Cloud with rain|`:Cloud_with_rain:` | 🌧️
```

## References

- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)
- [Basic writing and formatting syntax(GitHub Flavored Markdown)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [GFM - Task List](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists)<sup>[1]</sup>
- [GFM - Emoji Cheetsheet](https://github.com/ikatyang/emoji-cheat-sheet)



