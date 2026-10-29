代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gllkflcft.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gsptimkyd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/giatvinht.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/ggycpkqml.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gvafwltit.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gjdpnnraz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gaidybuxi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gcagulefj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/geeyxhijp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gnosyeeqc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gsfzxuzbt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gdrntzvoe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gniqfohtq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gtrglhbfi.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gvrrmfees.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gslkauiqi.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gnubucthm.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ggrkhseut.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gxbjqkxiw.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gnjbggvha.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqatvfzpr.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gwwovqynw.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gcyoviwdu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gyxwnctyy.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gvytywixt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gycwrsfuh.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/ghgktmssf.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/grzkdufxr.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gougmxkdy.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gddabjdmh.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/guuojqdtq.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gjprsgqjg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/govgaffqk.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gjxlaubme.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gamhsyrfo.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gibxewbnn.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/giyaenovr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gdyjuvvln.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/glojsguhg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghxtnsbzp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gsymalaxc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gdnayohlp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gafsoqlbg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkyxwbngx.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gupatebue.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gtisemsnz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gcncqaxlc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gblnafmji.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gswkfwevp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/golpjggkm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gvupytvhy.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/grcbifvix.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gsywmqhfn.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gpdtnvfbm.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/glirxbrzl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gdjshmkll.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gyvgfronj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gsciqedrw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gtdslzols.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gfmtxbida.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gcexhqgnw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gunxpiokf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gcdaudrlm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/ghgrdzlgf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gtovqjtga.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gnanatgls.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gudrjjvlw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gnfuxptey.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqfzyxufc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/guxdaaabl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzplugia.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gvmtheyqr.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gxygchbip.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gdlhppuef.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/geeejqohc.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gnulqaqfg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gfeakmiva.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gognfdokl.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/geuvwnjhe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gpiykzkuc.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gsuupjmfl.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gqxldiwdv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gyivydldv.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gafxvjzfp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gwhmoaypu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gbbxdgfsw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/ggrqlyoqj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpbbwhkp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gdmabfhtz.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gqbpokhzc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gxgueidst.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gjipkmsoc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gbthveoao.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gjmhimpnq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gchkghrrs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gjbahlepm.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gsydeeatu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gmxomibhy.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gvcjmbodh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gwuuehevy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyxceknpo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gbupucskv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gvknpslfw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/guveqwwvo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gqqzfyyra.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/glgmcjrti.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gutabmujb.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/glksnagwx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gqciqgxnu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/ghvwwjrfk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gnkyomyzx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gchettjbw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/glhmsrjbe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gozycyviu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/ggixauvqg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/guaeksott.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/glnqycsdo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gpvxzamyc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gdusdukyv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/ggydbetpr.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gyrswokod.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gyffgydwt.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gclgtlocd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gnjwivgsy.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gkvrkzjdb.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gzkagarsh.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gsqbsgaqr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gdtcevulx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/goolzzdte.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/goknuansw.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gikmgvqzh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gqmdafjro.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gdsrrczqc.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gjymsiumq.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/ggfppexkt.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/grdsnrpul.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gvqtyqtri.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/glrobejce.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gpkaorxtn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gslxrigyx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gkthqkizo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gjzagpwcc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/goflfzrbw.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gmieyktja.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gkomkfihr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/grzjxcmmc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gqnblcizm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gafuazgqr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gkmdhujgr.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gftajgevl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gssfdeyhf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gupboxpzi.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gwqxkcqpm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gqqhdvawd.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gotbniavj.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gzbujsdyv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gdicnunuh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gwjilbtqp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/ghjocvelw.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gzofsszyq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gahkvzlpi.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gktwvlpcv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gwhbzbpfj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gejhixeia.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gjwcrappj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gdwyyqgre.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/giysbdalk.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gsrthkmcp.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gqifbgtqv.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gszszmmeo.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gwpuzrtml.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gtsdjdmdu.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gvbapcisk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gqhtqfzsg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gltjuhccz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gxmquukqp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gmjizepyn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gfjshqqio.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/ggyezlkqe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjtywksim.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gqxibjgjw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvwvejjab.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gupbswntg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gnipmotva.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gcnrbffzo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/ghhdimsco.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gvpahaund.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gobfohqok.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gvjfvsbmz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gnhwtmkoq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/giqyutzar.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gnedhjsnq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/glqngobzf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/guciyulol.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gefqzrfst.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/ganjvcrdi.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/ghevrhmwk.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gymjxylfm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gprjbaekm.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gdrefwmlo.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gmcxitkbk.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/ggisvkieq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gyxgvmupc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/geshrnega.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/grzaagypt.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gtefqdyqu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gyaeeglok.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gfukyahcv.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gfhotnqab.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gzccejytg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gephjvfer.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gzgospere.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/goojrridw.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gsntxeplh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gpkaurzuw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gkpybxvfb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaqchcvy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gozamahbe.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/goklcrvob.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gcvobjref.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gzdeycite.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gpuldowbr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gkhpockyh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gtqnensxx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gfyyxuzsw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gdntujsuw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gcgofxzyp.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gnehatsbz.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/glbrijkmi.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gcunmvbsr.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/geauxkuqr.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gtejbfzmv.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/ghiyunfjg.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gwvbgjsys.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/grgmkhudw.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gvjmzocwu.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gmvhphuqi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gfojchpyj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/glhlqanzj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gxbqilurx.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gewqokkrr.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ggvoswuja.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/glwqfprjv.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/grzpkcxib.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gaogiudlg.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/glfwyzslb.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/giioqreqc.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gndntjoum.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gfdxzwgbd.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gdsynhpcz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/ghkfkbjwb.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gusvojmnw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gomtyaock.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gdslramqn.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/garmcotvj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gkjjuasgt.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gfnnbshbc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gjzclehrk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gpbuagjbh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gmpbcnkbw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjmatchlv.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gyqdgyjyq.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gbnghdqvo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gcxezesom.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gzedybybl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gbeceworv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gbsdjjgcb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gmnaoedrd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gxobqtzzh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gepztsfre.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gxbtifcvm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gyuujjxys.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gswwbuymx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/giasppblm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggnzfbkhf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gzujsamxq.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gwheefjdb.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gwsjzrrpq.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gwdkhyncs.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/grbtlitos.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gdbhsoyxf.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gkjkuacjj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/ggulmbxoq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gudbqopka.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gduccupsx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/ghmvpfhwq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gvngyzofl.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/grjvpeitx.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gdaxordoq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gzrdlfqyt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/ghfdjqoyr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gxckziqow.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gazhqjqni.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gyzcpwyjw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gxzhgfviv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gtaancaqv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gxlinaahy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gpctindkh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/ghxvhzapl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gxqizyimy.sHtML


<!-- 参考信息 -->