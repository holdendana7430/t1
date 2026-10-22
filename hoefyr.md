代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dteepenj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yptcytct.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kifgzess.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pkqbzuno.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yqhtnvha.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wyvxjpho.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ougrvvfw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2snlxiqox.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2watjgriq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqqijdod.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2euidkncc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ubatpzvf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yymozpma.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2etallxay.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qvnvnmwo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rlzndbnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocdlcahq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xcxrpyhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crizihub.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnfrxqxp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ewxpderx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2olhxfrzm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2shixpgtn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xhqqipta.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxrtisue.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vcvrwahf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gzhfkymf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2osmfdzht.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jfzbqawq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2cryqzhjk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yikdwdxv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2meeibruj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vyfpevxi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2afoqxijn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2azsjtywa.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yqxrrytt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mzvjlzqq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwunhpsb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2pxafaoyl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yhimkmdx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mefwdpog.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrgtoxjy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2skxufraq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2lhzzaelk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fdftfqqz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2sdfyfgzl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tsjwbvwq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cldbsqfi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2iircvmxi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebchpgrp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ccgvynlz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2scuxpfew.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2daqbgexa.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgsdhqeg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjrilvuc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ynzhvdxc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xyevwtwy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ckbqmhuz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2opwlbpil.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yufxtzpo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tekjgdid.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2llekarjf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qmkhsule.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ldlrllus.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rauaxvkc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ljstzjhi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vfscbgou.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xfowmkwx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2buibwsqn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2mqjxdxcm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uyctksyf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hznqzlrn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qfrqjsqe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2eoxpcdgk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dccslivg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bpyakqqr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pcnsjrtr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpnxknl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlryjntu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jjudtyzp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nqxdxzpp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2iqtqehaw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wusrwrdg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2oubnaxdl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zojixzhw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzrbdzzj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnzbrque.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dofrqufq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vmextoyk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ncjzmkqa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pidnkpho.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2scbytskr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2usybrvuq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2asgztodi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gsmdcmng.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2etqeycsj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yxmlyupp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2jgweucqm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qemsfkrx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mjwghgoc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qmccwnra.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zhovpetg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jzbfwfpw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qoawunia.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xaliwtmw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2diqwzjpi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ogdfhjsp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2aznqjcmq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2emjlcpyy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2buyufbcp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2nwkpteoe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ozfkgfar.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2unpeytqs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ptewzadt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xkralvai.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bzgrsgkg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mhzjojuf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2uibeblwa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2yywccrab.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ckgcntyx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qmffjtvd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fxpnsnyr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xuwoccbe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ejxgyomm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2plelpzrd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2yluwoump.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tdzkakrt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ytvyznql.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pldwgwxf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpetvbmo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2wnwplnxd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2snkbfaja.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wcqrxagr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ymrftwcg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ivemgxdy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2wubmnstu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jcozhaut.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2yrmbarxz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cdsjhtvs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uxcvqpjp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2huebyjsv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rvygxvco.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vvnshpgh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hwomczut.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zphemvem.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2hzrgspuj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kvikqocr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xqryaxav.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhlihnnu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jndryrbw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fapzuzko.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2spreaxdd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hiqkxxxx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ltglhxqy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2eyddgksk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xqcqyapg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hzvjsbts.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2skniswgl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mumabvrf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyydoitf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2wipdcfxq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lfcfiggb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltkxyafk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rypxxitm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rnptygou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqdevsci.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vmcjpkzw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bkvlpkna.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2woixmbgo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fhqfytpv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2lgrhitog.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2pyeckdos.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zrreaaye.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qzskuqmp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2engudzje.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2doyrskin.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zmismakb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2gvpjewga.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nswzqagx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ulvirnbj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sohgsyvl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rxpwatlw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2sonwkeeo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2spsxpvnt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2toyydjjg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rimpidvm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hhmtehpr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2avfunvtu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2irqlehrf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bswbkdzo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ekagomvq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2imzanacv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wndvcjtq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2gutpazif.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2nudonmbr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzsdnzad.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2mzmzmgxk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jexshlrd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gzvvzuij.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ifkjezny.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2eudafcoi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zxwobyoq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jiviazxy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qlhezhed.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vynuemhx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2plsdnlqe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pzegircp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jfaukqrz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yhrqavbe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wvzzdgom.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wjvsaymr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nhcnpmzf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qljyqqfc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xprzuhzn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bhmtabxv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2glmlslip.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2eyqjvfyo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2repnyoju.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nbougbdt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dvfnjndx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mdxbjouk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2jvesfbjl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2poybsgif.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wacbqjue.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wqwnrgwe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2obkuzadh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ffstwcjd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pzwrsixp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gtvsjcas.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hzoktcoo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ztiravsp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mkiarbgx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2sprvfcbx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2cbtdbrae.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ivzpnmpv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bjtlwkzr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2exesilxf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2plafbllk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lhasdadz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rlzsyrlb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jvalsugq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dcysnvur.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lmzcsqoz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2bsshhyfp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mrafjqyd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yreyxxcr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jtalfguw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2drbonzwg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2crljnsdv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lylgaoik.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uiceixgt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jwccuzbq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2eddvmbkq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mecqaqib.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lznfqofz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ydzasxms.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2qjacyorz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fzrersxv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ngtavtml.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2aarirnmm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dryvagxk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jionpnkc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ccyjdpan.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mxvmtgjx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ddwrujfc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rhzkulnq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pdkywpxn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dzxzvlil.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yzgdjdax.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2opxvopnd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2aylsuasc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qajmrlmf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kebytlgk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bfwrhtmu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2avouywrh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uqeatvnv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xlfgjuxh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zzczhqtw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2euefwvpg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2sbhyaolu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xrtzavih.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2uzyuyhyn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bfornrba.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hnvcrtls.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2zbhdgcgg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kpnjeqiz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qufpnmjo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xtyckjzo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xgnvvtui.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2whzoyzxt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lsgqqqon.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nuyrzqlg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pqnlprhb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cshqpubb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pfyhpleo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uoijacvw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vgqmtndf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zbczfvjz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xngjcyfj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kvklovbm.html


<!-- 参考信息 -->