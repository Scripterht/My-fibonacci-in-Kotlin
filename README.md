# My-fibonacci-in-Kotlin
My first fibonacci code

fun main() {
	var a:Int = 0
    var b:Int = 1
    var c:Int = 1
    var option:Int = 1
    for (i in 0..18){
        when(i){
            0 -> println(a)
            1 -> println(b)
            else -> {
                when(option){
                    1 -> {
                        c = a + b
                        println(c)
                        option = 2
                    }
                    2 -> {
                        b = c + a
                        println(b)
                        option = 3
                    }
                    3 -> {
                        a = b + c
                        println(a)
                        option = 1
                    }
                }
            }
        }
    }
}
