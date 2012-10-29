# jquery.passwordMask

__jquery.passwordMask__ is a jQuery plugin to allow users the ability to toggle password masking. By default, it renders a checkbox that, when clicked, will unmask the password field, allowing the user to read the entered value. This provides two key advantages for login and sign-up forms: (1) it grants users the ability to check for and correct typos, and (2) it would remove the need for the second password field used to ensure matching values.

Credit for the idea is due to Anthony T, author of the Smashing Magazine article "[Better Password Masking For Sign-Up Forms](http://uxdesign.smashingmagazine.com/2012/10/26/password-masking-hurt-signup-form/)"

## Demo

To get an idea for how the plugin works, visit the demo site:

[http://aduth.github.com/jquery.passwordMask/](http://aduth.github.com/jquery.passwordMask/)

## Usage

#### Default (no options)

    <input type="password" id="pwd_noparam">

    <script>
        $(document).ready(function() {
            $('#pwd_noparam').passwordMask();
        });
    </script>

#### Shown by default

    <input type="password" id="pwd_shown">

    <script>
        $(document).ready(function() {
            $('#pwd_shown').passwordMask({ isShown: true });
        });
    </script>

#### Custom toggle text

    <input type="password" id="pwd_customtext">

    <script>
        $(document).ready(function() {
            $('#pwd_customtext').passwordMask({ toggleText: 'Make password visible' });
        });
    </script>

#### Custom toggler

    <input type="password" id="pwd_customtoggle">
    <button id="btn_toggler">Toggle Password Visibility</button>

    <script>
        $(document).ready(function() {
            $('#pwd_customtoggle').passwordMask('#btn_toggler');
            // OR: $('#pwd_customtoggle').passwordMask($('#btn_toggler'));
            // OR: $('#pwd_customtoggle').passwordMask({ toggler: '#btn_toggler' });
            // OR: $('#pwd_customtoggle').passwordMask({ toggler: $('#btn_toggler') });
        });
    </script>

## License

Released under the MIT License (see LICENSE.txt)

Copyright (C) 2012 Andrew Duthie