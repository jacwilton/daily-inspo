# daily-inspo
pip install twilio
python setup.py install
$sid = '<AccountSid>';
$token = '<AuthToken>';
$client = new Client($sid, $token);

$client->messages->create(
  '<customer_phone_number>',
  array(
    'from' => '<your_twilio_number>',
    'body' => 'Thanks for your order! On a scale of 1-10 would you recommend ' .
              '[company_name] to a friend? Reply with the number 1 to 10 to this message.',
  )
);
