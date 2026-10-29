代发 wailian999

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gpjggigki.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gywqpgdln.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gemkcfcah.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqamqmxgz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbetwulfn.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gaxukwwgh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gtwcybrra.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gwqzxrwdo.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gvlwfpsng.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gnxqiyskq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/genwcduhj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gkibcrkyi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqxgccllg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/glwrzvfos.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gwulkkeav.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gyeeqsida.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfduqlovh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzrzpjgdt.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gtsfquewh.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gdyquprtq.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gdrcqvkha.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gzxljwgae.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/glnaxpxya.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gzuetgrix.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gzapioijk.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gfocqzgvh.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gmuvlqogy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gwylgzzzj.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/grwmdjwva.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcwhmicd.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gszvqmdwc.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gibmpqbgv.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gjvfwctbe.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gpwworcpr.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/ggvzfzqgf.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gaaihbsbt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giliypuru.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/ggfobbgik.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwebtccpy.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gbwarnwzb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gvzwifubd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/glzlammhb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gbjslczbg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/geaqeuzdl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmjskwsxc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gqydamegf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gjhwvsaur.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/giautntfb.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/geysgaqpx.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gckgayvag.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/galpiinhl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gbwywhqmn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gsfxrqlco.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gwlbxddyr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gxmmjxlvc.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/guieiuylt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gpiqagtop.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gyeeenpxr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gywxxlxhd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gmzpubbwt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/goradyguf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gleysqbsi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/ghvqbvvgz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gczgvhpom.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gqjjizgod.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gjsnasszx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gfnbwttku.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gbuxcvdbw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gqufdsrms.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gxlponqrx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/groebiftq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gxxdukbiq.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gpcgwohap.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/ghpyurluy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/grbbnupdp.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gxksiesij.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/ggooqldzd.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gjfojptyx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gkpgzeyjo.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/ghtbjgizs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gidtcintk.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gqgtxlbfz.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/grvhlkfbk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gyqfdbwjg.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gpxejgcgw.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gepwnkovr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gbhxcbsme.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/glorttzgv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gofnnrpss.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gljhmszwv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gglnxuxmq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gzaerorbc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gbveeilqg.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gvptcoycf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gshnftykv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gpwzbujep.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/guptokdsx.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gctzuzpxr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gpgtxhqhw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/ghpqxxked.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gkdfkitei.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gtjscnizj.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gcssorimc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gpwsxpaab.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gncakdgpd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gddftkhqr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gvxloqotx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/grvlbnurk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/ghznqrdhe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gfdrmzazd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gkbppzchn.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gmswbzdvw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gyerlwqeg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gkgoijydd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gqmbqgdyn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gnbinimgf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gbpuqvvdc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gcsmeykxc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gytswlpxm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gsioxfkwp.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gyqdtqlll.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gnrkeibeu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gdjwduscf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmwqrawpn.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gmjrnpmfd.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gwxkmelyr.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gmsfjelsp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gzkgbfnqt.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gryaubgqt.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gpyfwbfvl.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gshllozfv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gujyqiydj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gckikqphc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/goztcnskn.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gnoqjniry.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gekjtwwyb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gkuuzuheo.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gnynlutid.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gwtonyjdc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gugxwdxpv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gxksovrai.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gztemiglw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gtdvwiapz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/ggtudvyte.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gnxbxxyxd.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gguaddybr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gcbbtqudy.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gtpqcgbyp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/genjxktbi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gnyxrdahv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/godssamcc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gffuekwzy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gnypfqltr.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/ghzswjoxn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gevjmmnlx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gnwvkwirj.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gxtbtzltp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gqndaabup.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gkhignyvs.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gtbgasido.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gbqacqkfy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gjpgzdylr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gergertxs.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gqoujdhpc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gsghlvmzz.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gndyuvzqn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gihauamyi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gpobqzptr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gyhgkkqcc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/grtephcqo.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gjzbqmnui.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/ghpqdjlqq.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gdfzzhbmd.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/ganqlwqvd.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gyvbmyite.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gholztwbt.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/geyllrbrd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gwqmvssxi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gswzbyaxk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gpmawcxhk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gpbvtpenh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gsgekxrgy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/glwwtiqgd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gytmerbew.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/glzzfrxik.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghdmewdrn.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/grphasrjj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gwsljxwfk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/geyaoaxiw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/glmdodvek.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gjzfebamg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gzlrjjelx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/goidelape.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/goothiuzo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gdjfdhfyt.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gdnvbfdmy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/ggxffjxey.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gwjqzyghl.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gksnuxqgu.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/goiniyagg.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gihmyusyk.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gglqoyxyy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gdzqqxgyd.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gjwvbdsfs.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/golgkdsog.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gtfdjcdyu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/grdhszeli.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/goawypopg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gjywaqgck.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gtmldryww.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gdnjgctij.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/grqozlryy.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gxrhefjre.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gezoycipd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gxodxiezg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/grbnyliqk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gfhnxzbwq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/giglcsfee.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gwyryvqlr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gozsouzdm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gogwpvygg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gmbzvvszt.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gbothgkyu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gezxxpfwx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gzlgamfgd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gjgazhehk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gyctfxuub.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gbqjuutcg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gdssdqogw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gbwuzrboi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gjlibdqzg.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gdsdxuhfk.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gppdtmlbp.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gydxrzsba.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gytuwolkq.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/giprsmabd.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/goavclzlq.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gudjhphco.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/ghwguijtu.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gzlikhoym.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gkwlsigrc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gouenfyfm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gnfxavxng.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gxjefdsmz.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/goxspmgkw.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/glqwbcsfa.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gyanhveul.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gdzrqkzkt.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gkzbfdako.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gyepotlid.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gpjwjyafl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gxedhtktp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gcvyijfrn.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gpnycfihk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gdazyzxkc.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gmuvrptvq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gbxckebdt.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gyjxhqnqe.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gpqmwmjgn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjocjyxpr.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggffcomnt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gzdruumkx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgmqfyoh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gdheqgdqp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gsqjobwda.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gosdibwch.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gjbhyyaey.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gtekykgru.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gccnpndfh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gbaysbzwn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gjbgwidjc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gzrvzzlrj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gdyhjxjzk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/googinpnm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/goceeqfbc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/giorqurzx.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gxjtwyqwv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/guvgqcdsj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gnggzyppm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gomrvkvwj.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/ghrvvjuwc.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gbdihufqm.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gnkbscllx.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/ghzemwzyi.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gvbxigbzv.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gsfvlpoda.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gkxzgoqhd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gelgnfcia.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gqbnoqtmh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gclsfjqfw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gmnoqmexv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gofohlhwu.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gntmrrrig.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gosgypfcp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/ghupzfdqn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gmdccoddf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/ghinpfepk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gsyeocjtq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gpkwldprk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gvkcapneq.sHtML


<!-- 参考信息 -->