# ApiRequestClass
Class Api Request Php

## Example of use

 - **GET:**
	

	    $urlApi = 'http://localhost:8080/';

		$api = new  ApiRequest($urlApi);

		$response = $api->get('patients');

		print_r($response);

 - **POST:**
		

		$urlApi = 'http://localhost:8080/';

		$api = new  ApiRequest($urlApi);

		$data = [
			'name' => 'John Doe',

			'age' => 30
		];

		$response = $api->post('patient', $data);
		
		print_r($response);

 - **PUT:**

		$urlApi = 'http://localhost:8080/';

		$api = new  ApiRequest($urlApi);

		$data = [
			'name' => 'John Doe',

			'age' => 25
		];

		$response = $api->put('patient/1', $data);
		
		print_r($response);


 - **DELET:**
 
		$urlApi = 'http://localhost:8080/';

		$api = new  ApiRequest($urlApi);
		
		$response = $api->delete('patient/1');
		
		print_r($response);


 

		
