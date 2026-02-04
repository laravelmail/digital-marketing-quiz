# Digital Marketing Quiz

Professional email template for conducting a digital marketing quiz across multiple industries, tailored to engage recipients and enhance their understanding of the field.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Industry1, Industry2
- **Message Type:** Marketing Email
- **Tags:** digital marketing, engagement, quiz

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/digital-marketing-quiz.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/digital-marketing-quiz/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.digital-marketing-quiz',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
