    composer require uspdev/senhaunicapixelfed

Colocar as variáves de ambiente:

    SENHAUNICAPIXELFED_KEY=fflch
    SENHAUNICAPIXELFED_SECRET=XXX
    SENHAUNICAPIXELFED_CALLBACK_ID=
    SENHAUNICAPIXELFED_ADMINS=
    ENHAUNICAPIXELFED_SECRET_SUDO=


Ambiente de dev:

    $user = User::where('username', '5385361')->first();
    $user->password = Hash::make('123');
    $user->is_admin = true;
    $user->save();
