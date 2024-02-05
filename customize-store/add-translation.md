# Add Translation

> Currently, Mustom support English, Korean, Chinese(Simplified), and Japanese. But, you can easily add any languages you want.

## Part 1. Add new language for admin panel

#### 1 . Navigate admin-panel/src/config/language.json, and open this file using text editor.

#### 2 . Add new language like below. (Let's say you need to add Español)

```
[ 
    ...    
    
    {
        "name": "Spanish (Spain)",
        "code": "es-ES",
        "path": "es-ES",
        "description": "Español"
    }
]
```



{% hint style="info" %}
Please note that the value 'code' and 'path' are combination of ISO-3166 Country Codes (Upper case) and ISO-639 Language
{% endhint %}

#### 3 .  Create new folder under 'admin-panel/public/locales/{new foler}'

The folder name should be same as the value of 'path' that you added on language.json. (e.g. es-ES)

#### 4 . Copy all files under 'admin-panel/public/locales/en-US', and then paste it into new folder.

#### 5 . Let's start translation! The the translation below is an example.

```
// This is en-US admin.json file.

{   
    "grid": {
        "topTitle": "Admin Users",
        "topButton": "Register New User",
        "id": "ID",
        "firstName": "First Name",
        "lastName": "Last Name",
        "email": "Email"
    }...
}


// Translate it to Español like this.

{   
    "grid": {
        "topTitle": "Usuarios administradores",
        "topButton": "Registrar nuevo usuario",
        "id": "ID",
        "firstName": "Primer nombre",
        "lastName": "Apellido",
        "email": "Email"
    }...
}
```

#### 6 . You are all done! (You can share your translation to help others. Please PR!)



## Part2. Add new language for engine

When it compared with admin panel, the translation for engine are not much. Only a few terms like status name, and email templates can be translate.
