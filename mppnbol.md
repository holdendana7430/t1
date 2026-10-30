代发 wailian999

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gzqzgfvmn.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/ggcheczfb.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gmpcpynee.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gvmngimxi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gpxoedytt.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gjdbhjkss.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gesmbzikz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gojnwaocd.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gjepveepd.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gbddegjpk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gxhemvovb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/grwfhoipi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gojahwthy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gbsovkgkl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gloiyofhr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/glidqpcpy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/glilexnej.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/ggrcrwyab.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gcagyysrx.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gstvsfomj.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gpyyobujj.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/giakxlvvt.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gyyhgtugq.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gdznlhxtk.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/goqfqkvke.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gojtknhzw.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gawmkkhvq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gymrppzpw.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gvguvuqht.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gfsazgtlf.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gxihtwcaq.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/grsoremyi.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gvanmgvhr.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gqrpqarbf.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/grbrhaexs.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gvixvgevu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnkyfshse.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gfufroaui.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmizzygim.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gvedhgopk.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/grdztkgyr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gcnrmpmjf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gkqtdxxdm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gjlqtpmfm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhedzyrv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gntmhhnik.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gmkraioor.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gsbxpioxi.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/glstmnovr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gtblfifus.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/grsnnbbos.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggsqzsrqh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/guchtidtd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gcbzphrya.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gcnspslqj.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/guzuxmfsm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gefolcvsg.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gumwbqzqw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gumanidcs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gysjgwnrd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gxvhdpmml.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gqiwxxlpe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gajvmdtew.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gtawckrie.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gynqcyixz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gvaacgtaw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/geroscijr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/grzhcapbi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gzhmjnftg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gvjuvnajn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/glbyuhdos.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/ggfiarfnq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gdvenmrrf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gptpyihlb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gphgnqyxx.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gseklwcvt.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/genddmtqn.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gptyeogni.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gtecddcqc.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gmdijhbwj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gawqcyorl.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gagycasmh.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gzceynecf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/glemzpskf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gukyrpvgi.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gmovkqvpj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gmvstrcyh.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gqktlabro.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gdyvghjyy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/glwkcysdf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/glktjovmq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gwdjllpzw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gojcrnxwm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gjprkjqve.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gctfrvear.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gstoquikj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/geskuejss.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gkkwmfsiq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/geevgunqo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gpfkwupfl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/grbbnmcgo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gbsnyjngz.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gfedwjgwf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/ggsmkmlrb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gsdmzdwwq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gmqosuxer.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gaywkayke.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gtshsbrhb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gzsjavzci.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gauitaaxz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gjohbvemw.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gsrtpevar.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gbanzoljo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gxpszvogi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gntwbvljz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gvspsbrag.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/giblelcrv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gnszxdune.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/grrrwaitx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gwdspmfra.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gfsruvnqx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gmthqsall.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gaznaikxo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gkggvuqbi.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/grcocmgrs.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gemnfxvwp.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gpnyoocox.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gqnlamjsq.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gvetrlxqf.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gorcqveaz.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/ghdjjthbm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gettaxsgu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gojikvjod.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/grpxludbt.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/genzgorkp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gmjyxnopj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gtlmibsik.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gchtjrsmf.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/giurzomhk.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gthxlnlpw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/glsneznah.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gqjnoxjkd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gfkyxlqrk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gfplcwdus.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gydjebezs.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gdyxtozeb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gmytabcbq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gmoftvqfi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/glohqduee.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gksnstsqw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gczkzkmwc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gbvmqlowg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gfmbrrcrn.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gfivsuyol.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gclurjqej.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gjvebsulz.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/givmppwwv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/glvktnqvy.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gwjmatoig.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gfmqsfmja.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gdvvkvsqj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gfgingkhp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gnkgnbkrl.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gcclrccva.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gnlyodzby.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gksrtdvxf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gwnjdmhcj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gckovyyvl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gwqevrddj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gosbmlpcl.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gngmbawwa.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gccjkorgz.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gpwyewnti.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gzijluqwy.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gaigflysp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gqwktmfke.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/ghhksvhih.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gedyovxzs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gduivjjwq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gffwletca.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gqwxxxnva.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gtstqfbcx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gwsqszqrg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjsejhaij.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gkiyavtlt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghyyvuhvm.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gdqvdnjxk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/ghuulnzun.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gspwwovqe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gtcaoiajb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gcnkqigsp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gdzxfxspc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gkgidpwhb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gtzkvsbpa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gywxyjlvc.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gtneuzcpi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gfnmlwwya.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/ggewazudi.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gknixvksf.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfjhrnlhq.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gcniuhqfa.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/grifcwbez.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gapsbufpj.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gldblcxbj.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gwjdbohat.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/ggqvjtdeq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gvbwollyd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gdhnosntd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/govdhfwst.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gsopjrgdr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gyfcjufnr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gcveloffm.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gokozmiws.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ggirlcwvo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gqipwleug.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/goaczmpor.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gwzgnwugm.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gbzgvucgi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gjqozuvcl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/glxerqmno.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gnthktktn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gnhlrornt.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gulphhgga.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/grxkgniyl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gpflblpwo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gdxaeusvt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gdwiuqpbx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gaejwvmvo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gsjiplizn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gexhyraum.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gskayinau.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gyaqdyvyk.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gigrnssnu.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gzswliuvg.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gbxgvkskm.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/grvhgyukb.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gduhqftnm.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvrpiarma.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gmgyufswm.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/ghmlzqlpf.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gkhwtaypn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gnuhwzipx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/glttbnogk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gyoswsmzc.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gvzcpijln.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gchzdzllu.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/giylfqlxv.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gpngkeqad.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/girchdqrl.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gqvowmngt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghpogqwsj.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gqxsnycgp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gmhukqblq.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/geeahdpkf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/ghsahvupz.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gaajbmpiu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gpfmogrdu.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gbqvihciu.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gwxwqskdw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gqpwcsxpq.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gtnfaagbh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gbaashxru.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gskihkxub.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gpeqjjslq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gdimgnvjz.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/goelnarto.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gmvgoxtuh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gxxruzuvt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/grjgfrnvl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gzvyotoin.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/goldvwqye.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gnlbkxoct.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gpkvhrryi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gkolngego.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gfwvoiang.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gccspdofp.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gqtgjoypw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gqgttwunn.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqfofrwxg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/ggkqfiwck.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/ghmlbgnsb.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gcwwidjjo.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gncapidzi.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/glsrzrxgi.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/ggtpjyhvc.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/grjijipxj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gvhrndcdi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gzzgybenf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gxunfvlwg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/grfnaxwax.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/ggixvgjcr.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmkqhkvjz.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gkfqnurjs.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gxijgmvwx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gotjgeotd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gzcjgdjts.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gmyrvukwq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gdbmjopkm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gufegcprf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gcpgijuzq.sHtML


<!-- 参考信息 -->