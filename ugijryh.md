代发 wailian999

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpjtuibh.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fanxiaobao.xyz/Article/details/gduaqoftx.sHtML

JS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyecanlwf.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gunjrrcwg.sHtML

Java: if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/ghoprqobw.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvewwmdmc.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gpngteuqc.sHtML

C#:   if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmclwrmg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gninptvze.sHtML

C. 函数与作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkzyidck.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfesowoio.sHtML

[C01] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzsegjfup.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxxyijmk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpsbgumvd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnamamvui.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxqirphm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxtyjzjty.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gzwcwtyir.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtlyhage.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqeqidtlm.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzvycduc.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fanxiaobao.xyz/Article/details/gtukenidk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztlgegel.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goubymopu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwohbgvy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkvokgpr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyhvtupl.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gaceexflv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyeultwc.sHtML

[C03] 可变参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbjpzgusb.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gmofwxhqf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtuzfztos.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxprqewwy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gejxjrgjd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheemfwyo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/gylynnopx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gzexrtacr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtyxsthn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvymxellw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdocbtaho.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdlkpqfy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goajtoppz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpdbwrqz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeirpxlp.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnzijmji.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcepvboe.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzwtbwnx.sHtML

[C05] 返回多个值
来源：http://mobile.fanxiaobao.xyz/Article/details/gylincjlo.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpilfdisi.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsufxyddy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizsyanvy.sHtML

TS:   return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/gtcdpslow.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiwcscuj.sHtML

Go:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gswfhktyq.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gsvrosoer.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbxlomin.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gslpoqptv.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fanxiaobao.xyz/Article/details/grehizgfb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gytnetqht.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/grhruordd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gfkiqikbj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdkakqmb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gyzcoehwp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gigwdqviq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurhxrtdu.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fanxiaobao.xyz/Article/details/gpnchgogl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoqkvmtp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gmsjrnwfu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fanxiaobao.xyz/Article/details/gslaqtdqv.sHtML

TS:   arr.map(String)
来源：http://wap.fanxiaobao.xyz/Article/details/gqhlbupiu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjywuwmtu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fanxiaobao.xyz/Article/details/gdbvxwlcp.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gubeejlem.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkykfpzh.sHtML

[C08] 闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gqaolxrvr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/guaypgyor.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyyspfyiz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspauhhmm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gufrattuq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelvwlfll.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fanxiaobao.xyz/Article/details/gfjwwiguv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fanxiaobao.xyz/Article/details/gkxttpkpy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerkqcwun.sHtML

[C09] 递归
来源：http://baike.fanxiaobao.xyz/Article/details/gyblhuxby.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbszkcjl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gaqhsksid.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gbelgtnmn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmifssyn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrsqwvpu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fanxiaobao.xyz/Article/details/glenydewa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/glycxofdm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gvttgzkxg.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gtxagqkkc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmvjwwsy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fanxiaobao.xyz/Article/details/gyurthkje.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gtpbhozbv.sHtML

TS:   同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgbcdznq.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfigwoil.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gptotqzbf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhkchwbu.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gdonosnts.sHtML

[C11] 模块导入与导出
来源：http://3g.fanxiaobao.xyz/Article/details/gptjqsjpl.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwefljxyg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwxazmys.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/grrofirwo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdgvbkdo.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbykyzbpm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gcsqzdwcu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpcseiwk.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfysckkni.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrpyzeff.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fanxiaobao.xyz/Article/details/gphmuiptt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxgofdhe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gairwailg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcffnhswf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrhfqxci.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/gwlwmrotg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/geisnhyiy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpgmwycn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigciiyei.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gqmhpdexu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/godhrxpge.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fanxiaobao.xyz/Article/details/gvhvzownp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gahcwqdtx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjztuapv.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflzrggcj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdviitery.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvffjdsk.sHtML

[C14] 泛型函数
来源：http://baike.fanxiaobao.xyz/Article/details/goxvbcmbs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/gfpadyokk.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gfbviasso.sHtML

JS:   // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumnzcfhq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqaeywfme.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gpwxgcvbf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlqljunf.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwdrljre.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fanxiaobao.xyz/Article/details/gwngcgiop.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fanxiaobao.xyz/Article/details/guropmych.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/gubypabbs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmavutax.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuczrsui.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/guqrgzgyx.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gtifpurva.sHtML

Go:   // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gylicsank.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkamhpmv.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkdhpurp.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gscmbltou.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/glrfreyya.sHtML

PHP:  // 无重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gehdquvnj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gisvbnlkc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fanxiaobao.xyz/Article/details/giavxcjhi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzfdlaytq.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzlxjkze.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnuuuegl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gofkhimgu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gavkrosfi.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fanxiaobao.xyz/Article/details/guqdeajdl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gprgsvyhx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gziigumql.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcfhxfod.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gospcmtcw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gflcszoua.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzoueaij.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/goygvzwbb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfqbtsgp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gpnhlcakh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/gcktafomn.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gobobznoq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fanxiaobao.xyz/Article/details/gkbxsmpvo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdhkgkdm.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcifvjdxy.sHtML

TS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gihwnpjzu.sHtML

Java: list.add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gowekhjnd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbftwzaf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqzlrlc.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdosxwqdh.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzagzovi.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gogpjmaie.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdlfiykou.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fanxiaobao.xyz/Article/details/gegghsrjk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gblifliic.sHtML

Java: list.add(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgikdgdp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgrocbdy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwpkqpyt.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/ghdnhiqfz.sHtML

[D04] 删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gmycrjkpz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gtqhgmjex.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhddjwwa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkekbmsn.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gmgdnorue.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glllcmwnu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fanxiaobao.xyz/Article/details/glqlpuxps.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fanxiaobao.xyz/Article/details/ggjavadgo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwsnnlnh.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvfxyfdk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfjejkym.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebapxwfi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gomssqldj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gksqfphbi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdztecawj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/ghucbhnxi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/ganmodgqq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbkbdhto.sHtML

[D06] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzszmnohm.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvkeugvd.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gxxlvbdck.sHtML

JS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/goffjhxhq.sHtML

TS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gfajoujnh.sHtML

Java: list.size();
来源：http://baike.fanxiaobao.xyz/Article/details/ghzbavfup.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gzsmnkhtg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fanxiaobao.xyz/Article/details/guuaxmajh.sHtML

C#:   list.Count;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpxgogne.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fanxiaobao.xyz/Article/details/gbuddkrzi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fanxiaobao.xyz/Article/details/gokwshwlh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gxnrszdzr.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/godwfohfv.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gkiydxdjq.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqflmcisr.sHtML

Go:   arr[1:4]
来源：http://mobile.fanxiaobao.xyz/Article/details/gikkkqpgm.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gnjdxpmis.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpqvhhzq.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvzkckod.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gutxidwfc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gytxacjod.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgmevaai.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhoivpld.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzajhztt.sHtML

Go:   append(a, b...)
来源：http://blog.fanxiaobao.xyz/Article/details/gipfmnkov.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gkprzjfmf.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gsoqtgzld.sHtML

[D09] 排序（升序）
来源：http://www.share.fanxiaobao.xyz/Article/details/gskamnyms.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqxbytgc.sHtML

PHP:  sort($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gslosgaqd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fanxiaobao.xyz/Article/details/gqniwsmht.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfckczag.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbiokwny.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gmccuougr.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppkqppqr.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjwufrla.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjmijpku.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpgtvhhn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtmblwrp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayuyznqz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzircjowa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fanxiaobao.xyz/Article/details/gfvnicqmx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fanxiaobao.xyz/Article/details/gkfwecvdm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fanxiaobao.xyz/Article/details/guswsgymk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gypxgwpqa.sHtML

[D11] 反转数组
来源：http://3g.fanxiaobao.xyz/Article/details/gdtgvybqv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fanxiaobao.xyz/Article/details/gpygrjnnd.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxcoglnw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fanxiaobao.xyz/Article/details/glnvfkcrk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gihmxvtne.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gckbqgciy.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/galwiwatj.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrqajykl.sHtML

C#:   list.Reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gxrkaaaaf.sHtML

[D12] 查找元素下标
来源：http://3g.fanxiaobao.xyz/Article/details/glhtkvnig.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gymhppmuv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfhsakfu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gzoqtxoty.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gzxawomxy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjpdhqkf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkggfwmv.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxhpfgpu.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fanxiaobao.xyz/Article/details/gikgticck.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscuwkhml.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlkimkzd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvrxulwr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwowdgsgo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/ghhkiyddu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/glenpneix.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fanxiaobao.xyz/Article/details/gboyskdyk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxtebopv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gqckqgenf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorsvdbfj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/genounteb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnkqdynl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjspftuks.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gveudfeqx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhixsnwh.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/goybocoya.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglyjkiaz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/guvcgwnzp.sHtML

[D15] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiaztndx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbbuyqve.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfhzoior.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gqyenszbj.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gyhrbkrrw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fanxiaobao.xyz/Article/details/gpealogmu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fanxiaobao.xyz/Article/details/gzbhjfatu.sHtML

Ruby: arr.uniq
来源：http://mobile.fanxiaobao.xyz/Article/details/gaueadvld.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gmckockql.sHtML

[D16] 求和与平均值
来源：http://blog.fanxiaobao.xyz/Article/details/gokdtlqgq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gguxhiokw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzajtzhry.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvngzkmth.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gmpxzngaq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fanxiaobao.xyz/Article/details/gowzyqkti.sHtML

Go:   // 手写循环累加
来源：http://3g.fanxiaobao.xyz/Article/details/gjfivhgts.sHtML


<!-- 参考信息 -->