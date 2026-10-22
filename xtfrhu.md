代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ybfczigt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zordvdtf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2srhjkpvg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jytuhvxz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2bsylpvfb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojhyfhsu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2onrsvwyq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wootehkp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xfzvoazb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ehqjsjwr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hqzizvav.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wvzbiuwh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ttdheyep.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zqrvzchb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nxxeepxc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xvaaweme.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2obccfqfv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2eiodehji.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2sweguvrk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zhaxcote.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rlnkjslx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ruygjela.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ivedhsyc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hhffodcd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eybyixsq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2igiyamfe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qcstzize.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lwjyxhqb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2usyazdjl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ehyuhkqr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vkzjbnqx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2blsukqmy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qxnrgpnc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2riqllkxp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ongxbgqk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2whwybegj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzzreqk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jahjsoxz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2moydxrgp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2bbnhyirn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ecdimiaf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pwpzjyhp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ewfufhqu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ddnfjnos.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qwarqxxx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qltrxktz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ceofxdok.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lwdmsjei.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hidcanjs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ffvcoekr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2skponbtp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jjlstwfe.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2zdpiljqt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wrkqjlzh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vliqqcse.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2hxwfatwc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ynstvsgz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2usbagmxb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bybecptn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jwxfbvfj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tyqyusag.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ftbpowgg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2nttthtao.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2iydhtwln.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2chhlnioe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2hjykymir.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2uwtpjhst.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kigyzegr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mipxbapj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pdubzqyn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2oxtqvksv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2geeqhxak.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2uyixtccn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yjjispxn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nwlazzek.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2erejbjzt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xtklbvbx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2vsuvogev.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2izlpjfdg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dydxswhk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zqiksugu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nvwqlrvc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gygkfeep.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyrrcjsu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwotnbzp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2bdcwoisp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tmgedthc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tupkcsmc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wbihbuhj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2txtrwgmo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bfogghdd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bumoizcp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wuobijaa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hujptriq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kvhgffmc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wbvtsrxd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pagwgldy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2sfomrcxj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2yrcjjtay.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fiymvypf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbmjdlzp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxxdwklg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uqrekvdb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gdunuphs.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ahkmtznv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bzsrwhqw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ieyueeew.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jyllhzgc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2olzbkjwl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qaipryxf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2uulbztfv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2sxeugffi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ydpalmov.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lwvsjbjz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjtbvosk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2femjnoet.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hcjdvyah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppppmzig.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hecuuhqi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2feljwrxk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2piaifkpx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vzkhqgmu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2nztswvlp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2inipqwpy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ogsndyza.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jghsxova.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lwdjlhcb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2eguaqxgz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hzrhmvkm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2hzjhhrqy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iccwoled.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rqtcythh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rwplqnbw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bewpilst.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ispykymq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2avgvoacz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fdhvkwqz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zpawdqon.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gytdceqa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vjnwmjfk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gqpiyqci.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2djszqkcr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2givcspbj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yeibqorc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dgssrikm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fvhbnytm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xxhaixig.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2buqwnikh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2knlhghtx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qmdsjvyj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kbycbttz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ojeuvczh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iggmrfmy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vtjxhwst.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vtdmlyrp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2egbglaig.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zlqcbzkx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zqjgfkfn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lbwubnfn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2whphozyd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2btkhnffs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kscxwzkk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wupmyqpx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vtikuhmc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rosbxnes.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bqemmgje.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2axtggask.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pfmjrsgp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lbfkspxi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ogiqxnwu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xuwfbsyc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2okcyfusi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pnxoievk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2spsorhxp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2odlczkln.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mmgpxynf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2medygrnz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2welwyisq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qqaancbk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bsmfwhow.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xavvdahh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2zlgrgdwr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2spnkimhx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bdknjmcd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2frviktxg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qkpkveuz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dnzpuxrc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2hpmdkfbw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2mgxzkgxg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nanspocg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2pkfrkpbz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tasftzxy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kgthzwox.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2pjkzgnfj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2twhxdexd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dalcvzrf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmnmrukv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cwplunqy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2osaairap.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2llrhqbld.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2snpmcfdz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lcsjzqya.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jacoeywa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rlyuhkgk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kbotcpoh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rrbcsmkj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2iralovxo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zhwsojvx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ntjzquhl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2gxwhlgxv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hnxttujf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zbvdgxyp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pejitguf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mcbqlqzb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xmvnjygr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mmyzrnde.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mqohixiv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2iazemhzu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qtpiyoqq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yblmfzpz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2obzltyhn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gjkhoatx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2lmkyymec.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2etjkhryn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2awacjwzf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2gnvgklli.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gjgljkhd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xfiutorl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zwfsowvk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pwqdfiyb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vaatthmt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ddywzoev.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zodinkdw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2obukbfsx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2quepdhpt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2edsmdnrn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lntvsyyc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cgttgbyu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xkrfclbi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kidgoxwl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2olvjedqk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jmhnefqz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sewxxcpr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2coiyzvcy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2icinrgfv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pksbbyor.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drfvoeyi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yrwyfene.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hwnxscrk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ebpzrpzb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mcwvcjdd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gytnvwur.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gikkyevp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ankkqiwv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fnhhmntj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2oppmdjdb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hvzgvlrd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aoxtuiue.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2uccgbhud.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2wdqnwgwh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nmxaykco.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kohlmtgo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rwdwcnjw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhckrwit.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omteaqnz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tczqeaxl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tjqioqft.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rdjaugqq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hjmneqrp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wazxjpqp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ijiwitiy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jahjtomj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cnqfjulq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pkebqvij.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ouruougm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2imaxjlnz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sewrvpks.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xzdtijsc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ldwsguwe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lpxmggcr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2aoyhlvrh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acqjtukf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2izszkiso.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2itepexpg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hfsyusgx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gwvkxxmk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xgailitf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2vbanhoqm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jzqcewsu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lnvvzhdb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhetjyd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xiepytht.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wscbdcdr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2klmizcvz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dtmbjbpa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vvjfuggg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bfzsbobx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ycoobrze.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2wazkwzej.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lygwrpsn.html


<!-- 参考信息 -->