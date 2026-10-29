代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gbiykslii.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gvjfqpqnm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gudsuqmri.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gcmzzdjyr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/ghssllmpq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gzekximly.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gqerfyrsj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/grxfnhtdy.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gvmtfsotw.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gxugdufby.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gxlcocuxt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/giyphxtlt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gczyhkytz.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gmpefwttq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/glbftprzt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gezwmfmlb.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gcxwlaang.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gwgagdjmr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gbzftekvg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gxcxvnwmy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gkbsttbmt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gjdfnzaoc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gpowpugby.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gxmxqmjim.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gznakkgxf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gcdxwyvjp.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/geofjdobs.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gzigxfdqn.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gkojlnqmc.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gmeosrbee.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpofhfrqc.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/godgtwlli.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gmklticnv.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/grdcnjthz.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gjkcmnweq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gnqiagexv.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gbwwztdwn.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/glenpoqdl.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/guandyacz.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gesxcmcvz.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gdsmimnuv.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gmxzjseai.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gqxeswxie.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gasfnhxzo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggtglatdn.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gjcwndaiy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzqrtgoef.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gxuksqckq.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gzzjpdfgk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gelvdqcka.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gpshipxjv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzaakomho.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gghucsnad.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gppaqukop.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/ggjmvjqcr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gcayvspct.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gyaymccdt.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gbmnhhfje.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/guqnkybom.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gdgdtsckz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gdjusoiyo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gxbjazins.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gfvscijop.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gnfonzwqz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gjllgqdgt.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gdlgrccgx.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/guaoxzesj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gyqazccsf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/grhwyajyk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gqizonloo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gklwcnyez.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gpmmvlmhk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gldeolbrt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/grcloyjqp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/grgwltovz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/ghpqkvyyx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gibeqobfm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxduucbcb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gqblejecu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gqwsencoc.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gcqyltytg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gdmrdnsrp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/golxuhtqz.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gkgykgkln.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gwkgdtkdx.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gydlnclvu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gxppfcynj.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gvnrwlssd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gkajincgo.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gfdnxtlmk.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gfviqwlkz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gyjoiebou.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gskjlmcfk.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gnisbvhsg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gtrsopova.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gkzpcjtjw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gcxeedpvp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gfhbywidt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gdstssyvz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gqdvthire.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gymfydcro.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gfiplbcmq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gridssqec.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gnarqrvzz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gugdivqrc.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/ggqzubcay.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gpbbtymjm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gyvatjhau.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gnsusmqkk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gahdzfndw.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gfzdrvuov.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gmovqrgkd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/grfrabppp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/grtxmljfv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gxkmcfvij.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gwhrftoxm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gwrkksusi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gtlitcyhd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gxxyltxav.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gygxogghb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/giufheord.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/glsqckezs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/girrgsjol.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gohojiuoy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gukqwbpce.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjcydlsg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gxenxudzl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gczjshwpc.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gwuhmykjv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/geogookuo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gkjgfdquh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gbvkolnbw.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gwgyqgyqh.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gwknjqunq.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gjcrpqoww.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/grazafvhp.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gnrpmpgbz.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/goflehbqt.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gacdonmmt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gddgpspnd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/glzygqusx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/guizhilnn.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gzcgbhbkz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/ghbggmpxy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gsrsacqqh.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gbnfeppjo.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gcbtvmaul.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gbwlcwfpo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/ghslgfovu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gbxpjqgyy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gjtpefnpj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gczflaqfd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gfpcmkhaf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gzuhtislw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gpldgnqtt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gmpmniazq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gqdsfbjsh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gntzetxui.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/grrnrwpkb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/grsvwhloj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gihczzxhk.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gaubxgqaz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gbsnugxuk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gxixerezj.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/ghaamlcve.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gjmldzhqg.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gushjtmgi.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gxgqngehh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gpbuablgu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gwidgrvcy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/ghfjwkaip.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gvdxnyvsd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gnvfkrmtg.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gaghmgdpc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gfnoomdcb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gmbebdcqq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gkpzstrsr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gnrszobsi.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/glbynagkb.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gsxxrwrtd.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gfucvwgtc.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gpdhpfiqa.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gbpqvczrt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gdjwbrwlz.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gzhnfxqgv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gwocztunp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/glopeejld.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gqixiwpwr.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gnxeoogoc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gwhmwkjds.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gmyrkvdti.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcrdjnwau.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gfyjonyfk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtwruofwd.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gjkwtguke.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gkbryvewz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/ggmlucggn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gzllsssjb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gvuoxqmpq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/glrkyjezg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gvtfytmuw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gqiijfwsf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gqehwnjxf.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/goukqnzjl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gseirehkg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gmwqqmzrp.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gdkjbdbfd.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gnhrptidk.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gznejecdg.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gdkflapke.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gqomokxzx.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gaxwatoqh.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/geikigbxc.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gezyqxmtx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gtyfzfawp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gkmokbhyw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/grjdpacaq.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gnrxqciwp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gogtvqbhb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gzpnboipq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gbjwdqrdw.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gjkayufhq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gudaqfefs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvzvpjbcx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gobhmmhgd.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gofuglfln.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzzkhqokt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/ghtebapti.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gmclcumvz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gehchgamb.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gshiwzoqe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gtxlaedge.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gzophqqem.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gtwewxoen.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/godxppwgz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gixokhysg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/grtrmotar.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gngrloqbt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gwxtlpmte.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gmeeojvpd.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gitdeukoh.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gluhvcqpf.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gbjsxoipx.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gjtsrndyt.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gxadkuvlj.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/ggfhmfcum.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gaguqncrp.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gfqhekfrz.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/geszssuiq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gdjuqthfe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gizqfxizl.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gtqrbmary.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gaznzcwfw.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gkincjmaj.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gcneqsaoe.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gzxlneqyu.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gtfmskdev.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/ggpmmlbvo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gizxaidzh.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/guobgpucp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gvpwkecxv.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gqoypxdoq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gifgfnnjz.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/geyanrnmd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gngexhepn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gkakgydww.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gcyxvfouh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gnyfqdzog.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcwjqgmca.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gfisaowsm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gtwpswmpf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/glwqrcjtx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gmoynseev.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gckwtvmvf.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gpdsncegc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gvhiiuwep.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gjbegdfrv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gvltspuhq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gvtguxyvn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gxecwedzn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gerxnqefl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gwoctqffl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gfuqtvyjg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gomlremad.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gewoulawr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gixejwzgn.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gbozgswgf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/guosxjytw.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gxxcbtkko.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gyfwdencv.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gfysgmajb.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/giibaxttc.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gdddopfwk.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gsiefwwmo.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gxndzuler.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gfpcgytdo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/guyterniz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gquefijmr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gfzbrqjro.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gfgorrpxf.sHtML


<!-- 参考信息 -->