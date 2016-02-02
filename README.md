# $$_GIT_REPO_NAME_$$

[![Build Status](https://img.shields.io/travis/$$_GIT_REPO_$$/master.svg?style=flat-square)](http://travis-ci.org/$$_GIT_REPO_$$)
[![Coverage Status](https://img.shields.io/codecov/c/github/$$_GIT_REPO_$$.svg?branch=master&style=flat-square)](https://codecov.io/github/$$_GIT_REPO_$$?branch=master)
[![Latest Stable Version](https://img.shields.io/packagist/v/$$_GIT_REPO_$$.svg?style=flat-square)](https://packagist.org/packages/$$_GIT_REPO_$$)
[![Total Downloads](https://img.shields.io/packagist/dt/$$_GIT_REPO_$$.svg?style=flat-square)](https://packagist.org/packages/$$_GIT_REPO_$$)
[![License](https://img.shields.io/packagist/l/$$_GIT_REPO_$$.svg?style=flat-square)](https://packagist.org/packages/$$_GIT_REPO_$$)
[![StyleCI](https://styleci.io/repos/45420482/shield)](https://styleci.io/repos/45420482)

## Start

### 1: Create new repository

for this exemple i use skimia/foundation

Create and clone locally the new repository

Download this repository as Zip & copy all files in the new repository

### 2: Search & Replace

<table>

<tr>
  <td>$$_GIT_REPO_NAME_$$</td>
  <td>Skimia/Foundation</td>
</tr>
<tr>
  <td colspan="2">
  Nom du repository
  </td>
</tr>

<tr>
  <td>$$_GIT_REPO_$$</td>
  <td>skimia/foundation</td>
</tr>
<tr>
  <td colspan="2">
  Respository GitHub UrlFormat
  </td>
</tr>

<tr>
  <td>$$_GIT_REPO_FIRST_$$</td>
  <td>skimia</td>
</tr>
<tr>
  <td colspan="2">Respository first urlFormat</td>
</tr>

<tr>
  <td>$$_GIT_REPO_LAST_$$</td>
  <td>foundation</td>
</tr>
<tr>
  <td colspan="2">Respository last urlFormat</td>
</tr>


<tr>
  <td>$$_GIT_REPO_EMAIL_$$</td>
  <td>kessler.dev@gmail.com</td>
</tr>
<tr>
  <td colspan="2">Respository Push Email</td>
</tr>
<tr>
  <td>$$_GIT_REPO_USER_$$</td>
  <td>Kessler Dev</td>
</tr>
<tr>
  <td colspan="2">Respository Push Username</td>
</tr>


<tr>
  <td>$$_GIT_REPO_NAMESPACE_$$</td>
  <td>Skimia\\Foundation</td>
</tr>
<tr>
  <td colspan="2">psr-4 CLASS NAMESPACE</td>
</tr>

</table>


### 3. Commit to master

### 4. Submit new package to packagist.org

Setup the github service hook for your packagist package.

- Go to repository "Setting" Page on github
- Navigate to "Webhooks & services" tab
- Click "Add Service" dropdown button & find packagist
- Confirm your password
- Add your Packagist username & token, validate by the button "Add Service"
- you can check by navigate to packagist service hook in the list bellow to the "Add Service" button and click "Test service"

### 5. Submit new package to styleci.io

go to your style ci account & activate styleci for you new repository

- Annalyse the new repository & go to this annalyse details
- click on the badge
- copy the markdown format to your README

### 6. Travis

before register travis you must setup github secure (for Documentation couscous)
tuto [here](http://couscous.io/docs/travis.html)

```yaml
env:
  global:
    - secure: your_key_here
```

- go to your travis profile
- activate the new repo ( you can sync for view your repo)

### 7. codecov

automatic settuped from travis


### 8. Commit to start automation

### 404 Error on documentation Page

delete your gh-pages branch on github.com & rerun travis build

### Need Package dev require

if your package need a dependency in dev version, you need to add the following in your `composer.json` file

```json
{
  "minimum-stability": "dev",
  "prefer-stable": true
}
```
 modify your .travis.yml to add this line bellow `- composer create-project laravel/laravel`
 `- php .fix_stability.php`

## Documentation

Please refer to our [online documentation](http://$$_GIT_REPO_FIRST_$$.github.io/$$_GIT_REPO_LAST_$$/) for more information.

## License

This package is licensed under the [GNU GENERAL PUBLIC LICENSE](LICENSE).
