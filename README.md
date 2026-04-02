    composer require uspdev/senhaunicapixelfed

Colocar as variáves de ambiente:

    SENHAUNICAPIXELFED_KEY=fflch
    SENHAUNICAPIXELFED_SECRET=XXX
    SENHAUNICAPIXELFED_CALLBACK_ID=
    SENHAUNICAPIXELFED_ADMINS=
    SENHAUNICAPIXELFED_SECRET_SUDO=

## workaround

if (isset($_SERVER['REQUEST_URI']) && str_contains($_SERVER['REQUEST_URI'], '/index.php')) {
    $uri = str_replace('/index.php', '', $_SERVER['REQUEST_URI']);

    // 307 = mantém método (POST continua POST)
    header("Location: $uri", true, 307);
    exit;
}
