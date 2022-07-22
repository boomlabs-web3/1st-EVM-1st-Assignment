1주차 과제

# 1. 
메타마스크 지갑을 만들면서 ... 궁금했던 것은
어떤 기준으로 지갑 주소가 생성되는 것이였습니다.

간단하게 봐서는 hash값인데 어떤 방식으로 hash되어있는지 찾아보았습니다.

각각의 코인마다 지갑주소 생성방식이 다른데 아래는 비트코인 지갑주소가 생성되는 방식입니다.

먼저 비트코인 주소는 공개키로부터 생성되는데 생성 알고리즘은 SHA와 RIPEMD입니다.

Address = RIPEMD160(SHA256(public_key))꼴로 나타내어집니다.
마지막에 거친 RIPEMD160의 160이 hash한 길이를 의미함으로 주소값은 
160비트의 길이를 갖게 되겠죠. 이 후,Base58Check 인코딩을 통하여 사람이
읽을 수 있는 문자로 바꾸어 혼란을 방지한 상태로 사용자에게 제공합니다.
 
# 2.
해당 스왑의 경우 스마트 컨트랙트 방식으로 시행되기 때문에 거래소를 통한 특정 토큰
구입과는 다르게 직접 스마트컨트랙트를 실행함으로서 해당 토큰으로 교환이 이루어지고 해당 교환이
이루어지기 위해서 유동성을 제공하는 매체가 존재한다는 사실을 알게 되었습니다.

# 4.
시중은행에서의 대출과 다른점은 청산 임계값이 존재한다는 점이였습니다. 또한 대출금을 상환하기 위해
예금이 청산되는 것 또한 다른 점이였던 것 같습니다. 예치 측면에서는, 다른 사용자가 빌린 예금의 비율이
높을수록 이율이 높다는 것이 인상깊었는데 시중 은행의 이자율 같은 경우에는 정부 정책 및 은행의
재정 상황에 따라 정해지는 것으로 알고 있습니다.