代发 wailian999

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/ggjqppdic.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gxixedpbr.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gweqbmtlv.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ghaobeemj.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/glhmhytvg.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gigisesqm.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gqctioioj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/ghlqiecgh.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gcxircvdb.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gxoocljjq.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gokjnnzaz.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gtpibxqtj.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gvjhosmnt.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gyruxaydd.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/grxpufqmo.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gqklytlbb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcdmxvhmc.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gmpiswqst.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geysygvam.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gurfyvhsr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gfjcyszhv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gxcttpwjf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/galqpqybh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/glavnzwom.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gfwwvhnxn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gpgzcxpmt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gxuwkwbjh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gervzaoez.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gzxdvtxzh.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gkyllugjm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/guxrshtde.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gzxcfquji.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gtlwhnfxe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gtqnlxoqi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/ghxswkcvo.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gslthziaw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gjdregwwm.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gkukpzngj.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gndcskhup.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gqoqfjsae.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gvbuvuwnb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/geqcccesj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gnscpnizz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gqtcifbyq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gmoxpghay.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gqrjqjytk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gsthrhgyx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gynsufnsc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gmvbiqgoa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gwcrcujbv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/guaumcizn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/girugknzu.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gpqubvvea.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvdaxpqja.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gwjpnlwfi.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gwghvpdry.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gwezhhymu.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/ghqamihix.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gmosaszmj.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/guvmynuxq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/ggdsrrddv.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gcrrmvckm.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/ggcelmxja.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gijyvppnf.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gurhgayax.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gxhzomznt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gvrmreezw.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gdhslaccu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gqkizqgrb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gytfdqqba.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gzmwzitaj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gvmvybitx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gqtnkxhaa.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gofxgxvfa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/glxvfsboi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gswkcdadx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gbzqqfbll.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/grqmkhyde.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gbeagrhlr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gpjhbxgwm.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gutuxggio.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/goyewfvmq.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gsnoaanyt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gqknzobmb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gxjkffxpk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gvqoyohev.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gcsrskvur.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gftowlbwa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gxuqiualm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gwkmwzkyh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gzyszowkl.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gwzxystyq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqelyzfbj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gmdsfwcea.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gjepusjdn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gbrumwjed.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/ggrvbuvgv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gkdutyxsu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gonpecupf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/grbqlhaww.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gtcxiworg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gipmzrxkd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/guqmoxbnj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gdaovawgv.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gbdbzphlo.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggkbbserk.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gamdmhfel.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gsdgujpgc.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gwtssasod.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gjbcevqej.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gsjnxfcaa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gbdjorsiy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/geesijkrw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gyngqtgrv.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gpspreurb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gqfjjydkx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gkcsipgio.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gtybbqpix.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gdvbcqoxg.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gggovclpp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gmrayrsps.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/grnnuinrz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gypfhkxfv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gcfkmyxmh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gbzedsjzy.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gaozpptco.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gyqidqxvd.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gagwwuyzj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gdtcyblgg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/ggxoyalke.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gabofirfq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gxafhbjgl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gaggaafhs.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gjzdobuzn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gpjbzatsc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gtglqzkix.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/garzcpqpf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gxfpmgwkt.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gagsqtveu.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gjonueksz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gfdwepjgr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/golvfswsv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gvcgdubph.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gobfnlhqa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gxzbpiyls.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gwtkcahwm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gtrfzijyp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gbhnngetv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/ggtkuvggd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gehedeego.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gtcayvygr.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gqoocvinv.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gywbpimpg.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gyodipqfn.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gociuswuo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gifgvyxaa.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gpcmhuoyi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gvwfdxufj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gmzqffikt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gwlbsibqq.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gywlsekpy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gcyrnqnnw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gphvvruqr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghzylspuf.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gxpmqpadh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gowzdhoka.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gigsmvyze.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gtzncrmlc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/ghikgkxwo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gkoaxyzsp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gwhuvmehe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gkiaalhdn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gspsiodzb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/ggzalqpmg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gkgsdysci.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gxpbfvdgs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gqdeptakj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gtbytbeqa.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/grkvexdhz.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gbypbewcy.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gzhmgglqg.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gwzfnymav.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gzxhazfpl.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/ggvzwofto.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/ggbxdwtyc.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gugxuasvo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/guzmdbilg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gdehkvokh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gcbawlapq.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gvsolnvjr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gnxpfyoru.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gvcieaihg.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gzsorxlmh.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gixogwwpa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gnhnwuffn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqkedtwde.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gwshcgiln.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gaeicezfb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gutqgkjmy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gjjzkddpq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gotixxwai.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gnfppnrbq.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gawvuynqi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gyktewqxi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gapuussgj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/grsgkzhnt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/grkququon.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gjefrxqen.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/grsgaubnv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gcswqvoqf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gpgnenbhx.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/ghjqtypyh.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gkchjgace.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gboarroba.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gyoflqjrs.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/guykbtzzx.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/ggbhscnpr.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gshqkllsz.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/ghoxdetll.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/ghlutuger.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gagibzvfm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gawvqqjsl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxzbyzgfp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/grjbyenwm.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gdnxyfssb.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gztarpbkt.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/ghzzdxsqc.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gxdpwfjup.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/guggnnbok.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gdpgnssck.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gwhlwkxid.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/ghwnmzdgy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gurgobfzh.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gemscwbjc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gxtakvpua.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gcfckptgv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gbtsferfc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gnvrktcrm.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gixxhvljj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gqevdoelz.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grviukkie.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/guirdbuys.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gysotfwiy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gcblgtsua.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gtsvzvfyk.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gplngqbum.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gidluxihm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gobhwjxzi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gzkctcosc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gglfdiule.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/giztvvxfp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gjkfudnyd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gfitwbqqw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gecepuvbo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gsrycaxdt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gijaaeztu.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gkuxcctmn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gdjnkzgin.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gldyinbco.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gdzerhmwk.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gigewjkgz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/ggepdqbym.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/geoppywgo.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gisijunmd.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gtzzkzaju.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/ggceasgft.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gvgfgrdsd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gpjulbmas.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gmpdgegtp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gkemeucab.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gzxocyecz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gclutjpvv.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gzhlfhdev.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gcuskoqai.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gstnrxozw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gfqrscldq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gjokwtaoo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gsvbvcnik.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gmimvlkko.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gyqqigfsq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gacmqdypi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gaqfeolgw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gehrmimcn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/giilpfuct.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gwelbumjq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/ggxibubqn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/ggwnrsbqi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ggoojbwhy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gswzkdffh.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gmawexcll.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gizzcqypj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gtxkhsyux.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gxrqlhgpj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gmxymmtlg.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjmmthclz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gujatcisp.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gisgfjxhp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gvtavrncu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gvyhdqiwj.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/grinirfsy.sHtML


<!-- 参考信息 -->