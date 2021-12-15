# Deallocation 문제
뷰 컨트롤러를 dismiss 해도 deinit 가 호출되지 않는 문제를 겪음

해결책 :
사용하는 모든 클로저에 [weak self] 를 붙여서 강한참조 문제를 해결

참고 링크 : 
https://www.swiftdevcenter.com/reasons-for-deinit-is-not-getting-called-ios-swift/
