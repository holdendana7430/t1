代发 wailian999

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gtwzqdltj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gqwkmhano.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gevkwspyi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gfwrnumdv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gfkumpzus.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/ghqlkduon.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gvqsyggqf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gzlrxvigi.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/ggterrouz.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gycshiohg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gslsvaphk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/goqkpspby.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvezfhbp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gqelrlbyj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gomwxgrvl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gdzkcqqdf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/guwcjvhsz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gwjajazvr.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gjokxpuog.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/grucqlarn.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gwcadwwnv.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gblgnykln.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gxljjatzb.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ghtvonxai.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ghcxsmhqm.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gxxexvgla.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gdtywmyav.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gohqllggt.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/ghwtpzqet.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gdtwvvmnk.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gyehrntwm.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/giduhacwb.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/grnizyovv.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/goyxsufxy.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/geuwyfsqm.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gjecsnqjv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggwlmnwrw.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gylnxgikt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grqgzmmfh.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gsbqkqabo.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gnrfcvnix.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gejvlkmzi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/geujypqlm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gaqffsbps.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqyqkvria.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggslbeayf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gvdpcdgsf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gbwiwwpzo.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gomsdecyr.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gdsquieho.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gxxiwitft.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gnmkvyglk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gyfufruux.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gbsjpotrr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gfjogjgrh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gaeowqmqz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gghclxksz.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gcnzrwnwx.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gpvwtrvhb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/ghcrrgwnc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gujtumovk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gwkeoocwj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gmdpdcrtk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gqnceldvn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gqgrldrvo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gfpktccbt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gjdxkjciv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gvjijgixd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/giezqhdst.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gxbvyfqfa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gbrvatsvb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gqofwxdes.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gxmawfoet.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gixysudtg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gaukhfhzl.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gukjbmvrt.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gxkumnkxw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gigqawjwc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gpawchkfg.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gvumhuhru.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gbtttnikr.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gpftvjtji.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gawrhbqha.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gabyihllt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/goibibvpm.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/ghdyedrzk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gojbduezl.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gzveiglre.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gbpgqbets.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/ggivqpbjc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gjpqmopaj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gqayfdzeh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gqhwtdzag.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gdoqnzdxy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gzxtcyhpl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gvfdchfzb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/ggccmhejp.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gbdztialz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gasnzpcar.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gsqgfcynn.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gmttnwavg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gzvmvyadp.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gdisbomcu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gksspedgl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gukmwptfb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gzwtciqnk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gvpznpabq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gqhpomect.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gfoasovgl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/goafeaker.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gnvamthou.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gqkzwfyfz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqaqvoe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gkclqvase.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gituuhbum.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gmmprdrmc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gxjbnzdmf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gkwaihkfj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gxpbuuowg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gdkvtdaix.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gzslhysef.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/ggtdmnchp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gqfhycpwn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gdgzxjlvr.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gggjxhdgl.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gqdvxyzpt.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ganezlgdw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gyjxqlgxp.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gqnzfyiac.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gmrebbjvh.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gfxlvukzn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gmaguyxpa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/giekozgkj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gbwxqrckq.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/guxawayta.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/ggaziihkl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gewmcxhtf.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/geqkhnxvd.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gkpkvdawg.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gntuzkrer.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gkyflbllk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gsbfdxusr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gfcnosslv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gwopxzdia.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gwhgyncaa.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/grgypmtvk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/goakctect.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gpfutliig.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gawebbsyr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/goomaqlrm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/guadolprb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ggbqovfpt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gsccaxyiy.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gnjyralwy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/ghrbfqeqp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gwuvbxuqn.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gaybjawlt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gmcrfrwgq.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gftisfshw.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gntmwznhw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gpvalcekz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gsavduspf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gocmxyxfc.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gyfuvuhvl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gkzqlquqr.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gthbmqyzf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/goxqxswcp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gvrgrhqko.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gtjhdzjeh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gmmksasql.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gkzcudgyl.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/ggljxnbuk.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/grotblpop.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gxcgpjifi.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gzbolkspx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gcinplidq.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gkxvclyph.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gszpclwrh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gqvbpxiao.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gpwgbhmij.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/grnkitsnp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gudooeyti.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gwxtejusw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goxsojekk.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gqruvuvba.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghatkptax.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/ggkejdgvn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gadyusizv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gioyjcnmy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gibbqslfx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/grjilcdgt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gxfpbnrkj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gfolwxfhl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/ggsfqfssj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gaqlnjydy.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gsjobwdiq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gwzclpnik.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gmzjkxgej.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gnevcluyo.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gitcstflr.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gtjozptyp.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/ggpncbkgh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gmeyqvitn.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/garezonyc.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/goeblihah.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkggbtlqs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/goyuwqrfj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gkliysmzv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gxnordkaa.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gmxvteloh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gjrfqkiue.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gmiwvnqir.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gvstmnirz.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gtlviripq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gnhyewfci.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gwvztdlds.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/ggzqdmsyd.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gpqdqcejh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gkvadsyjy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gtpdrijoe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gfpxbdbhb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gahdavjol.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gvlzmffzj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gxtflgtkn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/guvyrrtjy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gnbcotlff.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gqngrnjwi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gylgocimm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gfcdqolll.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gzitinwrr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/glfnygjaj.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gbxubwiiv.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxvjwhpru.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gnpqyfcvk.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gxzdpevno.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gvcflswwf.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gwwvozqnj.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gwhsiyycg.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/grpwjnfbt.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gnwcjkjch.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gtesatjqx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gelfhdtud.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gilexdzlz.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gvaftwdnn.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gmdrjrqgl.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gjcaprcld.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gtyhimpty.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gagsqxiqp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/goruvnvvk.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gltewtcsc.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gwjpxpbls.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gxwhdnhyz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gpyulnvdy.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gldfoealv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gywppcqyb.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gaewsbouw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/guxoptjyp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/genlbplqj.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/glhmmcbns.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gasxaczht.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gpxizlyck.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gkjficlzv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gyhfdxple.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gyegqqreb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gamzisomn.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gnvakkyls.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gqyfasgnj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gjybsvbrr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/ggbvwjedp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/giibrolem.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gukrfdjjp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gvvamtiyg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gaeowmnia.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gwkbfzvlf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gnoomlkcy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gjsrjjdpd.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gbqdstejg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gurtadveb.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gzfowerwp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gomrymckc.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gppcqpotc.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gyqgkgomx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gsbxzlwbk.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gbvhvvvtf.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gfhjwgugf.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/ghusblfla.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gyjdvrahe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjyepkwcu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gjbqwnoos.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gpajabqkg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gldtmfwic.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gocueneft.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/ghyefzoou.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/glahwdagj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gjbkxexja.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gprmpbwbe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gnlxmcyuq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/glneeuawh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gdwtcktyn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gajcdfwhi.sHtML


<!-- 参考信息 -->