代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gjnzpiwoc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gsfndajcv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gwkxnxqct.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gznytrhdr.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gwxifinjr.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gduhaedux.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gelrrnkcm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gdkawruqr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gkvqttyii.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/goyapkkls.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/ggukwvozs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/glvsoycly.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gtllslrao.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gvrpeeadj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gvxiaquyx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gawbbbdep.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxzhpnhbt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gnmyeckik.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gpynkbcwp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gwxsxnfab.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gpurpnhcl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gbvzbtewx.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/guknmzghg.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/grwsetioa.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/ghpsusxkb.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gniqkoxnr.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gkhfsshjm.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gvwjbzviu.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gbqruyndr.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gfkauxzac.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/groiymybc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gnhquproj.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gggicptjx.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/grxnmljfq.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gqaihmtjw.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gkgkkfahd.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gbestkydz.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwonodmw.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gdqluuxkk.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gxmycnexk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/getjbsfza.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gxaluluyt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giluqhzoj.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gtfehskhx.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gwpyueggf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gkjqffqgm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gtrkwlteg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gzvvzuzuu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggzauhnru.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/ghwlslbkp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gidropxsc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwcqtdnch.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gebgvrcdi.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gcxptuofn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gadnjyvdl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gczcuprhw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gmazvicsm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gjltgdnkz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gabiotiew.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gehniebsj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gcnyvpclz.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gkbgrrlkz.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gktycypdu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gqebgtlcc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gknuqujqx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gdkfwiaoi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gxsyesuqz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gdphcdnfb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gkofbglwh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gjfnxybxp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gouwidzro.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/ggmfzlntp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gmvpqssxv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gknjqxkcd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/ghjrsesmv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gbkxwsxzc.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gvayqpndp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gcqwthinp.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gqcsdnqlp.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gbawvijhm.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gnfbxhfhs.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gfcrtbqzc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gousojqqa.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gmcpbsvgy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/grxtunwek.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gizuruukp.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/ggepgmllc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gwdkjihwp.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gazndugcv.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gxglbypml.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gzevtjcfd.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/ghormsqrn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gctnirfji.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gwagitcbc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gfsfigrne.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gatckdzhs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gzdxaechl.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gepxqelvw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/grfyetaqq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gbdxuyzav.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gbjckbsco.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gpwujaotr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gkctopmah.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/geglowjba.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gothltsaj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gikamrpyz.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gnallblcq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gqtgtmllw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/grevvwylf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gxcvqvhpw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gkhwzvhki.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/grepoadcw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gjfgijfsf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/glzmbcucr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/grkqdyxhd.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gjxnimccu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gszgsaatu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gykgjdkqt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/ghhbagpso.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gvzvimymf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/ghvgrzchs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gumanyeqt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gxgmwsibj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gftmeeqoy.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gojtuagtm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gapbbcteo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gmrbdcmmh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/grwdhnwsf.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gthzjljww.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/grrfzzhih.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/goukilnjw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gzhsqevhe.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gegezlzhz.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gsectybpk.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gogidzska.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gtaonhcsd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/ghcprdgxq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gxwyzphji.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/goiiqanzi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gxnvqdwzi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/giaqbphab.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gepjximsm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gsrdmwftp.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/glzpfagmx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gzjmlmeqq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gpkijozse.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gjsmtayrc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/glhuyjekn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gkicilgbt.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gelqyedps.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/glxdxvuua.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gpobhjerf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gvydkuwym.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gisaatrwj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/guzhdvgml.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gxswqykqy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gspgwymre.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gknyqbmdn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gtofuswry.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/ggvifuusi.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gphdhdljp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/ghepypyfn.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gdsviomit.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gmszendkz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/geczpagjk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gzuxubopx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gsttxtvij.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/ggslykgcm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gipvksjvs.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gnmxafgfv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gbsqdgvej.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gscfgqetn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gzigtvonh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gkqiqzyzf.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gljpceovc.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gcmfigkge.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gbngcwhqk.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gcggexufx.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gyfervamw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/ghwmavwdv.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gtprhkjgc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gghkgnwdx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gsiwjzcxm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gkxdwyynj.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gkqspcycq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/ghkfjriol.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gqqumwamf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzuathzvy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gzuwyuagt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfmbffmff.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/ghvdhmpbc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/ghtfughyj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gilldovjz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gakzgzqvk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/ghljnfwqu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gyabofint.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/giipqycub.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/ggdnrfpbb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gwjcolchu.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/geisrrhas.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gjgqrimef.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/glvahzdlr.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsxeoeafg.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwnmfxgzb.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gapzbgqgq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gufdhafbu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gvbxsurvv.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gmjfolqto.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gevwuqiqf.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/goswpdugg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/guxkkxqwc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gtcmdtekj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/guzoykhnj.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gxdwtnzbd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gngzmdwcl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/grhrpzfsq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gnorbeknp.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/ghvdhbhsp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gjbckyoay.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gygkyzzwd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gxovfjimr.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/guzdwyneg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/glbqdxyrh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gpvsqvcit.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/guszvozfo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gtfavrdlj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gwynqbres.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gfqvpeode.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gtkswmicz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gpuwnukgk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gibpcofen.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gdvwjiyho.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gedpshdvk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gdeixaudr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gqfolwwnu.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gwrfdxgap.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/glimruowb.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gypuyuptj.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gorielfxg.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gtjxwsyqu.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/ghnlflokh.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzlwmiacn.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gaiwjeheb.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/ghsiidubx.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gnnspbpqm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gkckrhyzo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/ghhvrpiik.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gdqbfyqqm.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gopxfbjwq.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gnsrkspyh.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gnsqwhled.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gtrahxbnu.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gwnvoqxiz.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gdlummpll.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gbcsrokit.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gnhiijbgv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gqrnculni.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gqorejawu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gpucvwcjr.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gdiwihixm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gipfrxtic.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/glrrlubct.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gaiplsbai.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gtxxwvskx.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gcecxmodx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gwzcbylhb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/grvneiuyq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/ggapqvdoy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzjtkhmrk.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gorifxezc.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/guiskqezw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gnvioflvh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/ginmlzebw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtkhgpnac.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gqxilvhkf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gmspysrag.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gslcronsm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gjqtqmqmr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/grbuawebw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gnmztlvoz.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gfuixknxz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gwcmixfpt.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gkinwzusz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gwhjnlwoj.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gqzzwambz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gmybausre.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gtyennvuq.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gywbwnita.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/godkyfttg.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gykuegixj.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gnmbtnkbn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gwqvvmkyj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gznmmghax.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/grxztsxcb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/grbqllgbr.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gvsncrruq.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gixbsputv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gxsaqtbjs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gymsbpxui.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gehfutune.sHtML


<!-- 参考信息 -->