

package main

import (
  "bufio"
  "fmt"
  "os"
)

func main() {
  deli()
}

func deli() {
    
    
    a:=make(map[string]int)
    a["Osh"]=45
    a["Manti"]=8
    a["Shashlik"]=13
    a["Somsa"]=7
    a["Tandir go'sht"]=170
    a["Ko'za sho'rva"]=30
    a["Lag'mon"]=22
    a["Beshbarmoq"]=90
    
    b:=make(map[string]int)
    b["Pepsi"]=12
    b["Coca-Cola"]=12
    b["Fanta"]=12
    b["Sprite"]=9
    b["Family"]=5
    b["Montella"]=5
    
    
    d:=make(map[string]int)
    d["oddiy salad"]=8
    d["olivia"]=9
    d["uyg'ur salad"]=11
    d["k_salad"]=10
    d["g_salad"]=15
    d["d_salad"]=18
    
    
    
  
//  Foods Menyu...................................................................




  a_count := 0

  fmt.Println("\n....................Food Menyu.......................\n ")

  for food, price := range a {
    fmt.Printf("%s - %d ming so'm\n", food, price)
  }

  scanner := bufio.NewScanner(os.Stdin)
  fmt.Println("\nFoodni kiriting:")
  scanner.Scan()
  taom := scanner.Text()

  for food, price := range a {
    if food == taom {
      a_count += price
    }
  }

  for {
    scanner := bufio.NewScanner(os.Stdin)
    fmt.Println("\nYana biror bir taom xohlaysizmi: [yes/no]")
    scanner.Scan()
    add_food := scanner.Text()

    if add_food == "yes" {
      fmt.Println("\nFoodni kiriting:")
      scanner.Scan()
      taom := scanner.Text()

      for food, price := range a {
        if food == taom {
          a_count += price
        }
      }
    } else if add_food == "no" {
      break
    }
  }

 
  
// Drinks Menyu.....................................................................




  b_count :=0
  
  fmt.Println("\n.......................Drinks Menyu....................\n ")
  
  for drinks, price := range b{
      fmt.Printf("%s - %d ming so'm\n", drinks, price)
  }
  
  
  scanner1 := bufio.NewScanner(os.Stdin)
  fmt.Println("\nDrink kiriting: ")
  scanner1.Scan()
  drink :=scanner1.Text()

  for drinks, price := range b {
      if drinks == drink {
        b_count += price
     }
  }
  
  for {
        scanner1 := bufio.NewScanner(os.Stdin)
        fmt.Println("\nYana biror bir drink xohlaysizmi: [yes/no]")
        scanner1.Scan()
        add_drink := scanner1.Text()

    if add_drink == "yes" {
      scanner1 := bufio.NewScanner(os.Stdin)
      fmt.Println("\nDrink kiriting: ")
      scanner1.Scan()
      drink :=scanner1.Text()

      for drinks, price := range b {
        if drinks ==  drink {
          b_count += price
        }
      }
    } else if add_drink == "no" {
      break
    }
  }



// Salads Menyu............................................................


  d_count := 0
  
  fmt.Println("\n.......................Salads Menyu............................\n")
  
  for salads, price := range d{
      fmt.Printf("%s - %d ming so'm\n", salads, price)
  }
  
  scanner2 :=bufio.NewScanner(os.Stdin)
  fmt.Println("\nSalad kiriting: ")
  scanner2.Scan()
  salad := scanner2.Text()
  
  for salads, price := range d{
      if salads == salad {
          d_count +=price
      }
  }

  for {
      scanner2 := bufio.NewScanner(os.Stdin)
      fmt.Println("\nYana biror bir salad xohlaysizmi [yes/no]")
      scanner2.Scan()
      add_salad :=scanner2.Text()
      
      if add_salad=="yes"{
        scanner2 :=bufio.NewScanner(os.Stdin)
        fmt.Println("\nSalad kiriting: ")
        scanner2.Scan()
        salad :=scanner2.Text()
          
        for salads, price := range d{
            if salads == salad {
                d_count +=price
            }
         } 
      } else if add_salad =="no" {
            break
     }
  }
  
  fmt.Println("\n..............To'lovlar....................:\n")
  
  fmt.Println("\nFoods Balance: ", a_count)
  fmt.Println("\nDrinks Balance: ", b_count)
  fmt.Println("\nSalad: ", d_count)
  fmt.Println("\nUmumiy to'lovingiz: ", a_count+b_count+d_count)
  fmt.Println("\nTashrifingiz uchun rahmat!!!")
  
}
