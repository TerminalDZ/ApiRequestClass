# ApiRequestClass
Class Api Request Php

## Example of use

 - **GET:**
	

	    $urlApi = 'http://localhost:8080/';

		$api = new  ApiRequest($urlApi);

		$response = $api->get('get-patient?id=1');

 - **POST:**
		

		$api = new  ApiRequest($urlApi);

		$data = [
			'username' => 'admin',

			'password' => 'admin',

			'remember' => 'true'
		];

		$response = $api->post('login-account', $data);

 - **PUT:**

		$api = new  ApiRequest($urlApi);

		$data = [
			'username' => 'wassim',

			'password' => '123456',

			'remember' => '1'
		];

		$response = $api->post('login-account', $data);


 - **DELET:**

		$response = $api->delete('patients/1');


 - **Upload File:**

		$data = [
			'file' => new  CURLFile('path/to/file.jpg')
			];
			
		$response = $api->UploadFile('upload-file', $data);

		
