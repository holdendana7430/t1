代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtsafbkf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pewgdeql.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ctwblypm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3szvvelqn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzmucocz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wjxtxphy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ejewwszx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ptvpwzqe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nypdjiwe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zpiuqlqg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nwbmoqjh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3qjrdiuot.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gnxnlgdp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzpjgati.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytyngsyy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ryxaqnar.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bmllpltf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hfigjhuc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fabsoxsi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3txwybzwm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3pmllqedc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sizuitjz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gmnstawc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ylkspsib.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3oxigwnty.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3odfkruft.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3pavansbu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3flvkpeod.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ikmfiqil.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3reabtsdf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ourqnntx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mtgvbefm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mmfzsbmb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ixxpbahs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zwnbyuxp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wnnkqrbf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3oqqacywh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ydvvbuex.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3plzlnmmf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zacmfret.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3oflcjqlp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ijqedlvu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3awtlfcva.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3snnkagsz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3davilhva.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lldglryc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkqgsnbz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vgmyfanl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qktpjjzd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ofqhrsqf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dgjokfrk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3orgyutbj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mesqecub.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3spqsmblz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3btvjungr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xclvioqo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mslraymq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zcnbxhvr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uyoldmfe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gsyqyzkj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3bigwuuvp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wolukhpg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dskncnqj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3hmledvpo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3veeexgxi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jxlugzqy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ffiggyli.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hryybbke.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sdfdssvg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3aqrlvvqy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fktggdgo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3obshkifb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xubdiuii.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3atlxshku.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rxyqjmue.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3acfllboz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qorcarbh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3opdaphgj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3rlxoxjvu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ihpawhkg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3sdjgxgqo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nlstjneu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3juxacvys.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3awmmakdw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gvbzfdxx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zhrxdzsm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kzresczd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3frsvxofy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ebigokob.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfablaio.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nxermzjo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cohmpzay.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3njfrpshj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3oabvotbx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vwoqjwev.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3doygbavu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vwvvtdiv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3wnpqcsam.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3onqilajn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kfqaajso.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvqmupix.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ciaumnwa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3gavrkhkc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pyvswtdy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3grkegyqv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dvytgffm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3iudtaoac.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ksxtgjmp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulclccij.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aujfltct.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qzfkvauy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yklluwlv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wtmmqtaj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kmphlucn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uvnmrsht.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rljwxxlq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hojowcmp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3angxmbwv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3mgucvfqy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvxtjunx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pjqjhkeu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rltvaopi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uorbykte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovksqquc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3edwpeagp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ioqkvqsa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gmvdpmfk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rgcrgyvl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3etsytscy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ygdoutbg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vsnswmry.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rjkeprmy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bxxhdwvx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ejguvhwq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zftzcigr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ocsftvvt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hfqknoil.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3utkozxza.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ljjheuot.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ktxmpnzk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqfvsnnd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nuertrzl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3jrhwnecd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vmztqgiy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xttxeyyc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pnheslsd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wtsqpsjx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yrzmjchd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ysaanfpi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dlgqlzng.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rellveso.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3chdycmkg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yjryhpkq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ojqqsblk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3frtvfozq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3iglbhukn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ytoakmvp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hztfzyna.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pdbjdxzv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qgtzsdoe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mmvjqlmt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jfvwjtfa.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bdxtfxpr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3drkeoaoz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gpwlohto.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sgfltoce.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3isizjsaj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3oorlrszr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ylvpneec.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3akznxggp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3arzndcrg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3coulaykx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3spzqmstn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jfyaxibb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cssufquf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xmhgcwln.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3tmbqfngx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dihdqpic.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lkxpceyy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zjjghnik.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ynrzygex.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3eznlqgqj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3irhzsoin.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ezwzfxov.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ayvmmznw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hvyfxzsw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3meduauih.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jfcmmxks.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cyellprh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pvpkdxmh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3slmizwks.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ahvbalqd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gnhpxakw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rubpahur.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3khcixpas.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3yfxwfaav.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rexzlcni.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qcghrlpp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3prkawhjr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tciatyec.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xmghrnww.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jkepyazw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jcefyoan.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ixupfdcm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jowgfhxg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xhnlwzim.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dkjpanxa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3buezyqtm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cxexwwiq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3albnnxyq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lilbtlcb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qjyifnud.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ajzcbegy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mnybsipv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jjxfbcec.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vxrfsrnh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lhzigvlj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lztyjauq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xkuekect.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cbosyhfb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3anjsqvxp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3igmwjdqe.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jzwgrdfe.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bsuwhfxz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dhjoegtu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xseoetck.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ztndqljm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qhxlolse.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gwvukdgw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mmanlfql.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gvajppxw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmqrdaan.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3iwjgxxrr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3oyqgrjzy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3exreosfw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hdxewitg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oicgrqzx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yncyxqgf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhxdniqh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jvhcaajg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vrmzwuio.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pvxiavmh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hoicofik.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3iyidunms.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rnsxbhah.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ojnpqrpf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3erjpvslf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhaayyaw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xekcjmbe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ydxzvjwd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pczcquwx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dlbvmlge.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3egwwijrh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dajcgqst.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gfnrmtyq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xbbvrlpy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nvghtrau.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vggvglph.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mhzpekav.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3rtwnrkbc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nizyyysp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3caamwtxd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vmtqvetx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtzfkezo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ultiedwl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gxzgglxg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jspvhawz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qartapst.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xpngjrrw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cdwaznda.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3corkeepk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mmrsmqco.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gagmcnmu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3xhlqjbze.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jcoanavz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oumdymwj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tphbzmmc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3pfmwdcqn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nrupehho.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3tdbojjfw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yuqlgowb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3isvskzyq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3milhnufo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vvvbznii.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jaayuanl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pobyosuv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ivtcevww.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3emmdclgo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wjxfhyzz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3euiiddpy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lkpoxlox.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dgoclblh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ontvixxr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3konkbdko.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3groezlua.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3raurfxjn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3eqxxqszy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ovtnldcp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bnsvyolk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gacjpwzw.html


<!-- 参考信息 -->