代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gmcrpevnt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gxtjfkhor.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gwahkycgp.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/glkwilwos.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gqjdtzhox.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gtoyotzht.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/giuovkvjk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/ggciuxatd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gcmlediyv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gkyenecqe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gdsrkeyug.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gegrzebrx.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gdojinqni.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gczfissgs.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/giwsmknin.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gdjryyfmo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/grpxncrsw.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gvgvasnmq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/goaydllqe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gcuxpplzr.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gmrxsvrmt.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gmhfpezsp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/govudxaze.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gsscrnwxt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gluxycbec.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gccoaobqd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gmnuyisvr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gufuczyox.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gqrelrbny.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gizaxbtbu.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gmhfpsyvr.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gzleksjer.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/guagzppcf.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gdroxatwb.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gsujmdvxi.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gctxwynuy.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gyeotexdg.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/ggvdlxhhi.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gwhjrbimw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gndjzhuiq.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gpunlkrhj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/galgjexqw.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gvsstllod.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/geinpvfos.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gfgnqasou.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/ghlwdvdym.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/govwejxxt.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gvdihovno.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxfutkjuf.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gtrsjvvgw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxvpkewuf.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gqfxdilyq.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gnnlnnrqg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gusftrnbg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gevbxnsde.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ggqkrusmh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gukzmpobm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gyozmvmaw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/grnuyzvcq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/glfyjprru.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gyjeyrhpe.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/guwmaqpbe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/giyvuvmyq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gxmridfue.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gimigzbnq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gdnwteaun.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gnlebtgnc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gixcwhevi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gfspyolmg.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gftjlzqkt.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gbttirwjw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gryavjltd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gwijxkyvs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gbhorocjg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gfupmfrrn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gdwabpenl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gzjabcngz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gzbkexytl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gdhgkwezr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gzimyigwh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gfdfvsbch.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmzhyjcdu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/grwevekpt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gjudymqnt.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gngznotqx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gtcbmhiip.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gazdrsjra.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gfidwxicp.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/glhztxsif.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gykiixyia.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gkhouwjlp.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gymusiarn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gomurzwgk.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gxatkdwat.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gxdihotlm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gshyatiog.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/ghqpwhgsj.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/ggkopwdgp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gphtyycvd.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gdqgigoql.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gbipxdjbl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gclliiwri.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gckpiigfb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/geaqcopmj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gvsrlsfwp.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gpgmlldhj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gqxzlufwd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gixtvsxho.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gvrgkorja.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gbgozwgzh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gppjaincr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gkdvubplw.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gzkfgqqtn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gancwdsge.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gqharithk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gyuelsxsl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gkcauirpw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gzhzhplyo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gevpiprmc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gaivyhimp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gagjuuhmr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/ghjkuqaxp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gncnlgkdi.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gctptpdnd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/groszbfbw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gwieylxlc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gkjxyytrm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gmmividos.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gvxyrzzfw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gtwppuual.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gdgadzkeb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gdsstgjat.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/goaroudkr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gsvoddzro.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gmoqiqoxo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gwicehcbu.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gycosgvhe.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/grgnatqve.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/guephqipk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gxvyhlnlf.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gjiudkynk.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gextvsjkm.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gbghdbifl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gtblcobjz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gsbzxnhyh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gkidwzxoh.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/ggxxmtjos.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gjttairnj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gndmmqeje.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gkdnhcgtx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/ggrapxdrn.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gdgrfckvn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gjnbiayfl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gmloppwrc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gclpcthij.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gdtdnexxd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gksqblisv.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gffolagff.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gmttyuktt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gdtikvfsi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gdbhdlaqw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gxdtirorn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/glvtjjrmp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxoncbnzb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gtznyhnap.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gogtscxmw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/ghbechold.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/geccvhshe.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gnxxvuscw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gvcecspag.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gxfgfybrc.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gjbwhsxod.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gxydvwbhf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/ghoiszkxg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gusndkhbh.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/goldkrmrr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gvbrdhgsf.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gitbqycsz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/greluigco.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/glphjihxt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gykdllwzy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkapcoqmm.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gztcansmp.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gvpfzvenl.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gcaotjana.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gyffnrhvh.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/ggacpyybg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/getrtbqyc.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/guniolpzg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gaxipgmlx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gmysiyxzk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gjamfmzpu.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gzfmjkwhe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gkcpcnqaf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gqxnywzol.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzaqgzcbm.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gfmxacolg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkbmgsygp.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gtkxuuxgc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gczhohpms.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/goqvpvhqt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gxupjhofk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gmulemlbw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gnsxvrfsy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gndtuaobo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gxmxtzlie.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/ggdzmurdm.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/ghdsnqwrn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gprjwtsvk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gnbnxqljk.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gjcqcklvd.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gpdjwprff.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gghfdgtnl.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gvckejlee.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gvnoqreeg.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gxvqrgobw.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gfdhnyxvk.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gjwvowbzm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gkcgqvdpw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gowpdskjj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gqrkrfbgu.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gtimhijyp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gbbqgijtm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gfodlqqfo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gtjmcbisy.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/guzdcplrk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gqrjqdvai.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gbquiykrr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gtxyankbe.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gdbnwdezf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gspgmhnpf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/glrcnyrln.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gjknvikes.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gvguhrlzf.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gxdauhwtd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gclncrezf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gvvmbgpat.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gzshbqcyz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gfjjmvbzz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/grckvzmln.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gcugdjczn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gyroanwod.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gywocseur.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gjkrwpmxz.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gusvtqamb.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/ggrlcznmj.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gfpjoliuv.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gdqloyyav.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gloiewluw.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gwaicgwya.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gacgewkmn.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gkqnkvpbd.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gqrpdruts.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gozkifzwd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/goimplxzc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gvfccxvzf.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gxwfxokpw.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ghvnslrum.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gatperlkp.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gsxnfpasc.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gpjgzivfv.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gvannmgyf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gauobzzwn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gxttxwxix.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/golrkkdeo.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gushqxuvz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gbvqqorhn.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/ghtgddunu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gvrxnspcr.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gblmrutit.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gmwlefzpk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gxeuuqsks.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gktoonwbs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gngjysytm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwomeoaw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gylqnjlix.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjhdacrvj.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gulxephzp.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gdchsqbci.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/goalgyqsl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gqyirgyzi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gnkgvfmhl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/goapzourr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvojmqsb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gvbtvqrnv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gfqmycolf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gxfqgqyva.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gdmztkcld.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gmwzgcxdc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gzqcpfozp.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gqkmkrfdi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gyifzdyin.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gajoqdszk.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gahkldqtc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/giwrkrugu.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtjiyqftc.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gcougoecy.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gulibybwr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gmiptbzfb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gjrrodijy.sHtML


<!-- 参考信息 -->