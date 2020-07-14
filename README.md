# iOS-DiffableDataSource-Study



## Diffable Data Source 란?

- collection view와 함께 동작하는 특수한 타입의 데이터 소스

- collection view의 데이터를 관리하고 UI를 업데이트할 수 있다

- [Apple Document](https://developer.apple.com/documentation/uikit/uicollectionviewdiffabledatasource)



## UICollectionViewDiffableDataSource 란?

데이터를 다루고 collection view cell을 제공할 수 있는 클래스

```swift
class UICollectionViewDiffableDataSource<SectionIdentifierType, ItemIdentifierType> : NSObject where SectionIdentifierType : Hashable, ItemIdentifierType : Hashable
```

- iOS13 부터 새롭게 소개된 UICollectionView API로, 기존의 UICollectionViewDataSource 보다 유연하고 선언적이게 데이터를 다룰 수 있다.
- UICollectionViewDataSource 프로토콜을 준수함 -> 관련 메서드 모두 사용 가능

