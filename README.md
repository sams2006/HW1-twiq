# HW1-twiq

fun main() {
    var candles = 28
   var layers = 5
   println("Number of candels: $candles")
   println("Cake top length: $candles")
   println("Number of layers: $layers ")
    
  
   printCakeCandles(candles)
   printCakeTop(candles)
   
   repeat(layers){
      printCakeBottom(candles , layers)
   }
}

fun printCakeCandles(candles: Int) {
    print(" ")
    repeat(candles) {
        print(",")
    }
    println("")
    print(" ")
    repeat(candles){
        print("|")
    }
    println("")
}

fun printCakeTop(candles:Int) {
    repeat(candles + 2){
        
        print("=")
    }
    println("")
}

fun printCakeBottom(candles:Int , layers:Int) {
    repeat(candles + 2) {
        
        print("@")
    }
    println("")
}
