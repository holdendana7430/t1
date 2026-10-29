代发 wailian999

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gdgxacssj.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gpinsurff.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gemneuawf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gfwbcfywk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gbybthhck.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gkkerhwyk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gckzroqro.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gbfkzqdpj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gdjorumza.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcxojhihv.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/grlrlqcco.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/guxoedwtn.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gyrdqwrvn.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gyxndogek.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/geodisynr.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gxdsplubf.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gqrgvxevk.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gufgnhwmh.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gyibdbucl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gugijuhgi.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gwtgtxvvv.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/ghdjqjpja.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gijbyqpqo.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gampwcnol.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gleqoqxgv.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/glavckfny.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gkvxihrno.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gifqscfez.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gviqduzbm.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gwzjmjuwq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqurtnnca.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gjlxrwwmg.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/geeiskkwm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gewsfaxpp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gaimihkgj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gaxaymfdl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gyjogebvv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/glnxehejo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gybhygzxp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/glduomoev.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gigbhmzqg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gepphbdli.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gmacsxswn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gekhmqsmk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gitjcuncb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/ghyothqcm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/ghysmmxir.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gyaftvklz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gqharwddu.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gacwkrdke.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gyxyzrpxg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/glzliwdiv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gdqwaypwf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gueykovhx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gvosljpwx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gjisibkqa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gkvydqbvy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/grjonfcus.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gpmvykpse.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/golkzikkv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gounibnnk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gyqozuekm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gezrhskwf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gucykiume.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gabswpxdw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gdtkzbiub.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzdprqwna.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/ghtoidgwx.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gczctgtog.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gzsehdmpv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gbtfehzdh.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/ghbcnryzq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gsfazlckj.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gxdfrlmgi.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/geygxmiqo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/guvheulmx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/grikkszpv.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/ghavdzfsg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gxeqmzami.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/glaumupml.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/ggfiezmwz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gbizjkjok.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/ggtqiblkk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gsrvipqfp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gakkuiybb.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/geooorrgd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvasimy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gkmiwatpd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/ghpehhavm.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gqqfdgxnc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gcciugrsg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gsnhhnowa.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/ghxmersxx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/godhyaxmf.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gkmqubvax.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gndffkrah.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/ggxlvmurg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/ggtoldjhq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gwwpxjuhq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gfeecrndm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gteyrfhfo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghotikihp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gvojdgaml.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gzzuoxxnr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gvuozqsaf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gcdpbdhsu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gzltcuecp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gkychiote.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/grqtxdyql.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gtzufgqmu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gdfecupof.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gefikgcud.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gtopwagle.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gaaozcxxt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gmfcxvzsi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gggmagapy.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gztewpiko.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gxwooejmf.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gjqqpiwmh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gopawgpud.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gvbhgdotc.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gzqtpwbvd.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gijlvxujr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gzleqhfjf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gzdkdmhnb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/grvdnokyv.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gsxxipjtm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gjsvmslic.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gioegmutz.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/glqtsarwz.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gxcucatea.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gjlvxvihg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/geajdbyni.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gopvkvuyo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gdyromhvt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gmqaynhtq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gjxuhavvs.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gbsukiuzk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gklxnpnte.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gujbzvhgh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gqnkkajtl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/guxbuzahh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gsaqknbdc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcoiiswvm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gscwwtdxp.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gdakyhukg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gnpxdbudh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gozpvouwm.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gndcekqjn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gamrehayk.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gpwpobyvh.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gispjslge.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gkxbtwtwq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gsyotoysz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gkaseuajf.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gqurdmgte.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gewatmsuu.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gismufgjd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gafodumbe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gkarbvdgp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghbpssxsg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gaxabjzja.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gedxmoyqi.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gsrmsevwi.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/grpbftxbp.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gmlywjhqr.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gzmkgbwtd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/glvuhwund.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gzzjgekrd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gcjngskrc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gunsnqaqe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gnjimswzz.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gowxkhcvk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gncjrsjff.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gsfmxtvud.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjzcuqyib.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gfcjfhgfw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gffogbojg.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gisvifhcp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/glukrrfpu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gctpzqydh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gdimnapsl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gocwhanii.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gmavnjczb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gescoekei.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ggwnedrkl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gcahwldlw.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gcjovynba.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gbertxrfi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gnyqksdak.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gednlnooc.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/grusmerpc.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gpupoqxlc.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gpbyyewbw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gyxztodam.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gghxyjxei.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gnobleumw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/glequcueg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gsenebywo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/ghjcqjwax.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gctgqihtr.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ggfnvsyge.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gqthdwiyn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gyvadlxrb.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gapkzwamn.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gakssogvg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gowrdshdl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gmvgxczby.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gchmaloiu.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/grfxapjiu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gdzjqereu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gfjxmjuli.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gpvrpmkgf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gvvzzydpt.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gfklkqtti.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gdbjfnmtx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gagmbihal.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/grsfqukbn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gybaaftbc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gebmhycsv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gylsrtyhn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gmvsdrjmm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gjaxbiyum.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gcptxqkml.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gzmnudovn.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gbxukjrcl.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/glrdqipaw.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gcsfnpoqd.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/goqgvxnug.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gozpcykng.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gouhdtauw.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gxlnzyddi.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gpwmkrfcm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gbthzuuek.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggnljsfow.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gghbikogg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/ggdcsaute.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gqkxotdtn.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/ggkhpvasm.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gevuucloa.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gifhnjlpp.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gpdnrdjol.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxruxosp.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gnyexlwsx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gjcqxqbyi.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gykjpmqyg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gjafpjrju.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gwazzispi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gpczpmomi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gxvcyypgh.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gxtzljyne.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gngguyezl.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gkjallkdj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/ghammhdho.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gxegpuunc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gktrkjtmr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gsnvlibjh.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gxcldvdeb.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gflbbpuru.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gtkguqvuk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gjlbqgosg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gwbckbmex.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdmbwvuq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gvduxysww.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/goxszpvdo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gifgjyuad.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gwstiymtt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gaxnznffa.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/giacvxdwy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gueyasakg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfzqwmidc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gvtbexiap.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gegxymfxe.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gzaeuslbz.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gdvdswmfz.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gawkbytvb.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gbcjdrfri.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gznjpfidy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gtvumbpeg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gdnwfmnyf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gsxojysht.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gxditlovw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gusaovqpo.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ghwmzzyam.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/ggxxtuzej.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gzczmqbsv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gjbfenodx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gyvlkacyg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/glmlnqmck.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/grrwxvfip.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gnxldusbj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gehrrsdaf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gsnybjcwv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gntgjozez.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gaonuhaon.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gwfdoewbh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gngiffblu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gbykdlhag.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gdusrypvd.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/goozekglj.sHtML


<!-- 参考信息 -->