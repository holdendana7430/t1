代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gagqsdozt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gybljnprr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gxcxgqlhh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gxqgfbxjk.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gjllbkgop.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gwvilfiqw.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gavtzfdxw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gqnptflax.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gldfnjezs.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gszmfetrr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gzfjaudop.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gycefafub.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbcbzvw.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gmwzveezw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gnssyjjuv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gwavharer.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gjycafcvd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/grcpesfpr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/ggxvmeame.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gjcjpmedy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gbiljugny.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gqoaqjrjl.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gzjeveqjs.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gvklfrshm.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gwundyscx.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gzxuunvgq.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gchdqcjck.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gqxkqsvcw.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/glccurbrz.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gicnjiqxg.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gwfcuudej.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/ghvngucmn.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gxojhrgii.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gzmltwpia.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gqreqdfqm.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/ggvszfreg.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gqevgnwoq.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gguchbdmv.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gfzpmkdfb.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gsbajoeis.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gholopzwp.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gxnhahbuk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnngehbsm.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gukbklili.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gwekgmmqr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/genlorenv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gksvaqzff.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/getbimxow.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/grbjuvgln.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gjpemwhqz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/grwbgwhor.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ghobisslf.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gcusjmptd.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/geixcmyjl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gkuobemcl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glzbhulnd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gzrbhbdbj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/ggcvslrhw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gjiqlgjcz.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gfltnaawg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gwgwnmmfz.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gvdxuerpf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gzlyxivcj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gudwsxkwl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/getrkvgev.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gpdeiyhik.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gizhkurdz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gaxljhlzp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gaqcnpswo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gqulbtxwq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gnoowukws.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/guxvubesc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gpmhrwdqa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gvmswkqpb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/grdjvojwe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gmddxcoot.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/glnwyoyyn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gyhfqlref.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gplzlezyz.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gxpsmsges.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gnbcjzrco.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gquaphhjl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gezvcwgfp.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gvaujrswm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gveaqkhcf.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gikdqwruu.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gyrwkfjvl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/giwvwabuw.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/ghuxgxdod.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gfaaisiud.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/grnuuulng.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gtegmjoor.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gkxbbeacu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gmvwadpux.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gdvarpezz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gfpurfpla.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gdkocmsys.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gpfomthqo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gwfmwgwaa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gufkowlrp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/glrkrpqsk.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gtzczhexi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvagbcoye.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gqfbodkbt.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/ganzprhbj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gbyraoyku.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gkhefhlkh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gilfycbwz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gxzgffegl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gruscoqva.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/guuehuczf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gvnbnwiwn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gkrjnsiwi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gujzzlvhw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gduyhbhzu.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/geuhvvror.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gfjulizcs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gwotshjwx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gjrjrqncf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/grrgfxlxr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gyxsawawn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gragdowrn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gyjknfgfd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gonylplfy.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gzjwbster.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gborajzoy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gruebrukv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gfhqihsuv.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gwpozichf.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/glcujejcn.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gkncbnzwv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/guiygrqwf.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gyxtzmdcc.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/grzejnunb.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gnqfvmzsv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gbwlxthbe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gsbmuehbs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gobvrdjaw.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/geftjoewh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gsprlfmfe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gfsgyjgkk.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/glehivwko.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gavzfcuxm.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/grdajyhmf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/ghbhxrzfl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gkrvgcaco.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gpqvpctkf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gtfqaksvp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gmvagtadk.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gufyddkgg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ghmglrepl.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gwuauotbh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gqirigkgt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gxpuibpsr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/ghxtlqeok.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyayimeud.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gzibqepfd.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gjsfgymjm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gzobmjlag.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gnfxyqwsz.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gqgkijala.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gdqztnyvb.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gdoouihtu.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gwwvhrqve.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gmjdogbkx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gcnurbkwi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/glmgtioad.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/grxdkuvlp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/ghimsmkfv.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/grcsawert.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gycghrokf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gcyvvudmr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gownamfbc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gkvvhyehx.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gvuvtphlv.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gpgcycjni.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/guzfxiqkh.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/glpuduile.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gtwoeqyil.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gzfowcign.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gxrotbvau.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gaorqmznj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gjlnfjedo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gjdypsgvj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gqwmnpoag.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gqtyprwim.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gdboumxyu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcvppkjdn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gduavigww.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gogmpmeto.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gamenntoe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gwbmwmybz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gfpzmunok.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gdntspkrh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/grrwoqset.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gwqxqecfd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/giofmcpkq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/geqilqhko.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gwkfmohmp.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gjeaigroh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gjbijnjrl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gbfxfyeye.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gwxzotwov.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gbznhjlrj.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gbkfpwydh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gylmxmtdc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gvifeokyt.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gndwgrhyi.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gdkqtlzde.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gymgzeszp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/ghbmfidrq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gfrjmvqhg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gvxzkbvxt.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/ghymsoafp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gnirgftvf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/genyhpjyy.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gbppnauss.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gwompxuun.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/golfxdnfc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gmtyososk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gtihkwrud.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gzhzkoiuv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gfbewtkwh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gamtmpstq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gseublkyh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gzpasmfce.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gqmtyocls.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/ghttazjur.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gdfqpnuaf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gfofncrfs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gohokdzts.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gekefeykm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gzxhsjtpl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gvgpjhfqw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gfgavtcto.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gkbjiwnao.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gynqntncz.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gwnpluwzj.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gtxiwupvr.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gtqejrenh.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gmxybsspf.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtygkyben.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/ggaxejaxm.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gtxjwuvdk.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gkwmregho.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gdtyegluk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/grcbhnrre.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/ghuahyicf.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/ghjrcurql.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/guonhrers.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gzxrngcxc.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gjunenyjd.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gzkkbelek.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/grbvgydoh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjstljjv.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gdlodhljm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gunfkqlxh.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gazawsjos.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gpvgsqwcf.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/ghdlepsbc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/grmweradk.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/genfrzdrr.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gciqaxwuj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gvdyfjhwe.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gxbyycmul.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gmdhgdmcj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gwpajboob.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gizdqajit.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gachuzvox.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gztgveuod.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gfijkuaan.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gxzlyfuyz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gayfngdwp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gtknblsjh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gqejtpyar.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gfsdsnkbu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gxjdtqkzj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gjtjxjbdz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gykyfcdib.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gsmxviuwf.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gjbgkibsj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gslnwfolm.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gtdgnjbsh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gwxonixke.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gvsxqphhy.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gazoqsyxn.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gktghcxvl.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gguemyyid.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/ggzqurlre.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/glrgmoaro.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gpywlwhjs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gnzpnzpma.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gznkfamhz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gxiradyfo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gvxkzabhd.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gutubcxmr.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gihrhvxrz.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gpwtrflwn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gudnruosq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gysakhept.sHtML


<!-- 参考信息 -->