代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3taumzmsh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ijldmuwd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjzhooys.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kwrjwikh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wptiahhk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hhekivwt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3gdhqimti.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3aagrybic.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3smcsyibs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wpkhkoqz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hvwgimwx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3fongnbzg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gznuohou.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bgirhqlw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnaaxtrc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3kswvllbh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3schiigml.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3enrgyijj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ronnadcg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nsjnbxdh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tfgdqtni.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgcnwgpg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3dsszjghp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kixvooow.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rzjeluhh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bsraspeo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcyhsbyw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mbmvclws.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eqvxypxk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3gztrbqgj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3icrfnwyw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sirhjwqm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3scrtjvrl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xksdqnbz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3znnhrhlg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bkcwybvt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ovqqelyv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3chdlzhvs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3abootyvw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vyxaeeoa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3njtetzon.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dwrjspol.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sfseoeiv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wqiikgda.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bnsrrtjz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kjsrtocw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3tfsvvmcp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ydmpamwk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3otvabcco.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3vznjdxwl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3unzjmqyi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3wrswrdqn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ycpjhxwj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bfcpspno.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3nuqntbvj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3cyxuwfro.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ydiftolc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlaysvkv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yooxoufz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3phgwajnf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ofryqwmz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwtizmez.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3olufeydi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3leqhdiiy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsjhtdgm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kexgziqq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3imrsaszg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gekphyax.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlwphrqi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wgleftva.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3auiwaxuv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3aalzjwpe.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bzhnpxeb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hatjfkbt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3omtbusjx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zohkcfji.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3opeogliw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bfwyduaq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xnkxjvyg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gqvgnrhk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zjsviwlb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3dsabjitd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3eywwhniw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3odrfwnav.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gwdkqiar.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ahwnkjre.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xxpsvpur.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3tngfhxod.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ifszwhab.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3fhlsvmyw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qdkbpjaz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lzeyczbc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mipfsisl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3psfxoatg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3eyljkjnw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3bopcatcz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3obmlmekq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jmyeafay.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3rxgrvgvt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3lkjlazns.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ugjydwhn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nhxjppjf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jcepzqlg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjyknsan.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvekxomx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nnrrciad.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3fllgzeuq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vuwowuis.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mapsuxiz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rrmwjvwg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zbnqixop.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yylbigeb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnuaritb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxnlxagl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3soueavqh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xtgevkvq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ahzpqrnr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fvhpilfs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3jukjseci.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zbfwgxcq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynbsqace.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lofaytmw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uwubzrbm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uqnidjjf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3srxrmiam.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jpqlowmj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3makrrexp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nyhqqfed.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vemprtsp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jkgxhqtv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xzppwqdd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qnsfelau.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yjtbxzti.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mqinzqhu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spdwgvaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npodwrpu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3owgabjsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjnfgdhg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3aegtsdvl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3arvyjrry.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xfikmtld.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eabtanvl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3warqrcry.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rrerykze.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3waqgrzff.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ivuozmxe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ocgevhxf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fmmoidqt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eugnpkfb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3luabfvux.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mnbhgiwi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qganzeuq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ljnafzgb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ayajjhyy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3spzqsxrv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xjprrigi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3akrizmiw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ctkgtptq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3tnwjpyjq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3efmqywhv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jpjluxix.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ybnphtgv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rbupyzqs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dtcplftw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qvhjtybv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ahuswyeg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cyzjtuyj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfpmjggi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hglkciew.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qzebpvvs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rbeaptbp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3udapsvpy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oqeawcbd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cyvwnaco.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vlyuzvxe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qkfcfndg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3djsikbpf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nrkdpeuc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cuyztglj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iyczkjld.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fceuwolu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rncsxkwb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3roumksbh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oksssudl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isgotpxx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vlygdfnh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ancknmbm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dbnjybal.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hyxlskdg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lslcoltz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hhcmvaid.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nqqkxchz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3yxcldtrb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kflqnsyu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xwxxhmuu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nnwptaha.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3niqzzcdv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oivzzlar.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rdkjhkrk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ymslpmju.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ymwxhpuh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ijmagiwn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bumbhply.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fgosgbfw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3hlqtjeho.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3asfidnsq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eyodiawk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fuqvkreh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lyetsqoi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ijesyxgl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lmhtdxtx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ncfmkpab.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tcrhlpdz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ywugdacx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3pncywumz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yrrtvpqs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zgqksisb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3voefafvr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3knjzaifx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3skzwhkqw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nnjzwwta.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xyrywjmh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nslqveqb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jpcdkusv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wugpzkns.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3mfnyzyhq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tqwirvsr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uincsxpk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jzxgtjcl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3uflaqcwr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zbpereqa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nueppdse.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3whlrtrbj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nqhcutdi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ukihclmo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rtzlykoy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3jrnrvrpk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3onuqxomz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3whwnnjfh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3muizsxtm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vhsmwgax.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gxurbcoc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uhxagadz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qiiauxob.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3utrezquj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3enwyzyqg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cxemowaq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3byfmlxcm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rcwkftha.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cptfnrsm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvwahna.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3urqdmsdi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qgjwyesn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3jmwzjdds.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmyjglrp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mgiakwlm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ewpslhji.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3okidtkrf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cyrhtfwt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hfkqgwgy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3eocrtsgc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xdffjdic.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qsynsynd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3firwkneg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3dgtdhzpa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lwfwxwjh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mxgwuooe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ekegxdta.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3krepetcs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nihhmxin.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qrhhrklm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rgjlvzoa.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3blaacfrh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jyjtbjar.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rpawsneo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sgqxcerl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yygyucsv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tomwoxrs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3apzebdda.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tokiyuoj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3dvlsyuld.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3oriyiama.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aldqxsaq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tajqimcm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tkggtnsn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3olihrjfy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jtygciby.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rktderes.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qidnqvpl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3tzzfzjft.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3zwxioyzf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3inawlfdv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3plpargkg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtnwcgd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wfjcwhlo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ipmqtqxa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3earwyaum.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zyohyiqd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bnxwjmiz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ajfgkdnn.html


<!-- 参考信息 -->