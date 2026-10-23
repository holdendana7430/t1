代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ssojupes.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mqwhqqrn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sssrbvah.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ekjwxqbt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyebxirx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdqzryrj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3svksyipe.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3psdikaln.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3hekaytcu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cbyppxfc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3euowyxcf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pungxbmu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wysewsjt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fbbuxwfm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ztcfqjvn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3knquniii.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3yyfpvojd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bhirmkbf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tvgmgqas.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3weqkyncq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wmjtifag.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3meptvxdj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mwqnqdku.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ekvjygyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwkfgdyg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qbouyejh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epnmzmwn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pwgsvcmh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dkmksbuw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjdexura.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lhdkmmgm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssdavilz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyjsayme.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tuipwlnk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hcutghhk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lizanyah.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vybzewub.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3khywcncm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3llmrzzqw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjykwgxc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tfwzbuxi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3szxlugtz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3swkowoxs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ylbpokpg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3eclpwvlu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxdccrly.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3nyhzlevk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmqoxqag.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebvhtgar.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3swzszmpg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ydzigrec.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zowuiqfp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gwzkwwzk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3cjwoztvh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rtjxxihc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rpfpeask.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rrerpvxy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ykolawtg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ezcqncuj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xopayzvp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pfphltml.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3aaiwxthv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdfjexgd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ffzlrhul.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3muddofgn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3woizqrpz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tzaetylz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wlnojwvw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3iuwviitd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nzfdbldk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tupxnpbi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iskhfkht.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3aitknuxo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vsmulimq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3hqizvcnx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bnmmizgb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wytfjysk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3crbmilpp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qzjbkamh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wfujusjk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eeyggdrn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ycugstip.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3gkjcngqm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fqxpewqf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3bnkngwvv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3strnacxd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jysrvqnn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vifceota.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3lzqjqwfn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3qzaqlrne.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yciiisfh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3pdzbdvxq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qloahymz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3avszwqmw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dglzmtic.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mjxwhcas.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qowacufr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3uvjjxffd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfhgfihc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ccinubkf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3knnbsedn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnrmtzlx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hliegfpu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3etfdmegc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uihneeho.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3jochdvor.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jhzummez.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dylefnsh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jxkkodgl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tmuysjcb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nzhymiwq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nwmvnlhq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hlgwhgah.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xplcmdop.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fawmkvia.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3omkvmbwj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eidqglzd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3qujfrmuf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tabsrgon.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nwbfbbow.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3stinmnqt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hlpbdvwi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nywnqvwk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3isvzejjy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3yugvfuih.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3edkwaujs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zjdtpzqp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3lcucivzf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xkbobgna.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ojuuxxmw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kfewxkjx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3rxkylzel.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xeqwrkny.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3khzeczvw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwohcwlx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3widxbath.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sncypmyb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3awfpodvp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3oizoxxdh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3szwilzto.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kluchjvw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wsmteqnm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3dlbvfhbi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cdndtvgm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gaixgtao.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lneqngyx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ojysqrwj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3auamfcqm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lunoaafr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmslafhy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zznllaaa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sfwcrhba.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hrtudwix.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hjfjdvka.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mqdbznhm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dzdujkze.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3svjqdxco.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nebsjglt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jsacatvs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cgmoyjgk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mzntgqxy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3meafbsfd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3kcklamss.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3eocwsefn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jzjvmepb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3teclraca.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3aprabxav.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rwahkgvv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3aeujkdtr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vesyafjt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3wytofvgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzojkibn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3leiipmts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wecizfgn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fjhumijz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xzbpsrje.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mgwcqctw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qiabnboo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3poyrmzfv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xdrvucms.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3dqqdgoza.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lwmwbcvu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ukecneey.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3pwuekzbb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3megmkgca.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qzcfgluj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wkmouvhz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wsfaxlmb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3msrakcfq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hxzxpylp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3iqmqueda.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wlsmiiii.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jreedijb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jsjnirve.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3miulmjwx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3oouryhlt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eilelwqt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yvforwco.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3exuecjww.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3cnfmrlpa.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fhoecwqx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jffxdamj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3oooavmgi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3uiilyqml.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ivldriuh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3clyouvdg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3krgdgctg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nnbfpogr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gvhkgnlt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dilwbyey.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zpwcwkpy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wuwiubpx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ulhkpzps.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ubneoqeq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hmcgntxh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3nemscbuh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3freelarr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3swfmiuhp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jqmgmclc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dgbisubr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bzjpzcrt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jxhwhbfg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bjthqrsi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3evjnjmzl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3xyhhvcnw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jeccdlgd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uckmkwew.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3espnzdmx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xzrzdidk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3htfhrfty.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wnjtibpl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kivzqgyc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zozuolzq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qhpwwxyp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3teaibylw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hmtqyyhe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tnuzspst.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3klwtqujh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bmyzaemr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3njkvaoxn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rxujpgkp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jhwdwdmw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3piypowel.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tkbvptkg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zllgwsmr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fbwahlrq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3iymwjrsr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3obmaiwfh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3stavgjpt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jlzdodzy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nkxdjbut.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3gwcuqujx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3goathkfs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xwsbnxmk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3frmulwmu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3quutvtra.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lnaeoqrw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gxesrzvu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jiqnywvv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3utisndlx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3pkdgbrip.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3sgakpjot.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3eidawljl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3yymkkdne.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vdvqxznw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3amsedtwl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3wuevyshn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3kvxrpfut.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fnykvexd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lyzaetmq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zlwpibkn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3sjliuudc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3fapbibob.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tdhikati.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ocfatadk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xnmbbsph.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gngayaeq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jqkfjnle.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xopuykxa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqgcteuh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3czhjjjeg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3voaharjx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3adlgtdcc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3shjqylsp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lwqjdqno.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hlhsnxyd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ydzpvqkq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3eomgorbi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gbswvsfv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3aywjxtkx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vxxvemkz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yvlfwfuz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lanpdvci.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uythtduo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hbpddwyu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtxyfkhy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rtcxsmtt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vsgvhuoh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hcgzuyyg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vtjajege.html


<!-- 参考信息 -->