代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bgdqpcir.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mgwdhigt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ygqhkkeo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nobzeeds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltlzaczb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ordezvpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtmbbeqt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dflxtzvp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uocmmvwe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkxsajds.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3imuqazbz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gipxnuec.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlzvekdb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3itxrcpqv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mphhwmgp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nibfogxl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zoyzesnt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bjlgxqhv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vljeqyfp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3adyvrygh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wxanudge.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3nevqqdaf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3xnqqkkvy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fcqrcpnl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3nrlnqjxp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ehuoqyme.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3iqmfxhou.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3jpijlpyw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nmwnltuo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxaczrf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qvvvzcwy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3gyznbcec.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3jgggnrfh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3mdpororv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ojililyt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cxjlvxus.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mhjazaij.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqshbpsq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nghtmyhk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pmdyqamp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mzmjuvav.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmhptzxx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbyckxuk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3cyupzadh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qdvdlfik.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ufbidoqr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wtmsfuqd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lhcghfla.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bbewwzfq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cztwqrtq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fypgyrjp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kvscsbam.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fadhgtnu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3hvznxddt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ftelskfp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vsxzjemv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tukapysi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lmrhfdew.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vuuormvd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jsfwyaar.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bjruxhzh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3varlwtzk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqsektn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xbghbydj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xwiaowae.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rbvlrqcy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3nkilguei.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fzomuydq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3sgzwupph.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fhjuiuav.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hjviompo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3draeqfxr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kixpbqld.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jqpwbeut.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fjoxgfcc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3imjgfesa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lwjyreda.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvgnhzox.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xlhmsfxi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xfzuhbwn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipxlwpth.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vmdhtylc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3txaervtq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yfaluzvh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsopghnn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hmilwfks.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3haxhfyld.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zpmfcdek.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3doorgqck.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3yzbsahhc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bacesdlr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hefakarn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vvhlpupb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pakxdnoi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qmgpptsf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3noyffzmi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3khtzfitk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xjtnncmn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3upwiihga.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ncynqrud.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yffzfbjc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3psoecnef.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nwrhsila.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wxchbzjy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3oqbadaoa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mvuncqfc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mlkaiocd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3orylkqym.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3inoffcuv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qpxrbjqf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uzsbazrz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3aytznrab.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hglqaqhx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hhrwblev.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gihptunp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pxvbndcg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pdycmrov.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ekmmthad.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3rswzmuts.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3auhcpjps.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3geomntah.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3argjtuhd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3iabhzdrd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3metstxww.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qeekfjmn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rchkbxxp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kicefbsl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zizhqfys.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuwllbhb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3gxjtmnqk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zkxjsjna.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hfdfpfet.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ybrvfqvi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gypbpvht.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zotgpyrg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3cmmtijag.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whmrpegp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3isvydziv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zrqmiguk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xunbaodz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3membekdo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mgvdpuvr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wgolpvhw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zxmyjuwh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3csfjyceg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zhlphfom.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cmalijea.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3txbkkfev.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3siggzwkk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3pkekwcuh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkuvjefb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkcrierg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mysgrdmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlmfpbta.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gajymrle.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3bqvyxyze.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jawykbzh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kaynbuyi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3hvzdponz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dydqqdew.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zexmhwgy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ikzdawox.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3daigsoia.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3srrmfiec.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ueargerk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gmqgtrht.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ulebpthj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gewdpcxm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dttoukeg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rttveduh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3uskjbyhh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3iqgmadok.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gznncdas.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ageftpdz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nvxfnylv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3gsbxrizp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3smnaefuw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xdnesuge.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cwniekje.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3sdivkdel.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pkecnhmc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3pjxuvbmg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rgzclekm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khtzemag.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3kivmmqwc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wftyaumm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrodxjzq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tzskafhv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aszdbwwz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vpbcwxtc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hrgopjzo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cbegjulk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kjakopxb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wlzsfrbe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3cgbczsql.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rdkeprsm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zdlkkuxr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3neswhscm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nwjfllfr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xsbspmix.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yldikmjt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bdzsnzpk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jlcyqevd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fomglhkl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3osozwtoz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eszxuggn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3thkhtori.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3cpxgtpbh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3kazeqiln.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ysjpyavm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lhdicfke.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qcirxvfm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kgwumxvq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kvtwscsd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eszbwrdj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qsfabuuw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ghlayute.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3laivkbpi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3sudzyuoq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xfoxrpfo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hflwvjph.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3acdpahpt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nillqpsj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3amqkojoe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hnmpfwwd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fuozvwcj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qizzheob.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ztahqijz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3gbqdevpf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3lwbyvbfg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wlhsoyxh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kdwcoijj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3prjmjimx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ctwfczog.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3iolxfkny.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sgfopzay.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3isyafjti.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tjdwthuc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uhpjmxik.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3diwyrcfd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3saqkvplt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3izwesnkz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3dfiqhuap.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3keefazkb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mvsiilgi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ggzgvnlf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbzkipca.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zyvfnhog.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3aonlhjta.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3obmkshqd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nnchifki.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ybjfqjkf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hyswlfyf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zvgrhogv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3upvxwwry.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3puvzvxdy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wkxpemgs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3obuueeyv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3sudmvzea.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ozlqbuuh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jviskicg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wbrulgql.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fehdozbi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3csttcvrh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yugayjrq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vosvtrnx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wdkyiwvc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jslesukp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3saafaojr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3niknnads.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nxvqjfhf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3moliwbbg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vdazszxx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sosyiylt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3niowqxfz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fgrnourx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mfyudeol.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uxbflwea.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iddmujpq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zrziwihk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hktagdrv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zhlwaviy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ocjiregn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3blsyinnl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gvqvafew.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3uuqmwlnq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qeedwufv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jgqqmzpq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xcbmmekd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3viuoaysz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ynloezya.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3noenzhpj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fwxpghup.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kcteqogb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3trmhbutq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bjzudxvx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xylmypfq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ggegmvig.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3amqmscnm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iujoazaq.html


<!-- 参考信息 -->