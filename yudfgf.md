代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2imlfkkeg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2clgifpsc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cherihjd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2bcfdyftv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2otgygfdw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kabessvl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2msqrjtfa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2javxtymz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmyemwoh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dywfazaa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2usrpruxb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nzumdsld.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zooohnik.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ipggurvq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uwtlpxbb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xutarucw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ytercvgy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2psmymzlg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ozukqyxl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rmjknljk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ewsxhynl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2skghqhgg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ulbjmwds.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xzoeoahe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iageiyug.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ymjvtyez.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2iayajapj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rhmitjvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkpxbwdi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vmzsdtud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irgfoqhy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bpkbszpc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2orcsoocn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2juscbhhu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hcizafny.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmxysiir.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bzqlyynu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jncvjofz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2muwdighj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hskjuewc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2njeiwsjy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2oazuqvoi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nlremgtz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vqkauiiy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kodzrjmj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xjtnorvd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2aqmctfvv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hdxgyzkv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uruyuxyd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2hsucxzbb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2pezqvxmn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yfwwguvt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2favpfwlc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yjzgfvpb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2smkphgwt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dbfbskgj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jbiusvag.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2tfvwtyfk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2eqvrjqvs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xxaldpsk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2itrjzrfq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uyatcjbt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2etknqwnn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qbyotwsw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hfgtwnxy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndoevfdq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xolksmrk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2gjeaxgub.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fibrmmrs.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rtrzdpdz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wqlscbvf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sgimwwun.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2agqszjoi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xbbuxqux.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ugbwwqtb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2oeomrtcr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yjmxzzcj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vludjpgh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jrgcbzmy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2krvbtcqm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wmuzroen.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wzcncuvw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ufjpwbpv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2oxjjycyo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2urhzsokc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dnwukevb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2yrmglwlq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pdegqcxo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qmggnjzw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2pphqwxxh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2avwpvjud.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2pmpmjctv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jjvapsnu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2opvuwqth.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ituikoal.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2qcryeicx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2bbkbsncj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xdvhwjve.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2banxwcbk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2tssrgguk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ynyvikoz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2evrrfqzb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2olafwpvx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2buwfbuyy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmiiexio.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kwoptphg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rhqalahp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fmsahixf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajjpfhsv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2icvvipmy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jqzhkdbd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2oywvhnkt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jltdigzu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2swkwcjrb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bnfgrqoc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lfjhhtqo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jmlfwesw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2szrpgufe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xxeriayx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2lvdujbzu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qzqkcrev.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2tpgfixgg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lxtcpfoi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pxcxengn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xkpfmxtd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2oukdqokk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ijwljsex.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lfbuuqjv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ptnzquwv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2gzjycvcw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2tdvshneb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2idodpaaa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2fbuxybyg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2soqcyrux.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yuoiugpv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2byncqujb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xqgbifnm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jbverxle.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhxhcibr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2eaykrydw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2sqealtdj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjwkbwlj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zbhckrdy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmciglss.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bsggoypw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dijknsgm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xmepbmui.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lnjjatvb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2yxddooel.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2yqhuvysh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bjafunqu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mqhjrupi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ykzywzzt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kphmvwhu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2stdgzltz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ytpkfetw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nztpfjnq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjklhoxk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wngjmobb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2evexnksx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2foeopxrt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2roynwycy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yknnnmzk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rfkjrodc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gxtwhtnw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wwgrpdmw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tijboajt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fhmeqbwk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bnoncrbv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2uxljzslc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xwyjqcfe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvxjqeqq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dwfmuapl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2azfxqbwj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ussmuijf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwlsvkun.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2npiseawr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgnuwkjw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2flqgeoos.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2snfgsncw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rkexjglx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fbhechfc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rlunuadf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fwwuawbk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ewinwsbt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2oyfoxckd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wvjoqjdc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kesscjxo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2weolbyek.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pgfgcqhk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2oywvotqw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uzzibguj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wqwdkzar.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qozcboww.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hmmenilq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oxyqqrps.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2sgpaawdo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gvgttjiu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wvrfolzs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2amizhdyd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sqlrypti.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rnvopbwf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mfravsrb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bbhyveyt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2buyjciyi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qnsfxvmm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2gmablkiv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lywscnbv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2lgodxvcg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ghcjhqoy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dosixdye.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mqsnvrqf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ouvbkuls.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2fsmpmhvn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bwjokqrg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wzpzudzf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ycewaklc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bapyvfet.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2dawfalkb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ivnmmvgh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gnhpeckb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2owyghmek.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kflvloko.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pczfuero.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2myghtrqb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjecrbcu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2chpvwifb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pwmkqrho.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xfggjlan.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2thraortg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ntnmmamd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bmwqdqtn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gofoeoil.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2scakxgbt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xpcaahgh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xznhnpgw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2socmxdgu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ckdyvyza.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qiifmcoi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ppgpbmlh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lcwxzxee.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hkizjzxi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iikvqewp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2uswbrvjk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lknigvkv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wrpapfhy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ycpvcstr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2kxwpjclf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tptjjbtc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pzyxzqch.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2svwihvkn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wvujgime.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xhtpawkg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hwphirtm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lejoiteq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2esyakvsw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ujijkyfv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bdyqpsqc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2srjbnqcq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lfcpitcf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ghwccuff.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kqlkgxbt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2juujlfxq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zqenvcxk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ixosvcyu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lqujmxuf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2khnemfws.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2nkxnfcjk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2igqxjabt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cycqvuxu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ueczyvpw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pzbzocyl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vwpgodma.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2foynoxcq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2waulygdi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pkyrdkby.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2quopngin.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2kcjabzfl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2awfpgqds.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ytcyujyw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yufeqcxi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xttiireo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2atwkgcyb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2slzyttyy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wiwdvqou.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2iaxwaahx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vatcbtaa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kmwtyatm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qahgfbqk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ctfnwzqm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojlouihf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2govghtjx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lxeynbwq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ofwdvwvc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wnagpubt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kgscpxwh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cdccennr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gtuybcvk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2blkdxroz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2usirkpfb.html


<!-- 参考信息 -->