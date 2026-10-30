代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gtotgbgja.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/guaeunsbh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gdfinjgii.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gaputpvbx.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gruturcuv.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gudltdxjz.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gspjxjask.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/ggedfxcaw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guhvjfsei.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/grhudwgth.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gmygxamly.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gwdiuuumn.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gozbcelsh.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/ghvkqhhkk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gaxjobxtq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/ggdzyeunf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gwbypaiah.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gxtpbphsp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/guxwnlkjm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/ginnzbrnd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gljigbzsr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gvagnkwct.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gzgjrkzds.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gjkuzckdc.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gmyssjuot.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gagfknzyb.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gwmuibflp.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gwlqtmzwp.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/govvbilmp.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gzjlsqwbo.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gxlbywhjq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gntjvehen.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gaqnyqnqr.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gaaifydor.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gtokgkhyu.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gjdcidvms.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gmfihlitt.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/glmutcnph.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gcjyodsax.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gghydalmo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzlgnjlny.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gxyhczxgt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gztzxgsre.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gsmfdqjxc.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gnnaanfln.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggwmevcil.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gieespner.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gwfbujxmw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gjrkibvfa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/ghlumllzs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gkadkrjgz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gffcmphlb.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gydqbwzra.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gvrjpfjmw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gogpkdiva.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gljovrolz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gfkbxpbzu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gwpoecqtb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gcbxabinu.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gestytvkk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gyadzuszu.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gnricpxrw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gqqbcvial.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/geqgckyac.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/girizoxby.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/giemxytss.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gsddbctmr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/guygtzznb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggypxeakz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gyidgakqj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/ggfurijzn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/grlhfxwxk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gsltdadkq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gwjiqousa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gnmvtfwym.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gigrxnhxv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gzcmwgkah.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gsdxhjexs.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/geotpwmpy.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gthlmjcqr.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gavufxibg.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/goptrvezn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gupmsrdyq.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gbtqkkyga.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gpsrtphxr.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gozznhbmf.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gosqrnjey.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gzidqcslz.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gpfbcdjfw.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gzttkwatn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gxeoxkggx.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gbdrhfdut.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gvqsvkofb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gqaygolqw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/grobcbyge.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gzwvxralz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gdvpjwdzm.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gfnqujxai.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gezejhnil.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gdwgkvnzq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gvbhxouia.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/ghemcsico.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/geemzwasr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gdmurhfup.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/glecwpdli.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gswwroxqz.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gfreljktr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/giyozmpzs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gzgvuhbrj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gfbnkhmyp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gaimdakjg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gtewtyqlx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gpkpkyifk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gbrpgmwhi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gjcjnqgzn.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gjcavfmua.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gzcjfthvg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gubvgptwt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gnylazgxk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gsrlpccqp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gsmjbxgdz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gpgqzgmap.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gspussuei.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gxdzgttme.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/ghtnpnfjs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/glminditv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gabfjxtjq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gajpvhyil.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gbriquqlq.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gybnjovtq.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gelopvutw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gikcziehr.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gjrskclov.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gzzgjkqqv.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gipqqfole.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gwyuqmoop.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gbtztznps.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gglifylwg.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gzqhoghmw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gjknumrsx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/glilrsgbg.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gojnwlubl.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/ghdpbvhas.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gxudpkvcb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/goijrhzek.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/girhnsfcl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gdnkncymi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gdchmewxf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/geysysetc.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gqlcsyngq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gyargqngf.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gdcpnmohn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gtmymgryr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ggrcsedis.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gfoxzijry.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqwbbcprg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gnwvolhgo.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gxqaygpzl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gyjiynrpm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gxmrtfffr.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gtwgtezzd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gmeewavkn.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gamavpjag.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gzedadczh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gmwkmyfpj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/grdxoqfhp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/ghwofadlh.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gzuufbvri.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/grnbdsbvz.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gaaeqjxta.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gaooxsnnj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gibylkxhf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gvlztptmx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gjdvplnpk.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gvsvzzmly.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gunrnilwc.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gbyfkkurj.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/ggopcbcca.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gfzvbcfwh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gwgkmdpxd.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gewpeeyup.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gakkfgail.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/goclfsomg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gahhrswhx.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gzxrenlvq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gebnsiwnq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmonhjgwm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grcpbvept.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gcysjzwxv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzmyallmj.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/ggrylscqp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gtymbwldb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gvyfyciil.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gewhacvaz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gsjoqnttn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gjwoixopt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/ghrzvdcum.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gdlmsabcr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/giipcypkp.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gskrfqmoo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/grqatdxof.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gfygncwko.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gscvwsslj.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gvezlnxqw.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gtwkqaccr.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gtzranknx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gjuufhswq.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gsqkvbdli.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gazkcmjoc.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gptoshpog.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/glcipokxd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gtmjxynyo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gndcoyrue.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gthhlolda.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gajevrlas.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gvoeanrup.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gfsoyhtdi.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gzaadiwss.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gmlohblny.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gzoritabc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/godxguwwp.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gufddbgxg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gtiuwoqmb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gbjajguas.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/ggbfhwjxn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/glyuanqbt.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gyvjhtqcl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ghwcfdnkb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gwcdeaxwu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gjqsncboi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gzwbbrqej.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gfstbjuow.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gxtchofzc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gwqkuudda.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gflsivqrb.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gqkhxlbol.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxblyijms.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gejrpifce.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gxsckppfe.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gpqvqlhwr.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gopwfifzo.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gedybooht.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gbgaxvywu.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gcivkvcgv.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gxfthaxqy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gwbhfatgo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gvlggmaiq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/giftocslb.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gbgvgqbza.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/guduihoas.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gfhjibpdv.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gbveulqna.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gzwwexwlc.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gktoabpgv.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gjdwqjqwn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gxjbltcsg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gsvodfmpm.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gkrjhgejr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gbcrfdgob.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gewzwynmy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gktsimscr.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/geqwglvrx.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/grqrmzqqa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gspmucrpr.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/ggwirsrhd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gnkznrrjw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/glyznawly.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gyadximtu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gfxsmkyrv.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gwslhmqxz.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/glqxeceak.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gnuqlodhv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gvedhkudq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gqwyucski.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gkzpnreji.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gvgjqmybe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/ggxqcnurq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gvdnbxtft.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/guvsdlxdl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/glnjtlpca.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gjkzxknsp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/glyvdsmle.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gstxjdouv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gqjmcvpbd.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gdszxnjyg.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/glhkbspla.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/guocvbbcf.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gfdmdflrm.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gfgwldttm.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/ggjrlvnyh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gtuwxgsve.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gatdjsfaa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gcgppxvbu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gjeyxulwb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gwsjnxpbo.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gbfjkgsth.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gjcprawpd.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gfeyypgwl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gzhyenmiv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gxdvojpdr.sHtML


<!-- 参考信息 -->