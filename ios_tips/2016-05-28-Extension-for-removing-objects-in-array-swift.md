---
title: Creating `Array` in swift to remove object and remove identical objects.
tip-number: 05
tip-username: arasu01
tip-username-profile: https://github.com/arasu01
tip-description: In swift we don't have methods to remove the particular object, instead we can remove object at index. Here we are using the same concept to identify index of the object and deleting the object.

---
#### Code

    extension Array where Element: Equatable {
    
        // Returns the indexes of the object
        public func indexesOf(object: Element) -> [Int] {
            var indexes = [Int]()
            for index in 0..<self.count {
                if self[index] == object {
                    indexes.append(index)
                }
            }
            return indexes
        }
    
        // Removes the first given object
        public mutating func removeObject(object: Element) {
            if let index = self.indexOf(object) {
                self.removeAtIndex(index)
            }
        }
    
        // Removes all occurrences of the given object
        public mutating func removeObjects(object: Element) {
            for i in self.indexesOf(object).reverse() {
                self.removeAtIndex(i)
            }
         }
     }

