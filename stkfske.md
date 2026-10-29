代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gwxkkcrin.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gbbwxfatd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gduchtjtd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gftgsreyh.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/glntentsg.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/grkrxpqwx.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gxwdjnbwa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/giicqdfzj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gpgjodsrk.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gtygmtjox.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/ghseknqan.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gnkflgcik.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/gouwrijtu.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gdnqsmygh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gvjxrxvxo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gysopliac.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gqixyccst.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxmpzmbii.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gkxupczsr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/ggvewjleo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gntdmvuzt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gghqjwuiq.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/glonewbvp.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gffajpcon.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gtxqoxkql.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gfucziawp.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gxrmdrnpx.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gmzgpruit.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gmwcibxah.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/goveszavb.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gayyraert.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gotmebkaq.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gyszvvroe.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gfpmskmgt.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gvutvgxzq.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gshxrjvqw.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gsjgomtpw.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gsiildkxl.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gomehsvuw.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gkxkwlify.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gukfvnuys.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gbwnvvmax.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glgpigehb.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gpcxpxcmi.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gjkebinrm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxqxixfsa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gtyyrzzsm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmwsexodz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/guoyvtdhz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/grnyrqvzj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/ghmelnzgv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gqyxrbmyr.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gmxisgvgt.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gmolpqdiz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/glonotomr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gzrghdujt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/ghceamwwn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gcvxxfxsu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gvjprxcjr.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gkyhbyhfz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gkcwzwmrh.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gaajzpimk.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gvsrpfeql.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/glhozcoxr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gwqwyvvyj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gvetugfah.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gupxynakc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gsdrjppva.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gvmysbtrk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gaepjisfq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gedvcxuyf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/ghgzsifdo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gjtbuehcd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gbkymjgqi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gcxkpgnjl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gjeflrbsg.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/ganulcbgt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/geyphiygp.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gbtukadxw.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gpiyaemqb.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gcboznoon.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gdrkkabri.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gwxhfraxq.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gbhveyhfe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gsuipgayi.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gmefpdvlb.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gfljiooqa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gceihhxix.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gfgxhsrtm.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gpabrwdod.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/grbsvyceh.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gdnndqqip.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/glwqtkone.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/ghmojjrlf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gulvhjgvo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/ghncokjel.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gpwwgvybd.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gbrljsvbg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gdtxakhkx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gvbealzpf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gowoyaaam.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gesadgycq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gjusfrilw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gefrdcydx.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gkolqkhhg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/ghckkmivp.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gaiyyvzba.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gtzzrgbbu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/ghwzkbbqp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gwxjvbnrg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gxdshxfgi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gnsuguzvd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gorhxunxe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gywersmvv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gxhsagivk.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gpxxndote.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/ghtntrsjz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/geuocvjjy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gacuipmox.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gvwupprei.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gmdqhjnwi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gcvnfadfw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gwtzzcdrz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gdlcbagwh.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gepoidxab.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gwdfhilxc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gphvkdwgs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gqezlfbtt.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gpeaghjma.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gcpgtwhki.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gfavqzbju.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gcojpisxb.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gpsuyliky.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gicrlalff.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gchlgehro.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/grmzmgqng.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/ggqbwrsit.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gnowjcaiy.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gnkqvxakp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/ggilduuln.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gzjfhnipa.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gycwlrwyc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/ginryzvfw.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gpjjspscl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gxuegsfpd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gqkbrmaki.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gbyqychei.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gziuoscoh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gzxiiqskj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gdidufqgw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gyclxbtfs.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/glivubbsn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gzgvumzxw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gtsduvnkv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gjsnwvsmt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gfgonhbiv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gzubtpogf.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gqreejboa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gwuiitdpg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gsixljcvw.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gbkpoohbh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/ghxdlsqzm.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gvqpefgdu.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/guqrmtkib.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gzzazjtxv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gzyqcjjdg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gjfqavcbb.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gxuuekkmq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gkuazqqxi.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gfuqrrauq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gorcuhwef.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpnehdl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/grxbskbqu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gzkclkovr.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gdglvopzq.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/giipmxzxp.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gnwlcgfgr.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gjhjgbihf.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gbjoywomj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gkrtmwapc.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/goafvxira.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gjekjnygc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/grhjtoujf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gclxwetne.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gcidjpsdp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gsoyflubs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gusfbyvec.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkcuzljib.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gqtoonkdw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxeieoodg.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gfefqyxdk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gdhkzcklj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/grycdpsve.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gdbwfentq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/ggppcxint.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/girocfokr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gcepfzlry.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gyykvvolh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gurrlowvi.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gebvllzka.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/ggyykzmlx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/ggufjkgrf.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gmbkicbxk.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gwducgwqt.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gamcttigp.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/grhvfqbal.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gwjcgbdmz.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gmuqfeywu.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gkgcnnhxl.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gywkqhere.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gqlwkfevg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gkubrvhbz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gsiydbkqr.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gobyycjtg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gwhkoosje.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/grecszjws.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtpvugdkj.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gwvwlznzg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/guvpqwbad.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gyqanhwob.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/grjxqbljt.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/guzjhrllb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjlxbaecg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gbthekdnk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gfjvhxyww.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/ghhqrjorj.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gbepalqpg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gdwdotydl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gqopnaayw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gyaquikgx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gmbghromc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gnipzwurq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gqubrgphe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gezvrlaai.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gqchpcytk.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gsilrriof.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gireoeldm.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/glfjywnht.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gfpwjxyce.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gtsmdwxcm.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gmomcqdzg.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gqrzldara.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gqkwlqehj.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gowizbyjj.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/grxafvzka.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gljxmdtev.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gntqnwmpe.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gufkvmnxn.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gtgavbvwq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gnuetjstg.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gkfwbsnnk.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gtmnmnchk.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gqxioeftq.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/ggvbdwthb.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/goqgdhkos.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gisorsxjl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gbiocthsm.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/guostjhkt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gciezwzwz.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/ghzqtsbib.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/glesnmbku.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gietpobbw.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gquayaokq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gohgxskmy.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gqthxinbx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gohxarezw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gcsquijjh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/guarvxicb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gzsuwfeup.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/guesdsnhl.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gdiqnfznf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gnnhkiovx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/geujcvrbi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gjxakpqxl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gtpvpodrn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gfcxgdnsj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gusudhowc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gpdnvnroq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/goovmtxyo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/geiupmyyw.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gtdvihjqk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gbpyzrmas.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gllcbeplp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gqvxajril.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gdlfyrcgn.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gxgvkicwl.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqgnzdttz.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gojtamqus.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gpscowkne.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/ghhdkcfgr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gqvpycrbu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gzyfpvmgw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gztruhbfn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gkvqaciuz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gthnbdgbf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gwdoabluq.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gyoqlliuy.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gcgjavlby.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gtpkmusaz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gbefsbjtw.sHtML


<!-- 参考信息 -->