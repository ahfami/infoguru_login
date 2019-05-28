module['exports'] = function gorgomBot(hook) {

    // impor modul request
    var request = require('request');

    // mengirimkan request ke server API telegram
    request.post('https://api.telegram.org/bot' + hook.env.bot_token + '/sendMessage')
        .form({
              'chat_id': hook.params.message.chat.id,
              'text': hook.params.message.text
    });
}
