# mutable and immutable
mutable => list, set, dictionary

immutable  => int, float, tuple, str, bool
immutable은 하나의 immutable 값에 여러 개의 참조가 붙음
immutable 한 str의 경우, 
s1 = "BlockDMask"
s2 = "BlockDMask"
로 해 놓으면 s1과 s2가 같은 메모리를 가리킴. 하지만 s1과 s2를
s1 = s1.replace('D', 'ZZZ')
s2 = "BlockZZZMask"
이런식으로 동일하게 바꿔도 이제는 s1과 s2가 동일한 메모리를 가리키지 않음
