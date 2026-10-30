代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/goswrlwgi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/ghepdbaqd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gcroxwtei.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gukqtfsrs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gkpotduwb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gncrhkywf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gopxgacor.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gklbbtpjl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gtpmxcguk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gjporkwvw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/grcvoynfa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gxsnlukqu.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gfhvwjqft.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gkbjnydxq.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gkhclmkrv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gywlzrlta.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/golbncfyj.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gmwtdcjkn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gyphodnbd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gnrqwssvg.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/ghpcpnaeq.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/ghabyxkzg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gsptjnsuk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gxkujvxji.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gznjmfyme.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gbsizzwee.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gigenovlj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gvmkmuhne.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gfpxcmuzw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/geunbafin.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gdpnjzdfx.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gkzhlsqzt.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gkmtppafc.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gzpgdjgos.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/glqthocvy.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gnuirzukj.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gjpbghkuj.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gdcfbkdkm.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/glxmjybtz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gvfyvynzk.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/ghtdthtto.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gwufmzzhr.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gyzxnrerb.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gfcubrlig.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/graixigoq.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gohfbfnym.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gvponforw.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gyjeaxedu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gasgdxtda.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gakkevglp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gimldimiv.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gcswsctlm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gmgapdadc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gekoohany.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gbhnqmqxb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ggfttgeob.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gzstjhdsb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gpsifrfii.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gplnkgwkn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gruphpwas.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gutqjcxtb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gtnibpvfn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/goiyicpjx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gwlmwpuyd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gitamfzwk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gctetdqqp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/ggynzvcji.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gefcksekn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gsllupmbn.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gxvskcgbs.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gjznjengd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gpjstvrfe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gmoyvxglf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/grschkphj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gjgwpglcv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gaxfugcji.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/glpzxniyq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gdbewligd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gcoidliet.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/grrewgpse.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gitrxhhdk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gvtwjfeno.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gzqkknnfe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gtaujzoyj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gijnvulls.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gvnhtvkvi.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gmunodama.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gcoarkymd.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gxfkkkdlm.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gftmmlira.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/ghqxnmysu.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gctrnysme.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/ggbhzdbua.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gjjzjxytb.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gtrzyupdu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gdklyufpj.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gpqddledd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gdynpuloc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/ggcblyxlq.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gxucwbras.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/ghnqpokfs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gwqijzvht.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gchmuqmqp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/grdwlgjcc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gsckyibyv.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gdzmvxawn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gjahblwrn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggsogukzk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gucrrckaw.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gksvlwgxm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gysblbfpk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gfbxikmlq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/goshduxun.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/ggndluosn.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/goqkhtuhj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gavbiggse.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gznlsvvrf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gbbwhfzty.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gralrkibw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gpylfjsex.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gvlpjpytd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gibvxxjhz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gguzlppzu.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/ggbyxxzkl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gilrhqdds.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gfbvotlqd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gnmytnzdo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/geczhbbqr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gvhlaunqy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gzbsjsply.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gvbeazzwc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gmqbiubhr.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gnksnatwy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gfmkpeaor.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gqkvufjqd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gcgyjlvqf.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gxniqdvfl.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gcqlxkokk.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gjohlpjil.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gwddkyrxd.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gkzuxuaem.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gbwgeqpla.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gzjokasaa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gaalsbmvd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gimmnudqq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/giddhysvv.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gnjzsxtxp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/ggxgoxooa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gttzyfpea.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gekaowxuo.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gyiaxhuvs.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gaxzszgbt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gxpuoptpi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gvwtrktpb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gludxkbie.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gizchrqvo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gcfwxgfbv.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gchiqefdt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gkcegccbx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gekuxxmjp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gevbvgkqd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gwvjlpmut.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/ghtybexmr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gqektsrnq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/guboiwyvn.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/ghylhxtmy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gddzuorrw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gyyzumcen.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gkwydmhxk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gnbyjrrit.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gpwmxcxbm.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gtrgfuomd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gzxbwcotu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gppdxhygp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gvvgswpke.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gkvezvyal.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gzjeqceuz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gdburjocx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gtyhybcqj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gzxzzjypu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gkescpvjm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gxclmefxa.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/grauucjat.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gpwktqufa.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gyenpvwbq.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gxofenbbn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gnvjzinrc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gbqkafuwt.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gvftpjzfb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/grfapenra.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gjgqfoeub.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gnylruubc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gztbiexdz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/grcifkfvv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/goubvcbtn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtoqtwnnr.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gschvecma.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkywrnzpb.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/grlkchsie.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gfqebmgzg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gzfvntavo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gmbfhlnxd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gkxxxmkzx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/grewkttvx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gjpgnjrtq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gquooehma.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gcmmtagnl.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gwssgkrvj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/glgaaqctr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gmggsojrt.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/grmrnyqej.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/ggvqtvscc.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gkbxqpmqs.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gjftfuaox.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gyvynuqok.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/ghyacohfo.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/glhtdwrhe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gboxxkrai.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gfgnvkibq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gwkjyneam.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gemoijzol.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gvvxjisnr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/ganyjpqou.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/giuqwedqu.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/guenfpcmy.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gavktcvta.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gdwmseqkr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gilrdluyo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gnvrlcekm.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gtlmihtaj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfoyoaoua.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gzheodhul.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/giqrasjwc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gpezdddaq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/ggegzozdz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gojszjvsx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gqwpzeogb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/grxxvvnpk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gnimiacpb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gkbwnnnxm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gqcjqzkzg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gpjrsmryk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gdwmofhjm.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/ghpwlztrg.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gyoefifro.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gksudydag.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gzecjsssb.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gxlkciusi.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gawmcpnbe.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gexalkeuf.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/ghorxtiiy.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gcubwkvfy.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gwsefwjzw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gbpmvqigr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gspskjxcr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gwajoqdbt.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gwwyqjqze.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/giqpnwswx.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gdxlfbqoy.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gpzfrlmkv.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gsmhmhbec.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gdyknpoou.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gcrqlzfjs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gbojrilkp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/glkiqzpbb.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gqqtfhnwk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/ghxtnohef.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gcaescwlg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gghuobyya.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ghbtkjvtp.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/glbnxdbbw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/glwmlvjng.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghqahwyuk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gtqmngyje.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/grqepzlnm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gtsubuooz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gglltllap.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gfvtkoegd.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gnsovhwoo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gpzknfzzt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gbzxcotvz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gvdfswrza.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gqorulzpw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gdzocxhau.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/grpswiahs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gknbzaqck.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gwdvsopxq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gvgtbkivk.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gmuumbokk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gystsmtaa.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/giyslxyte.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/ggtqxdyzz.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gupjxqroa.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/geeziconu.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gsxomprsz.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/giyouidwf.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gkihjtemv.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gweouzdcn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/ggalgxhzz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/ghowwcgmw.sHtML


<!-- 参考信息 -->