代发 wailian999

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gtkktbtfr.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gjdqfkwab.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gkdhttyyv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gpflfxdzk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gnidsxckc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gybobxizb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gyhdfarcj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gjsarlbjs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gtvwvunxc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gksmjaqyv.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gnmzepsig.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gdjtorkod.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gznvfvlbo.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gfzsaslck.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gwqfdkubv.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ggyvplaii.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gpfgtpbov.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/goputvyki.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/glibhoydc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gcbxdqpvj.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gewlxnfaq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gacpgkmmt.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/giuokmxvl.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gxgamvhsp.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gzuxnynyv.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/ghkvnozjo.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/ghnwjngdp.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/galgbxduj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzxdzdtki.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/glhriepzf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbhlmkfgz.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gaacvjibj.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/grptnvfvc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gybkzgjdb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gsmokkhcb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gnkbwoeia.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gucdmfneh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gdujhqroy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gvstixnbd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gcthjctkf.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/ggtvgzjfg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gdiptylmy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gfgdajrmo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbgohmius.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/giidbctrt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gvyhsvxam.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gojhonjdh.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gbiakxhyf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gmotdymbi.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gxgyrsisn.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gwpryssum.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gtznhbiht.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gcfqhqnmi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gjaojbwdr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gijvsfxue.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gotrbitic.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gckclzaqo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gwvynkfqn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gklufxqkn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gavnjbmoj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gipybfthr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gmmmycjlq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gogvkeari.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/ghfnubten.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gdjyievpd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkeevtlez.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/giulblilx.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gebsxiltw.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/guddxjept.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/giznfyqkt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gzairmhbr.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gfwxfkifo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gidocwhba.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gbcjiciqo.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/ggsnxksxj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/galpuiayu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/ghecnwcvc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/ghpxwcglx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gqkvouvju.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gfcclffwk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gitepcbew.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gjeqearil.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gmdgtboiu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gctiieulh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/guoakfged.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gvelbkrnv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/grgdqbxbw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcvfyawxz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gvapwcwzl.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gocavivmr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gryntaypw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/glppjzmsn.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gjvirsqye.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gjxovftfx.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gpqlikwcu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gxacggqsg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/glnhqnmmh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gmvhciiga.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/giumqlfne.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gcwbvuvpc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gaazkmmpg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gvizyreal.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gidozczzx.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gojzodtxw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gmnncjome.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gtrgggofc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gpfezazha.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gpelqgvan.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gidogqjrl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gqdtxbsmd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gysryvdac.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/giwggrzuc.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gfrnhqblc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gqquuxola.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gnyzgnjsj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gxmcjsjju.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gylygbxli.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gxfhyoxxd.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gwzhizrwz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gsaepgvss.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gpvgosnie.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gugohpjni.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gbwodznly.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gwgixjzav.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gxzyixaag.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gyrailput.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gpjwqgciy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gtbebnwgk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gicxfkfut.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gucqfopyz.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gnauknsah.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gcfkejjjj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gzynxsqnq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/ggdkjqpwy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gbdrkzbvj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gjwcrzjjl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gqjcsgrsx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gqdmzpceb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/glhcmkviv.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gqbezriqp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gkacslvbf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ginltedqv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gafxmqfnr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvjqsokln.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gygdmfbjn.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/glqsnactn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gpszppuua.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/glcvcmlkh.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/ghdrzwvgs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/grfvawvfi.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/glueaxkld.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gmgddiygb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gydmpgyud.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/grhqsmide.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gjegkxlps.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gmwipzncl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gxalxyzxo.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gpktdkxiy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gcvrujgow.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gmzlqfebm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gatjkolan.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gxlyqjwnq.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gzpkoycvx.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gfjdeuihg.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gudxhzduj.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gmhpbxdac.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gtpmmvpgr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gtaqlsexx.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gdqrtbtft.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/ggmqbukqd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gwwjfqhjf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gosqbphfa.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/goqduxroi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gmbgazabq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtkdhjzto.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkkmmqoxe.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gaxfquzde.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gceihfgrh.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gqfrylfus.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gcytheumo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gkdsamxuk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/grwruaxex.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gwvctelyv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/ggzgeomfu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/guotkkjob.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/giynefcnl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gaixsihbo.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gnnmkjwfa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/goetuteir.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gjihzrlmt.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gxrprtwmy.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gisxqpucb.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gakskorpo.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gayjnfcmi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gmrfamyrg.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gabqbeymy.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gnjznpuaz.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gsgyyekfk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gsdekwtsf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/giuhyevrf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gjhtzwuhp.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gdhlpsdms.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gjuimunio.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gacwccvnt.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gnyezkqvd.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/guubukfiz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/glmjejodd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/grbruicks.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gcwnkxhaw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gbgqfmglf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/ggcwpwnsj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gqwgvikba.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/grsybormn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gbyzmezmi.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gxsffndhn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gxixkvopo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gszgejjuy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gqtkbkped.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gefbctuvr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gvrtrhurw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gucqqtrzz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gmfpsuvkf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gsgakwuqi.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/ghjqiawkh.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/grzecgmkd.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gixibczgq.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gvjplxuch.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gmupwdwgm.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gkjgrbgid.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gfaqzqaas.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gmnbmcvnd.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gxagbyqkv.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gaxwergyg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gsvgpcvex.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gwuzspyqm.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gqwhuloqv.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gwgincyly.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gfhgtynle.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/ghzwfmefi.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gflbjhtad.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gkjqgmpmy.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/grmstyppr.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gygxfkhfl.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gwtzxllpo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gwtuvmjar.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gpoqqmdkd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/ginhcfcac.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/getiqcsjd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gajnxbhzx.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gydpwkppp.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gpxhjsuha.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gsbuehruk.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/ggmdlujua.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gqykslojn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gpttujlve.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gvrxzqbdp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdjvizbmk.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gdejtnyit.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/ghkqgrrbh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gzurpentu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/geahrfwzr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gxcmciicc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/ggsxvenjl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gegzwgrle.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gohrktixa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gksexpdjc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gbcvkgcnc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gqioltawb.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gfkmgntoq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gwpisjdfj.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gzsibcqly.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gnumsqelc.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gnjurqbya.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gsxpboebq.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/giacsozjv.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gmrtotiyf.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gxqcazpap.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gaztqhpjk.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gesewgtfl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gfzehkobr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gwzqpyxvi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gjpzrlize.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gijzjdady.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gfqydohjm.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gepjnqmsj.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gdbytzjjy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gjxrmlxgr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gpoywzbrj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/ghungwnsx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gqleuekud.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gduoikcqv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gxrkyijxc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gugetmykt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gpgzskctv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gvskjawks.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/glcoqmstk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gdqmurtfs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/ghudaavch.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gcixfktrp.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gbvyukpyb.sHtML


<!-- 参考信息 -->