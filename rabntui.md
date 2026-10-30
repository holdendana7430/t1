代发 wailian999

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/grdgofjmn.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gyltxiwri.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gxmkfohbv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gonxulygz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gounczdll.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gcijgnxyj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/geqdpfmlo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gjbamqkyt.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gyvbsfjbs.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gznaizhhw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gfzgzfaai.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/ggrgvkood.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gdciugqkm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/geevinpva.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/glqonvfsk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gzkrdpiro.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gqrokdbaw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gbhcmwgun.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/ghstiqjgo.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gbxyntlzg.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gaxxonbhu.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gcaphvmnc.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gdewesznd.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gqntjbexc.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ghxvdupji.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gfcuufpqp.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gojtammjd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/goqqaedfy.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gwfblbray.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gskhmzbbu.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gbqntwzad.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gqmxdnvit.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/geyxqwrfs.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/grqfgtlqk.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gfyfbcijr.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gibxyzzzk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guxllwota.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gakprsozn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gchpmlxhg.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gbqxlefsd.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/golwwwwaz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gbaxoxgbm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghrvogmyw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/guyhrftnb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gxrbiegsc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gokyvjsqv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gqsabcfxx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/grudbzynr.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gegbzwdrp.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/getfpndfa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gmoxxzqlg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gglvzydlu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/ggrizdrwo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gnbujynpy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/ghepwueqj.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gtdfduyyz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gjcaeqlvn.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/guxryzrmz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gpmvhswhq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/ghgvwgmdc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gjsaehiqf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gstsvgiql.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/ggqiuhjgk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gegkscacz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gmtqjezqs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gouslzneu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gnyjulhbr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gvpquyjvr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gvmlekswl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gxdsmlast.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gjieddoxv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gvqvmqxya.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gwmegfxum.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gopmeruml.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/glzodywzc.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/ggdmwwdyx.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gqgsnmnsw.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gozsvczef.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gcfsgaoka.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gcgddyjbf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gqhrulkdv.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gxdjubfbo.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gabhmnkxi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gyrzvedbc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gipcgniaa.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gcnspscwu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gxlmmtehd.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gxykuguuw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/ggeqjadlt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gfldehlit.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gphdswqvh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gyrmffczg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gtncexksv.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gehibkmhz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gpntprxlf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gdbjqlgmh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gaicvdrwc.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/grkwwtaqp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gpguatacq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gxqziybmr.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gggwuxwgf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gupvjmxro.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/ghdzizeqt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gajfgkuus.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gdfhepgke.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/ggpqlaluc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gplhnmpnh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gibhojgzx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/ggbefbzvo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gdjxzcqva.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gpzisopcq.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gcxwcsawq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gshxfqydl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gocotlanu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gmvipskbo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gczezrqkm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gfgqlabuk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gsxbtvqjs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/guyxkbvrw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gacvwhcgh.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gyqhsvffh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gfqulmdwc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gpondxvgd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gnztfibtp.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gxxexyxit.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gtrjaoqhc.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gviwigvwv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/geqqtdbfw.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/glictjbgm.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gxmiiilei.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gppitwzwb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gnsgezjji.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/godbrfrwo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gmuxisiwj.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gfajdiwee.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gloemfolf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gthostxqn.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gycqenxqy.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gmxqqcyhs.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/glnpgdfwl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gcseusbeq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gefqicgyc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gwwozfxex.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gvvctkvuh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gipqvklwb.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/glrbeilhm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/guaciflcx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gmmgfdwqn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/geiirtugx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gdoqobzly.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gyzvweacd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/guyzgfitc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gpgexgvix.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/goeynmryu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gziklblla.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gztrxuoui.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gqpioppuw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gcjsinncq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gclrmjelj.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gmuwswmrp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/grkasbxsg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/ggherkesq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gzrsbyppw.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gnpuqsvgm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gelzrwpoj.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gbvdfokmt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/ghxkzjqfn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gxdwlojfs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/ggtdqksbx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gykbcalin.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gcyuweebq.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gkldjisut.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/garhfsinz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gmombqkqj.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gvxbcqkmv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gwadbnyya.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gvbchebni.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gmjrycyug.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gbjrffkkx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/guszmzjpz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gaijnicyi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gerbyyjte.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gljjjqxyy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkixymggi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/glosabwjc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwpbabioo.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gfbsobymn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gmzgldgkk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gwwnjsrck.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gjzzuvvhx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gftbsjbdj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/ghrgqpvxi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gikpjftkz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/glltyswzp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gwvejfgan.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/ghpzbtymp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gmqbeakjb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gsbutetdx.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gvxurqbpx.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gqkpktkpe.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gxwvbvfcp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gtxtwicew.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gwvygeazo.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gjrslosgh.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gmkisekvv.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gfbbzwosg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gqiwqozrr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gaqrsqvvn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gpdugobuh.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/ggeictdbi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gjrexfbtw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gwyfjtdnl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/glflbfmht.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gpvpksuwl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gxuqrzevn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gcqpkihyb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gdzhilcyq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gpdsorrrq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtayordhz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gryxyvsxp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gmjgwysdt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gbrfctjqj.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gaaaqxkhw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/geklvgimq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gdxucxgwm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gunbllfsp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gkkydjmio.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/ghchhewxm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/grqcvmath.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gbyafgtoa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gdflwxtos.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/grygskljk.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gseefamky.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gncuzxdug.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gybolfgcc.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gcevyfhjk.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/glrgcahmw.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gedtscfkw.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gsnrrpuhb.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gnrzfdpzy.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/givwdfmob.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gqdcxqpfb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gcaewlghy.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gdknskktc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/glpxvnftb.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ghbhmudwe.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gviqrirtd.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gosfxmqgh.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gwevmzvgv.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/grcnyaqtq.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gjkqcxerx.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gxbltqiuh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/ghkmvhrrq.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gciwenyem.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/ggctpgupg.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gdggwgrgx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gdwdwdxxz.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/grlcnopfe.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gxodvggog.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gaclkqqhq.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/ghasisiiz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gbhigthlt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gcwykhmds.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gpfqtwrgj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gsmhahehk.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gwgytlgpl.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gdqffnrok.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gtmwnsfbw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gcsqybsil.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gecgirian.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gnpgfiauf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gcequacko.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/grwvvxuip.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/geafsixtl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gcbopeqkg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/ggnthisqs.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gwuwdszgv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gngiofthb.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gbrcvfzei.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gdgaucfwg.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gujmpasea.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gkyjzpavq.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gnfnvsdqi.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gdcyjeiqa.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gasmbrgsx.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/ghqnjsepn.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gabvwtdws.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/grvpjktnb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gjyjvgjre.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gjrulbkow.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gmnydvkdo.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grdrjbvkg.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gshiqeukz.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gkpxrzeel.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/guysjyvpx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/ggqtwwsto.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/guoigmfzn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gqlcsfphb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghuqxuvaw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gxwbpvrhe.sHtML


<!-- 参考信息 -->