# What is a good commit?

Good commits answer three questions:

1. Why did you do this commit
1. What did this commit do
1. What are the side effects

And they make only 1 change per commit.

## Why did you do it?

Why is important so your team members don't treat your work like a black box.
They want to know your intent.

## What did this commit do?

What gives an overview of the code changes so your team mates don't have to read
all the code to get an idea of how it has changed.

## Only 1 Change per commit

1. It's really hard to rollback if you have a bug in one of the pieces.
1. It's really hard to review commits if they make multiple changes.

## Only 1 commit per Change

1. It's really hard to rollback
1. It forces you to break your problem down smaller

## Never commit commented code

1. You're not going to use the code
1. You're probably going to write it better next time
1. It gets confusing!
