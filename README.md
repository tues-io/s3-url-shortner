# S3 URL Shortner

I know, real original name... at least it explains what the app does.

It takes a simple YAML (.yml) file and turns it into a URL Shortening Service in AWS S3. Creating a URL Shortening Service in AWS is still completely possible without this, it does however allow you to use a GIT repository to view/edit and stage your changes before deploying them. This will also allow you to use Continuous Integration (CI) to deploy the changes. It also means you may be able to make wholesale changes (not sure of what options you can change yet).

## Benefits of a URL Shortening Service

In my humble opinion *every* company should implement a URL Shortening Service, the benefits can be more than they initially seem. For all examples I'll use a mock company ABC PTY LTD (`abc.com`). They have decided to run their URL Shortner on the domain `go.abc.com`

### URL Shortening

Firstly, the obvious reason for a URL Shortener for turning long URLs into short ones. Eg

```
Long URL
http://abc.com/services/window-washing-service/timely-service

Short URL
http://go.abc.com/serv-1
```

Benefits:
 * Easier to put on printed marketing material
 * Easier to tell people in verbally
 * Shorter

### URL Prettifying

Here we take a URL that my be unattractive and turn it into something that is a bit easier on the eye. Eg

```
Unattractive URL
http://abc.com/services/?prod=72de275ac0b40947de8bd2f8dfa8a150c01a7688c6b9534e5ad23dff173a0e99

Pretty URL
http://go.abc.com/services/window-washing
```

Benefits:
 * Easier to tell people in verbally 
 * Is self explanatory, easier to read
 * Shorter

### Redirects

This may not be obvious at first, but having the ability to edit an existing redirect can become invaluable.

Consider the following example. Company ABC has a marketing campaign on print media, they send out an email with the URL `http://abc.com/c/feb2016`, they send it off to the printerand get 100,000 copies of the flyer printer, they get the flyers back and realise they had actually signed off on the url `http://abc.com/c/FEB-2016`. As the URL is case sensitive and their CMS does not allow capitals in URLs. If they 

It would have been a lot    

### Maintenance Mode

## The File

```yaml
pretty-url: https://
```
