代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cmlpvbeu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gzncprmf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lafnbswy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2aywbgand.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nfcxhtcq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2flfypmfb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zcxymxas.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrdlzrb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykekleqj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jlpvlnfo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2gwgykitr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2sakmrljm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cqqgnnzi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lgfwbvdh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yizwzcqt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2uudbungl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmsspju.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eapephjf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dyrqelxn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wdgguhou.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlagpxlr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aifcfxdu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2edmjhcgm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jkawbdnx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ywoebacs.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qvozsmda.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pgasanzf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jwxvnuxv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jrcrnjqs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ewkmgbhu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oypuwlrf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2quxcvuxb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vksuaoyx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mjmcxlky.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qoxfkldy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ljlexnee.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uwwrdhsj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2koehcjjk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2lkzdwqll.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kplvqjys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxipruiy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rdyrhidu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbijayeb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rfqgtpex.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lfbmamhu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kzlqivit.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lnqffvgu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jzfqiofx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fadlhmar.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fgeuzppf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lznovjzg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2udzrlnzt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2uvcksgmm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qlrhnrcm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2msilbrzc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tffdssfi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pkdgxtok.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jgmafckx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2sorvxigu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2byllkism.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2mhasmrvw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2eivizgxd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2dlasjosj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2agjteesg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zngxkiqc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yyzdbfcw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2aljzfbnz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bfpjnvlw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2wigjtvxq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ghjqghew.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zhqeauok.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2vplbluny.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2frtcbeun.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xufeavpy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ijsotsbh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2dezdtvux.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2svhltspu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uivrbgmc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbqjaxw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2uaxpolum.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ndynwuzu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ppeuylxi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dkvkxzyg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2axjuhwrq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2afhaunas.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tvkbnabj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tipbotib.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gqkrdcye.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vcanokle.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2lmpweuwf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2pmwpnoym.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kuwakpgk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hyykkrvq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lcqbmjgp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qvcwfvcz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nwmxhgyt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tyopygek.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wmumyrpn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2thyigaed.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2weatwmne.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2tssxvxbl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wbrrzjva.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zdawmxgz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qhbkgroo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kloemctb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2klwmzobv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2uwlmfavs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gzvufnsd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvllxtxs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqwsfmke.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vmtfbasy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rreghvyr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2cvsnxyog.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2quieylnw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lphumpzd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2zbywjlho.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ogbuhafu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2abrbdttw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ulzwesoe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xxlcaotg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tzmjallq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hfoojyjh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vdrjyzto.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wrhvijbu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cueybihj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ptbwqzgo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vgnpbxzb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2obntftsn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wdpgriay.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rrymhrbo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dnirujsf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qmvpfwiw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jkbtyqey.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2uiyesbyq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dagqjrfu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xccvbgra.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tsqlsqao.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lhnekbqa.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ncblzztt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kylpikng.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dwbgjjvj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xamtpokv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hgqgsfxl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2dermhadt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2vsepmkbl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vznpuxtl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wpqlcyak.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ebjslvaq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xlizukfu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nyzbwkqp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gpjdporf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2btwqfziu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jeahyqma.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzrpstja.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nsdysmgu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpsjrikb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vazvfbak.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2zhrxkcho.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vkpwndbn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yheezbbu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ipjjlvze.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ghoalffv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2umqrdwjj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tkrdeyyp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2sdgsywnt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2flgmvloj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2pjzlzfen.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2glqmytum.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2epfmcsfd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ehwtxyvb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2enpsbljm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mhmuzkyh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ldugosah.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hfuzbhlt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2txtzdteu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2btdpgbir.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ptbpavcz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vjmjjwhv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2aqiiimut.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vsuywdek.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2omacpgae.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jxakiuvx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zriljpcu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2olbojqvv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ocqxetnj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lgvzutjo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zejtsfke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhytcmqe.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dxkskfsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywbcympj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bwmugqns.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ssfzmgod.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ahgmjtxa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iuijjatu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vlzkvdpp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2keoettfd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2modcyypl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2uqdpwngo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qrixxnbk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ilguashg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qmubtnyl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fbxqxyqq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gnewplvu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmqzrprq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xrfrexfk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bqlnncqs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2sycrjpnm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yusezcze.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ilnqmvmd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vrrmbmwk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jbndhdtp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2nmpjowur.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ovumbmzu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uyaspeyc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2otntqwqt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qtnynfjb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lppdpldq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2efuhrlqd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bwdofvge.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mtyktuth.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rpkksypj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2toucgsbj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2nttwwhtm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nhxkyqwn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpsoolt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hfjtntgz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2eckdhpcq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ussgluvn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bejmmari.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yeiowzmk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2svgqtidy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tqjouzez.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rgsowmkz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sraottpm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dsfqgowg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tqccmraq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkuuyjxw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kbtxmpkr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lctscnrr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jqfyubot.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zjsyqlbl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qyxdkumu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ohudinox.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2hwldqqrl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2hxhjiqtt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2inlmegzx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ocxtrgrz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2musvdbhg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kwbbjcjm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zdktkelc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xrnqsqar.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ebqsxvzh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aaplosqb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fllijion.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2oovjzlyq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kxflwwje.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ljpciusb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zpmvolce.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ozvtlvts.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ualhdgoc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2klbglgkf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2prfnqsiv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2xhqddylp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2shjorpsf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lpyxilki.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2nvlayfsw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hlmzbgwi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2cojpvzaf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nbnohfam.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ciblzqpw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dnushwud.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2tsgubjzq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nsyofgau.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uqgpnpnf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qmuipdnt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2edlxwhrn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2dpqmoayr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2yahdellk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xsdtovtg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2bpwofmxz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2yfbauhhi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2btsvagqc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qzvgpyra.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2avyrskfr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2wzexiylk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xasfvbhv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twcheaqc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2phegmvpm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jpaooauc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ddssyfgl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ndixyuth.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qjwxbtcy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bqiaapom.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2guksnxip.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ctocizpa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axtvcfij.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zeabaduw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tbabawbz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ncstczkz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ijpokjwg.html


<!-- 参考信息 -->