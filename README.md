# codeigniter-url-encryption
A Codeigniter Helper that used to encrypt parameters that sent via URL. 

## How to use
1. Copy files to Codeigniter project
2. Load through controller constructor
    ```php
    public function __construct()
    {
      parent::__construct();
      
      $this->load->helper('url');
    }
    ```
3. Use the function on controller or view
    ```php
    $plain_text = 'This is a plain-text message!';
    $cipher_text = encrypt_url($plain_text);
    
    // outputs: This is a plain-text message!
    echo decrypt_url($cipher_text);
    ```
