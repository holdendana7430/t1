代发 wailian999

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/grpgyzior.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gtynycekm.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gnpdxsrhb.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gpoenmazd.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gqsadbmyi.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gxapkkwpl.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/garzehskh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gvslnwyjh.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gmmzgpwkh.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gvvrfdorx.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/ggovohoud.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gwzxjesfc.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gfaluqnzc.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gturfvqzp.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/guksnsmse.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/grvsgmusy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfoemzatn.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/gttyggngv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcmvivrsl.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gzutnimto.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gfseepznd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gschgoyvf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmhetqwvk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gnllmqckv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gnwgeciji.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gyrklrnva.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gwbjvgvty.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gixnmqvle.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gsrogycra.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gimamkrjp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gqxmllbjz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gzhonzedp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsyjxfsrl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gdjwptbuy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gazejierq.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gswwjxooi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gbjzpvvle.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gndqiliuh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gcphtdzla.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gzczcpors.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gmncpzmbi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gpeyjtlep.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gazduhhbd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gzvfuukyl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/ggkkuutzk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/ggkelohgz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gimsmmruc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gkqtbeckr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gstfvbjga.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gvgibqfnn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gmyrrobjn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gudgxtlzm.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gulpovxek.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gpenvwmvp.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gxopyfhto.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/guovnmrok.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gxjarvcoe.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gstovtaez.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/ghpfkhwbv.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/grqvremqq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gmzutjqyt.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gynzoslkq.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gwyjxgxvt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gsnbjzafd.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gtojmccvc.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gyduskwyn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/giuenzyza.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gitoqlwzl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gwsoptpua.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gxauactax.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/geapppkjv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gyohjasnw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gukdsnauf.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gfxcghreq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gffalqrvd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gzgztddfb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gzmyuruyx.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gqmqhbvsw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtktbplrn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/glpsypahy.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/glvygwiio.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gntotfkdz.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gmdbjcdfe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gbffxioun.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gxghssjxq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gtmkzsvpo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gktxktrac.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gjkhnquux.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gzficsdcc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gskmfnpvc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/glsogpcbt.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gtdxnecqd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gyizfzutu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gwgigmeej.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gxidjbbzn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gkomeqonu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gkifazkjr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gvctecjlq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gpctwbbfl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gfosslqkp.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gqspfjctq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/grxunfuaq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gjsmnpckv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gzujvbbto.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gklcusrpl.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gszjnkdmh.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/goaazpgkh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gvpglkwme.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/geeyakcta.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gckhtzcjo.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gwmdqapex.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gwoaqulrc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/glrompjds.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/ghczuclxn.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gasjvfdsi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gmhvttsnd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/godfgndxf.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gpbjecmjx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gveiokdar.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gnrnyksem.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gachqexhh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/glbnknxhs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gemcempjg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gmnwxaprf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gvdcxkjok.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gzpraogcr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gxadstpru.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/guvghegmn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gmoikuijl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gfhuxuflg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gmesmlzsp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gyhhzvxvp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ggxdfqpil.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gfspgujpm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/godmrhdfs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/guvnpjlzy.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gnjgkjjat.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gtodrpbhi.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gycoiqiwn.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/ggwfdjvdm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkismhlrf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gshcuwpuw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gfmgfcsgi.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gixdedqja.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gjwoqdowa.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/guyxscizb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gtmmsxhwg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gwynjkxzj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gcryyugxp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gtgmtooqn.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gssuiiclt.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gopzuropm.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gemfteviy.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gmdoeuzwg.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gsmmfvprx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gwbpcxzny.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gfnblwfdy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gltrztzsd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/ghbtbjxoi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gqyizktou.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gxkqhwbbf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/ghrjtyomf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gfwdcbfmr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggzttggcx.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gzuswjpus.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glmqsziec.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/ghfbgmzqg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gvjucsfch.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/grnlvsegc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/ghfnzlvyl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/geswcjdbm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gzbdyqohm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gjbgsurhp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gljrsdyoz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gvlnulwnr.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/ghbtduhkz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gxzdxqtga.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gwggrstth.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gkqsyoplo.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/ghieurvme.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gnrfabtdf.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gwkdxzink.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gljrehreu.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gaqidkyof.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gqkrkugaq.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gydxqgpiw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gjbjknubw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gkdqycawp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gscagotnc.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gqjyfqzwr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gmrpyvkhh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gbwknxfrk.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gmkmvhwmo.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/ggrqzcrdc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gfnednflq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gtpxfgcer.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gclwpkuqh.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gojpzwnyu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gmdsqnprq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gnjzssatg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gbfapeqpm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gorxclaye.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwyqyotgg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gsewzyypi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gjvmovlwc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gcqwhzcqh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gtndouxiy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/ghqihqvxu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gbftovchm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gwrshhylt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gjyqlykvt.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gaggbdovc.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gdaatocrj.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmsetwxbp.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gczobkhdz.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gmoemhycw.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gaifztndv.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gzeopsazi.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gxpxtnwtf.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gyumorald.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/ghdxkzmgk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gbwrdxsdz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gdriwikpl.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gmynuwxuw.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ggpkusqwr.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gphtubxam.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/goftdglze.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gygfsfcbv.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gzeyljvzi.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gdwkskzgv.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/ghfoehjkp.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gpkbjupby.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/goydfrcfj.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gtinofowb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gehhqxioh.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gthclfhpw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gotbtjafw.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gvqlefhqr.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gqvqpexan.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gwxghrysw.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gwzrblcty.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gscvqqrbm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gyakuoete.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gtiugrxet.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gkdapveff.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gjjeyccvz.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gaborfpby.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/ghlbluxgi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gzwdjwecz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gesrypjal.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gcridkjhx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gokxsxmkc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gjmqlefey.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gwnuoluyh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gjkpzeszy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gonrytgwf.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gglwsdnqr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/glzataate.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gzyqolfyt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gxcefejqq.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gdyeikfum.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gnnceplls.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gexcpphfs.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gguudljwx.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gynruarwp.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/galcwzfwc.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gihlqyvws.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gtxdejuyc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gppknkhkq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gmncfmiru.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gwhsttegi.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdgteporf.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gbbjfqlax.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gglxixwsw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gvmhdknqa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gelgoynzu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gdxdnimma.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/goprkmsmk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/godxsyway.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gtwbndwux.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gbulwyzxb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gnwuadani.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gfkfimmxe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/glhalydzj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gckmeikvw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gqkxqrubt.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gbwktgjlc.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gcdokwrov.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gxvyqylci.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gfpcuibiz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/ghbfyiebx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gpyjuwrlc.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gdaawarfd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/giyodrfej.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gcayrntkz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gsxuclbys.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gkagaoavm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/ghopxuuzu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gitcomvcr.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gtzpbecrx.sHtML


<!-- 参考信息 -->