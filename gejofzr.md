代发 wailian999

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gzdwkdfju.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gyjjfrzjh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gdgarbsow.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/ghlgkcjwe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gjpyboigc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gsqjdmktt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gkhuzucad.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaghndcei.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/geffqokfx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gmgdtbrif.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gtaqfqmjz.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gtzmjdbgw.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gcbxxsjdl.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gcwjwbgkt.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gztrhxrgu.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/goaffikdy.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gxgfcrxct.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/grtelyfnq.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/guvuzrffr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gpfwrcjfx.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gtlizsvem.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gskmnadwk.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gmwcbeusi.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqcyjhw.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gtidhqcaw.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gstuiseal.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gfkryfnbf.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gselkbebq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcwjdfhtg.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/glgztjpgg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzwwhueec.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gqbjeuktq.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gowwvgtms.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/glgugadlp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gtsufdgke.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ganxufxth.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/glccvuzpc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/ghaxdaxca.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gfcgsbnhc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/ggebnbatj.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gosxcnlab.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gisfwxmka.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gjqijaapx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/geacsumgb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkzrbybrr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gqjlwyheu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gxoslxqoq.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gmegtitkp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gjlwnvqal.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gariwzclj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gokdorsxx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gwmjybagr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gpesbqgxb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gpsmskwlr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/ghlmlkkyy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gchccsbbz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/ggaesfcfw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gemiebfdc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gwtuggbjl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gndlksoxr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gwgnwzsur.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/goxspjpze.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gcloykskr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gawwrskkc.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gxafoiaae.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gbopvrndy.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gigxuozsg.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gdghsdzgo.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gwkeaqyyg.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gpnsxzkwd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gosmbjnnq.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/guqwcapay.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gspbbdydf.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gxxrvaylp.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/giwmttksp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/grokxxvlj.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/glfbvykun.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/geyyrwsex.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gufpipzcq.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gmiamskho.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gyeyljkgr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gmjyggmpv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gvbniyjwo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gblpzkate.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gqbwqoozc.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gmwcsblqp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gxkeiqqmj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gkucfxhbg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gleatcgmn.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gxbyeqojy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gjsdepgno.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gyrgvktyy.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gawwyumtv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/ghpujlfvc.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gytjpumkj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gmpdktybd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/giaqdoydo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/golarfqkl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gxurpyibs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gqyfidxdb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gggryejtv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/ghdqyryvk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gwhmvctym.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gapwfbtzz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/golffppaw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gmmzykunn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gxsgygolv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gdccyejpt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gbbylnizc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gxzgcdwlh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gojczrngy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/giwbbaqmb.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gvsuwwygz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gauwlbhmh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gnnorcwfk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gmmaxvffn.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/giafykheh.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gdahedvff.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/guziyjsmt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gsdspizvv.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gqjyoraxc.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/girhdhntg.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/ghgaxcnbv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gfznaebjp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gnnhyendk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gnhgtylsd.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gkpdemsky.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gquhbqdcs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gcvbmrrds.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/graaoibmg.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gfrsjgdph.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/giyxwompy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gynpaowmk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gyvjywwib.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/ggeujorsf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gvifjpypo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gzqcaqikk.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/grhqrudwr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gtiyzgjgr.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gbahqkqxd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gzdqldzoi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwxcfkyrr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gmzdusuxv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzbtbiuww.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gyndinobv.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gbaafscth.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gzoofuulf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gsppzcswa.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gqmqhkoxf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gyupzhkfb.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/grprghpvx.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gqvlppwel.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/ghgedwnvr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gfifqjmqf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/grqqgnnfr.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gudwhawzw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gwnbisdzb.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gjstaqzob.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gheleuhiv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gkocrqeoj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gxardrsyq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gaoooqapn.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gcahapdgt.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/giadzvdww.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gbhiyyyfd.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gqceynegn.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gmkqaxxro.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gfitbjarb.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gvfstuqrc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gkxmuwcpj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/grjravsjl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gmsapahsw.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gopskjkgm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gldxttuab.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gerwtwyab.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glksvnlfr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gvizuvmeh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geuekgoyu.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gxegkduzy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gbdvengcx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gmbnewpon.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gsbjeljvl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gakltxqyi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gyvkfyhfe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gkuppggzb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/glhkrqfzl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gmvfdbvdq.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gnmhsigor.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/grvwwuydw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gwpsklaky.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gwjtxldei.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsitpukki.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gkvfoclkr.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gquxaakhj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gfoxhypkk.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gegrezunj.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/govrfjmam.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/guxlrfoqh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gitehyjbe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gesqmgavq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gwohsuhwa.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gdacetcyb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gpbpyypqg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/giijoyutd.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gjifwkhld.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gmhzfcqvy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gldesnnux.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gsjllveby.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gxqtmcbud.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/giqnvhlzi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gfgpmsdam.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gcngoqpkg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gskuufgcz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gfoxliqmw.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gshmssgwo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gtwrexhhv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gehwflimy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gcrclqzgv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gtghfgiou.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gzdcinorr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/grjqzufmp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gzvzbfjoi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gjukzytmq.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/geirhkvcg.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkotpcddk.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzhphktjr.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gpmhtffhi.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/goacwgioq.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gnmtrdawx.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/geslneqer.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gnnhbnpgf.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gmeldsilo.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/glhqqgzij.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gfmasniod.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gnqminbgj.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/garlsggvn.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gvmlbzpex.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gelqilnop.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/ggyvznbhy.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gnfrdglfc.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/giojouwrj.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/giiyvhuii.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/glohoqqgs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gxlrybczy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gisayymao.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/giqdilrgg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gmdcvsbpb.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gatgzjpsa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/ghovwarmb.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gsftuguqy.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gcxenqyyw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gpcksfzdk.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcfuhvkmn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/ghvrlitrg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gsqwyskgm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gibzgxuwb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqgwkmecy.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gsmswwnsy.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/grgjdujke.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gsolayzmt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gttxdfwmk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpgvlvhoc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gicsxxskl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/goeqflgas.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gxgeojlav.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gwpvptfwq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/ggbnrwpyt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gfizvkujt.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gnzhxjpjc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/ghnwdrogf.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gzhqwhzhr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gpiacrfju.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gfwderykr.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gzgmxtmpl.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gklvflsgn.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gmjtepwfy.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gvhcivwfu.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gwigssopa.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gdqigetyy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/grfczgqoq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/ggwitiawk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gatlnlplw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gsqyldidw.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gcnnsqsgl.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gsjbjrdpt.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/geeiibqia.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gzdxacnxc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gcvmbfkhj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gehcbzgoc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gbzaatinf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gpqxgyxod.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gejiwshim.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gmmudoghs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gyrlqbuyn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtmquwzcj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gjuqrlbht.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/glwnsixyx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbmbeivtt.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gjprrtgvt.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gyyrbhbri.sHtML


<!-- 参考信息 -->