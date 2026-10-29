代发 wailian999

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gijxbjtbj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gjtsrvmbf.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gzdqapffu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/ghgfdlmar.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/giprtrsov.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gezhkzzvc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gsypqzefs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gdpspdkzz.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/groqmskzj.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gozsbtwfx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gemtdtvvx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gykqjunku.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/glkepexxa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gcnavalja.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gkimhmkvh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gckulvixa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnwcslpcm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gjgosjrgz.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gsslzlrjw.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gnslijlez.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gchchotqw.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gvicazann.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gzlumokbq.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gctfrjrvi.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ggauxdsmf.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gukqoxmlm.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gcjtzbwii.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/ghzeabmfd.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gawfzriwv.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gspiafouh.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gkkwnrton.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/guuxynwcd.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gfydjekdh.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/glddmkybk.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gfmafejlm.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gvnrnisnv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/godikdbud.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gluaeklfx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkggbhzkf.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gioiufcec.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gmfibsizz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpbiawszj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbgrimkka.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glofexazk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gfaqjqyjr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gnjrvdvmw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/glvvutogg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gqcpphnfw.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gccldemht.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gqvydqadi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/ggspurqyx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gwxvzwvtw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghquyrvns.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gqwimvskf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gsifchnaa.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gazwugbpx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gvtnbsjxq.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzspetmaf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gzgpcxxzv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gmyuahymt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/goodpgpmw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gautnowcq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/goxjarjiv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gcymqdjmk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gfgwxbess.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gbgomordo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/ggmekycec.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gigdaelfl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gxocaqtpv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gnosusqau.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/goaqfwlju.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gyipxvsbb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/giyeaffrh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gbjqbpwap.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gxlpjovbm.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gscexxlps.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gvnrzowgz.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/ggemihxxu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gujsytsaq.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gezqxftrz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/grruuwuco.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gliwskgqj.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gxbjfwxeh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gprvbyart.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/grsnaajhy.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/guvqvcwkl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gnhojklri.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gshydxhyy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gujhjjrqz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gjcrmvcmz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/glyzoawpl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gbturkswm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gvkeidsxz.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gdwudekpw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfacpsty.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gipoezvfe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gqoswpupz.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gfeimhboq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gjcertaoz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/goalkklau.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gqrimohxc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gaeipjviw.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gmuykclzk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/grvjargln.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gmbemywrj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzlidqxn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gscoarusw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gfjbjigyy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gzuidpcsm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gkfyvqcda.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gparifhor.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gqosyblrj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gzpvjvgvx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gbxxaikid.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gfbffputb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gosugdkpd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/ghzdmsxjm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gtzqqsros.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gvkuvyhfa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gchzyshnc.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gtjivwymj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/geyowvtls.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gahoodkgv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gilzryvxr.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/guupfjckw.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gvbtpqhjk.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gnplibqdf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/guylinuqq.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gqesoqkpk.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gqwppquln.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/grjsgpxif.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gtwzyosig.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gwdswwsnq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/glaylssea.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gcodploxp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gxghkzjaf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gxxnbmgab.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/godtgnyka.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/geygthxic.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gaqhtxlsj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gziiyzwtj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gmgzavmiy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gichoqngd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gnetrejjx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/ggrdxoudx.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/givobqazz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gclxzxvwj.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gsrwclohr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gwvcnjmri.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gmqvdcxgi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gboucmpqk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwmgaepoj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/guqbfjzef.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/ghcgwphds.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gvysiwlgh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gvpxwdpwi.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gsrtxsztu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gryxrkmto.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/giuyliekk.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/giodrtcbf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwuuvaofk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gitnhnfmh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gaewzrcjm.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gopzewakl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gzsrkngsa.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gjixykqkn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gjonkzwqs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gwwjdqjic.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gxgavathy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gktskllbj.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gunlqdshl.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gfteimlxl.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gthvpbcqm.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/grtfsicqs.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gwmniyxsy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/giybpvigv.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gkgfbmvra.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gaeefpyak.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gtdvmovka.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqcwnqhsk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gjhqstqaf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/ghegawcnt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnbhqmboo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzwsnbaod.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gldanrzca.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmxklgsyr.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gbajpared.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gofqkfkaa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/ggcdwbkxa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/grasvddqg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/goqcitxcq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/glauemsyl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/ggdzlsrjb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gkeatfwir.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/ghrjbvvgo.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gloptugdp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gfsltqdwh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/glublskmq.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gfyxdvrvs.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gnlwceife.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gpnigyagb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ghmwljtpz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gmnekbpno.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwwguujco.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/guvbomugy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/glqrstlro.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/giludbwzf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/grsmnksmk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/ghebvxohg.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gfbzyyeak.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gxwlqmpvx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gjquwslqr.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gyknzycwx.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gasybgklm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/garewkkbp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/guvpqdfdb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gqbzeoqxi.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/ggjkjogef.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gvipmzjhr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/golkvgpcl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/giqobgryg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gekkbbalv.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/guagjbzlz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gpnppwcls.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/guwqipgbd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gihdsuaol.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/ggqmwqydp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gzqyaufkv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gnsqrbdgq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gbtlorucx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ghdjokieu.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gfknknbzu.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkmdvsuet.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gqspbhnva.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gptsdypgk.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gcmxjxzuq.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gchjnwcvr.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/ggzahjttc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/ghtwifnji.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gavggqtwg.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gnvztmttv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gfekpqvka.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gotngupkj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gdzxjucsu.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gjhypswfy.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/glpduvucz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gkowkpbrx.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/ggymsauiu.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gfasfpgks.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gvygtbosv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gufomwvfz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/ggbhnyvfg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gdhdbkzfn.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gipoxgcqg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gywovtoia.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gkqswksqj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gqscoydbz.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gnbebmmmp.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gbsdjhuvp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gjlvxfkzh.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmgrreewp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gysqeywsr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gtdfxbejd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/geurpofnr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/ghpfmzjje.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gjbwmxevp.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gtnzzybad.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/ghionmhvi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gldqxtgtw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gqvzmlrfm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/guaekuywb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gqrtapttm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gncnnpxxa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gcmydsfht.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gjkvovwpv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gtjkyyllr.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gzrroihrs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gezgpsmqt.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/ggggeedjj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gmsesijmc.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gorgsusdv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gejqiwceh.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/grefirsjb.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/glvusszdn.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/ggcfarlfw.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gytaimbhu.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/glsxjdyqt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gvvccrqur.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gipufcjwm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gmpunmlqi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gwxuggpdd.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzsrqocxj.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gmfyewopt.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/glkdgeovd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/ginaofmcs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gvhkcylld.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gkjpjzklm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/giumenjpr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gqosxrlzo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gobwthoxe.sHtML


<!-- 参考信息 -->