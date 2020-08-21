# clothing_category_attribute_classification-with_Pytorch
> 시각장애인을 위한 웹 쇼핑몰 개발 중 이미지 분석(파이토치 사용) - 의복 종류 및 정보 분석

## Installation

-

## Usage example

이미지분석서버: 입력받은 의복 이미지에 대해 의복 종류 및 디자인이나 재질 등의 기타 정보를 분석하는 기능 수행

웹 서버: 웹 쇼핑몰을 동작시킴

이미지분석서버와 웹 서버는 TCP/IP 소켓으로 연결함

웹에서 상품 분석을 요청하면 이미지분석서버에서 상품 사진을 다운로드하고 분석을 수행함. 

분석 결과인 의복의 종류 및 정보를 웹에 반환함

- setup.py

   - 관련 변수 및 모듈 선언

- get_img.py

   - 데이터셋 생성을 위한 수퍼클래스

- server.py

   - 의복 종류에 대한 데이터셋 생성

- demo/test_cate_attr_predictor.py

   - dataset_create_super.py에서 호출하여 사용함

- core-evaluation/model.py

   - Inception Resnet V2에 SENet를 추가한 딥러닝 네트워크 모델

   - 하이퍼패러미터는 학습 후 정확도에 따라 조정해야 함


## Development setup

OS: Ubuntu 18.04

Framwork: 

Torch 1.6.0+cu101

mmfashion 0.4.0 (파이토치 기반)

Dataset: Deep Fashion Database

Python 3.6.9


## Release History

* 0.1.0
    * first commit
    * 의복종류(category)와 의복정보(attribute) 분석에 대한 코드
    * 개선사항: 성능이 다소 아쉬움

## Meta

김준혁 – wnsgur1198@naver.com

## Contributing

1. Fork it (<https://github.com/yourname/yourproject/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

<!-- Markdown link & img dfn's -->
