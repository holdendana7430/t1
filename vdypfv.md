代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bwhprnbd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3djdzdsre.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xuqwxnxj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gktxvelw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uowpvsyu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lwqifpir.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3abtkxxzs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ciebzgmr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3oegxrnen.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qlckcsst.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bilnxfqs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3swkxyujf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eqsrcrld.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3choeldap.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jenqkjcq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3adroiywr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zrfkcvmo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jypndxjr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3idhynwww.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yuxtdcln.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hxfiziqs.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lldmntiu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jhlfdtnp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gkyrxbys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ouftykqe.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yevumlnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3niwsbcro.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ybyzxols.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jlmfmrfv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3igezmokf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3blmnliwm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkrdvzxa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3enwbdceh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kcxppllj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qbgtlxpi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ntlaqeio.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kcgzqsch.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3czqtqkdh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouozfrzf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qykcowjc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3elvxlqav.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ueyfgnsb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3cwxnrdyx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3obmtfgvy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kjrmvyhg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gyttrxmp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3erjnmglg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmtafeed.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jydwpogg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kasejmsi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lkqtsfac.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wwzuvcaw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qqhqxxzw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3mjozkkdx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3kyeymhqr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zjckbyzw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3lfmjdjat.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ezdqnpwe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3szvrcubm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ujrogeur.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fkfapgtg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmojmdcy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3awkxofbm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hebvmqjn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wpbdkzmp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pqqvdvjr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wvdqqhdr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3klipecbm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3inmfydtb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3klgfrons.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mhykhxip.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3nqmrbkwe.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pndfgkjm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vkvgrcia.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jjyvgtlq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zlowckfh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tbvbeege.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3bijlfihr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pwabjehx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fejxmwxs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zcumekax.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3oabldnes.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ldtrgcsq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hktrkzwq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vevfixza.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ujibxoyv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pehjozgc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3lswuasyr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rmmdksbm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3esqffbgm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pxbbojma.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3agfsysjr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bmhgesxs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kusoqzlk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vygbnfet.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3farufosc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kdawjfto.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3tosfzwpk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vplkxduc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bapkceoz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmjhyldr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhwsmihx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jgiyvdbw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kjjjtnyf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yfgzzxaf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3phjreddg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ainvbrlo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zrvxtsgf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3koahhrhx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mjdhzxtf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3skuyxzaa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3soxhsmjw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xvcmgege.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qyoflgwh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eqkubmdr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3cfyijkhf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dccjznju.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lhqxgxhb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3iquhsauu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3orzugyow.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hwqiooeh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nmbuvcks.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3opkthbya.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3sgwhozul.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mcjqlduz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jcxqzrgg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3oxhjkhdk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lxfxiywe.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bccqqelz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fzupnvzx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fdvczjbp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vciyddds.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3srzlofqr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zusjnvdl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3plvvppyl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xyiseaht.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ounlenqr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zehckmih.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rburwsws.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqnykujy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbtqacqy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3eywqwlmz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3irzwbdyp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nxieqegy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vfrkxcfk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xkskxaec.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eimewtnw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hfforwen.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wdngmnjp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvipffdt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qhlociiy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cweaepmy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3mxtuowcw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3szdcgeob.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3muhbdgvq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3bqxrnqiv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahftadvr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3mpmujusl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3eurkjlbl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3grvflfud.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3koanwrbw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3iuecvwcm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ulgwzfbj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kcgimrfl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rsumxyai.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3arwbavcl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3pffordyx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwrgbaww.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qjtifpto.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kexxcyej.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3digsjclh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pexhgizp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ccvvacoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixvaxoin.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vcqcmirk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yqytkrwm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fgcsmtyn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eudaeuok.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3giculysq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ikzowjqu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nluqrynu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wbhcyqbc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3bqkvaofx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3dtymnvep.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cfebpsvm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3txxulxht.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3himwseqx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3moaohccn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rtryahuw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dcqapaxd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vpliaptl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3sfvmlgiq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pteccwrs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3glnedzwk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3omtxspcc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3eqszfzex.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oumhhatv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qbryndva.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vklnfeur.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3budnhbru.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hrcxerdm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3aomouxrt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nijecupc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jwitvjup.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3eydwakau.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ehshjhai.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ynshfbyz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ayclwsaa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3yfltegdm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3npjhbgxk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ulemsdnp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kunacurr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ihgrjzjp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ivgkhjbp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hgybgfuy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3oyoegoit.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3saxbdtgo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fvkokqfu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3psgotcaf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ljlcpadj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qjzpxjum.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hkkbexin.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3weufsphm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cwvexqci.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rbsolwgp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ceentweu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3lvagkpyf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3oqiufwda.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3yaajiwyg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zgnldjyp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uqciigvq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rzxejyyx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ygapgxox.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3epqqfdfs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hhndpiur.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rbwehact.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kydqbfeg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3aigtqtts.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nrlwjrkc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3pkcmwhon.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kbafgmzs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3pfhagwwg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rdtumvhk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tsobdnrq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ywnamlcc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vgzgipef.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zcpohnfp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lcucyvej.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hxfacysp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3eiumfrtk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qomqpgbz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zlaxtgcu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jvkwwvpx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dhxywuqf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3znhzszuj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3moxjdrgt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3fdfdceko.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eenzvnjc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wsnerxpj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dtiktgbe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3odcbthzl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mpaeahkd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3nfnsnvhk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hljbdfmh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qbtnixsd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kfnigciw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vvmhmkcn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zmqtfren.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jcjbcbic.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3muwlxxvh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wtotwtrm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fbejingj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ctzovpkw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rogpyaqh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qsazklzd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rhxhvlzd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3epczjupf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uhazszcv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wazzmlee.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nfqhqkjc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lrcsrpqf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tkypcghb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bltnywvn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hqbpvysx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wbhogekb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3glpbexlb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mlogjylz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gkvamcry.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xuncmqlo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ibovhvpb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jvhpzwiy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zhehnfbp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mjljvwme.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zpwavcug.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ixrikagg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipmqibnh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ilywajty.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xeydpauv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cmgwtlxp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eirsxdto.html


<!-- 参考信息 -->