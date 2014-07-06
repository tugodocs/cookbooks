# Scala Cookbook

## File Handling

```scala
    import scala.io.Source
    
    def readFile(fileName : String) : Array[Sample] = {
      val lines = Source.fromFile(fileName).getLines()
      lines.next
      lines.map(fromString(_)).toArray
  }
```
