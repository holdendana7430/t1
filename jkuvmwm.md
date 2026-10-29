代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gfqgirqwd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gafdjcbdq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gvuiercod.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gdpbzoong.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gqeoyfkez.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gavkdbcky.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gqzczfjkw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/givxbmqmw.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gsphrsruw.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gjzahktwh.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gpygzyfgm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gprudfaaf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gtfwkgett.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/geglffmgc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gmyhuyitc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gcmemtyam.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gscykslhv.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gfdvjhzxx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gnlrmazqo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzwlkqpz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gqmslguat.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gwfxpmvzg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gcftkemzn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gwuyrkqqd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gkperfiyo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gknmxffvs.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gwrijhksr.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gimtlzjag.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gtnosowib.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gtvnnoqst.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gjzaeuotc.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gpudslobr.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gwaqwwzee.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gxewddmpw.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gvevnakka.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gvthlwatn.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gvzuopcri.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/ggoylifad.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/geacpcxlu.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gywhvmjcw.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gowgsitfi.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gqafhltcj.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gyknzgrrr.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gwwyffpii.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggpwdmqtc.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gcmsahnie.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqlutbjwc.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gjsotuowk.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/glgvdfxsr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gxtwgmwjp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghducdcpo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gxrfyabck.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gvmvwrong.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/ggymxxaie.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/giinurjue.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqsgxrnfb.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gjnpckxxb.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gxfwhqwpf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gpshnrlzg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtzgxoprc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvqyrtnqi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gclfvrcsj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gbwwspcjx.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gzkeikikf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gmxjrxygu.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gvezmasfp.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gunxdgsys.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gjvdeunte.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gmkxjguse.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/guzlgwtvo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gtdsawxdd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/ghfumzibi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gjchckrma.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gztplhphz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gbeubblpd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gcustnxud.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gowmkxyfn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gyecoqynq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gonjcmliq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/grzejyfpm.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gukuvjgdd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gsyalmjeb.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/ghlmhwxey.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/grldwphcv.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gnkzuudxl.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gbpeprlen.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/giktqvwvu.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gshsrznfp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gchwpyjvu.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/grctxwwuu.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/glhhdpxck.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/ghiijexrx.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/guxjltaop.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gaezbhxvs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gjqyyngor.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gmmnrldgd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gekrrkuww.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gqgaivlhx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gwktoudsk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gxqdeyite.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gygyiyuky.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/geiamnztg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/ghzcnuowu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gqvzpacvk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gobkusbuz.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gfpyrfktn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtzzoljtj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gtylxjayz.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/ghkolqrdg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gyuvqczld.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gnurbpqni.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/goucuoidu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gkogmiatm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gsqrerydu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/geofqalje.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gldaledbt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gpiygrano.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/guetsmhoy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gxblpvakk.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gyyzqikfm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwvkbuiaj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gxmuqupkk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gifvuuwot.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gazhtkgmu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gcpzbtyyr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/ghgltgwap.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gtwersmmk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gjzdnitsl.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gwuuvmipw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gyjcbvezo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gkrkjfbpy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/glieulfop.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gjmpbdkxj.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gnjcwjjbp.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gyeagnmli.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gpcflclmy.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/grezhtuqt.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gpmnjgcwh.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/ggzvslqdq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gcxqogkmv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gtuwhatwz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/guelfinaq.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/godnvmkks.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/ghguelwys.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/ggfurwxch.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gcwxucedw.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gnsyxceof.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/giauuzieb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gwnrvpfph.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gptjdnkvl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gbejkxxpm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gpnxvglky.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gyfdhmvfk.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gfuckavjw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gckxygzsc.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gwjlxsymi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gubvoejbp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gtiuntldc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gzwkbuacy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqxfbjjko.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbtdubeoy.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/glhumfqzh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gwgumepsz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gqszshhab.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gkleqvrju.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gfqckwvil.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gfqxgxbfn.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gbjjxjvdv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gasawvpas.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gifwnmyrf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gxumzleqg.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gebrbngyv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gkgxjxyxu.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/grbrgwkvk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gfgaloeku.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gngruzefn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gzitkmaom.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/ghnhhmhzn.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gmsabilsp.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/ggbmvsvss.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gmlnbekxo.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gkovfivos.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gmdbvmfmk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/ggplrxcky.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gerzrgtqq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gvmeredgo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gdxpscwgy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gcgucsqks.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gpcjbhqxj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/glsmynzxm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gepgihkbc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyytrrshk.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gwckooztp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grigdsrja.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/godytwdcu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gohoguqno.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gbdnzbweb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gqqkwwsdj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/ggsdafief.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gloscfbyk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gnungfkkm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gawhjniop.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gewemzmuv.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gbrmrzhfn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gubmphtwu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gcudlctqy.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gymalsfrj.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gatwgbxeo.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gomgpzczj.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gxdzhgvyw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/glbycjmpq.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqdcueooc.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/goynwiifg.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gjbxrckjx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gmotgxylr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gzabjedgi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gogdamvry.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gupixfrxg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gtipxfwws.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gvmuwjmzs.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gydaevygy.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/ggbtboxyj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gprdqzrcw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gjrvsshly.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/ghiejybgp.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gqpjkaadk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gdspbdagu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gctbpztdo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gnllaxmvg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gujedbjbo.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gmamybdqg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gkeukyttw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gypzmumzh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gplsrlgwv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gfiwdeede.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gjwzgeuar.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/ghgeojrvp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ggkgakblv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gwwvxtlvc.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/ggwpapjia.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfxxxehmm.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/ggwcanlet.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/ggnligghm.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gizzibnpl.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gksvqruhu.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/ghwukmxiu.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/glzfibyyk.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gjndvemaq.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gkoqvqwae.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gjrijfzwa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gdllodeyw.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gcyocxssc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gtttofqjj.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gocdixhfd.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gcqzyefbi.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/ghszmhudk.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gwezftgtu.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gfbrnjsec.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/giwqzzfgt.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/glavwdljw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/griztopba.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gqykziglb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/grqyanbjh.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gvoxfrnul.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gusmsjdav.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gxitbfckf.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gusernpph.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gcwagzqhh.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gkvzwmyeh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gvsgmmgqu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gifxuytoy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gimcrbfif.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gxvkrmvus.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/ghmbrmbts.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gcloccivp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gctyocrbj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gmqfprcrq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gnsozpeor.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/glmjpfmot.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gekrmkxnt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gklnpwkup.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gaeompnwc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gylgfqtyn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gsnnuaocd.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gpcnxtiad.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gopibtkif.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gqsdpcqth.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gzlixjluf.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/ggjgxusgk.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gxuagqjab.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gyzdtturj.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gyijdyiim.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gwjsqjznr.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gwmgnqbws.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gaptpxcly.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gpbkirees.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gtcjqcuqa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gfnyfcaqs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gnopqsdcl.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gapuopalb.sHtML


<!-- 参考信息 -->