# fuzzy-octo-guide
Para criar um programa de automação residencial em PHP
<?php
  require_once('wiringpi.php');

  // Define o pino GPIO
  $pin = 0;

  // Inicializa o WiringPi
  wiringpi_setup();

  // Configura o pino como saída
  pinMode($pin, OUTPUT);

  // Liga o relé
  digitalWrite($pin, HIGH);

  // Espera 1 segundo
  sleep(1);

  // Desliga o relé
  digitalWrite($pin, LOW);
?>
