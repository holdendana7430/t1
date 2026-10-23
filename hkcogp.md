代发 wailian999

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3euvlllnq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3khtaebqb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nlkqvzqc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3skgfqpni.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nfcgingo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvlplgvn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ltbkdois.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3frwhupwh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3oxlarwyn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3saqcklbi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ljdeghev.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rnphgxwr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wbilkkmh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hgbsbopv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tfzdbbcg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3efffvwxh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tjjqpvce.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3khxuyswi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uxbscxvo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3bvbwapyl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3sbmtfnlc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3danserpc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cfkkojpp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bikqwxhl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dggivowa.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zktrtsaw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ctyercnu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ojpsjjcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndhswluc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3cdhzsjmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lplpingp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3boqjthlt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pxxlkqsw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsaxcwer.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxeivbox.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jqtptuix.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bblnzwyn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vvfwsalk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3cspubzzu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dliwcpru.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ydbjqluq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3avcofvwj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3efgtkdrk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pehxqnwp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwnzbqeg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ojijzbtv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dtbtcusn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fwnirqef.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wbomujbn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3eteedsfn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3waftmtig.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3zliyhual.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcxohcje.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppsffwcd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ytmbdtvn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xwiujsyn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qxsdluxi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rcnbafye.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qjeydtvt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3lgejloub.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gapdapjo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vkemtcgz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3cswfxfon.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3otldhbjz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ecxfwnfd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fofthyun.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjtzbra.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3jnxxozxs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3msemjwcu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3uwnolbls.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3irhwjvkz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wbwlhzha.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nhrchmqz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hnndxrlc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vatgnddy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zvdojjud.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mhbwjpfo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3imggefgw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3lkzrtoat.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wublgbpb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uljhbsas.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3smsbczhm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mwxnawhk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3racxhnrv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3klceluoe.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fbhtrxif.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3atbxmmzd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tccybjhd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tnaesfsc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3vkswbffh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dtwtbfsn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3uxvjfgwz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fmeeitwn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vctzrvzo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3avnimpuu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dpscfsqt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3smsgdofa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuuutakj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vmrrxgrk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3rdagijxh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3oxaiowvk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3lpukufie.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hujprvfy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bqbbxdog.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qovvfngl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzaupzmu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ehokracl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jbsdkijz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjtpweiz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3idweuqsw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgrmnqri.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ssxpdhtu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lvfkzbcp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3yhwdluew.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hjrhuquu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iuolklcp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fmdkihwx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dngapomw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3neppimoh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ppkpmrgs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oicjlvvi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ufhucajg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3sbsyxzsf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nqmjvpef.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3srtgescd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qwpdxftp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bpjjveci.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vxftlfsy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3yplsihnh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3adicohdd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3armzbcoh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3jvasutrs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mwiinfia.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tmapcese.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mnolpqrn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3guhxvygh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pxzfluad.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3orgeiwut.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdhpchce.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3buzbatkf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zgcfztyi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3prxtbncw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lgrbqext.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qonnersa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3enbpvioo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vnxmxnux.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vadeonsh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3bjxlwgow.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmnannoi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bkkpxwfz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3agljrcku.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qogiuaal.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pyrbftiy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jctnival.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rofgchzr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nkvvaadg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xkxhphfu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jofqatjg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3eiyrubjf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xpcogldg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wzywfsjo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3peacuyoe.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wvpariwr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qclvswoy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3eyfvoqeq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3dqfafoob.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3awgnsldc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hkqiancy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3pbnvokrt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3isvhhbss.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jmbjkwzq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfujumac.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ggcfnkuq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3icuyumaw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3addvqhuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpzuorfn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3azrktnjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iplplesc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yeoznbkq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dpwqoftl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ijjrlcve.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vepuggnb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rvcpcrwg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3hijyndep.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ucrarmdt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3nlthezkn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3cfnmpigv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cerrhiwj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3nweskgee.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3epxjjgfl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vfyecaqg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fffzuafi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rhwopzkt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xbaywglr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3byaifgok.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gchoxmbt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ericnksb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3itizunhb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xnijsrbr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kkyyrsgb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eefuplvq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xpcwgvjy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dfgretnw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vlbjwmvv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uxthobzc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ryjfoexn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lfrryhtz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3onyjgywl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qveuctoh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uqzoazls.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3emtxsyqb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3scihisdj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3josarfji.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yhkfifys.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3iedrqift.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dqucbfeq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cvpwalay.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dkkdhbku.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wnveqpxt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3upcepqlk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ompimhgv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ibtgpwgy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sxeqprhi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cygalamh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jbvauadn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bfkgawrv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uonjhcqx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vdeudcgs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3pqyytwsm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rpmxaiid.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qvincofb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hawwqfyi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ydogqxya.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3moxcjkvw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dmpegfln.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bwxwejtj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ikkfcjnz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wkmuufxx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3uatswlmr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jsnbkebc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3thoinqui.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3wtosszax.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pgtexhxj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lwsllgkf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3asgawqkv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kdnpvhjs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tpkmmopp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cqkuptem.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wxwfwvqd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uupvmrca.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bsdznllj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oivdlcrj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tqwnrtps.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3nosawsoh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gmbqaxqw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3chqsnrxi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmxfctp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bfgklqgs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pgwvtlnb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jhpvgdor.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ehqawgtb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xlobheqy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ntqpriuv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ernksjsp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3moecsbul.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fhcjdzec.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mygmegvm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bhxvjler.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3peuxmpoj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3asjwzxvw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3augntohs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ekbvfjfo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xqaykaux.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bemoulig.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yfawofac.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pnkiqjrm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bnmlibvq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cfbuqrfs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3asssgppc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3puhebvth.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nqgyzwvd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fdnlgjaq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3uujjrjxn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qzocauwp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zrsudtds.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nrreaika.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ucxppbil.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3irfonewi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wmtldzmc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3shudawse.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ewlxxlut.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gerxsxyv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yjauocnx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qspyrqbg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zyrqijqq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fqlikosc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3alovksnw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3keyrnmgu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqicaig.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shvgxiec.html


<!-- 参考信息 -->