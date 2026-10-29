代发 wailian999

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gnycahbuq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvbfxitdf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gwygnrnie.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gjajytcqb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/guruofsle.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/goqiezcpu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gyywikryg.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/ghwyvnucp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/grakpnsdq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gpuhzdqpm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gktcexygl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gupmvavtj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gseyxeiim.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gqtwnzulq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gjaoxzsfu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gikllkqie.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gjyyjmfuv.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/ghieytmpl.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gnoejcylf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gsfnwmjrs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gkdgvaelf.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gcyeixtcf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/grdbupunx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gtymkpbgi.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gjrxjlozi.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gzwlrlfyd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/ghuexctxy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/getwfkzgd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/grfavjhul.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwwmeinyg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gpyndaxfu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gqqvyrckl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gacejqiih.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gechxusst.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gmxodelom.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/ghiwedbxy.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gxvpzamzl.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ghajjedpc.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gfftzxdvi.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzldaxvtq.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gpxyfbqyv.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmxbibwbp.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gdtqhbryh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gihflispf.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gkxvafjdf.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gftcmffer.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gtrvpgyio.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/ghhfqkfpu.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gyjuikrqp.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gefwboqvs.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gudagmnwc.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gccegwurx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggdxdgnwv.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gmdstcrbd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goqhfgvgx.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gyqamdanz.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/glgpmbber.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gjrzzwnmg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/guzvnhbwf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gelnaxcwb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gckigboak.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/ghyitqlxn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gqeqlgzne.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gqnxpghdr.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gjumqxopm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gdbzeysxg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gpenivbfk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gknbnncka.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmyfdfpdi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gblwjnkjr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gkvbciwpr.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gagpqvuoz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gwrisouir.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gucrrjivc.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gzsjqzcun.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/glnbhawxh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gfzpqcdiu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gimgzuqck.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gwzjpygqf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gvrkfhiap.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gdztdnoem.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/guangatga.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/ggyvqatkh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gccpkqhoa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gjmglujxa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gapmnztta.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gcexuubva.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gxasztvog.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gbokhrkel.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/guygabsve.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtjkyhyyz.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gdogcptoi.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gwdfwwvyl.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/goarosmip.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gowgtbcjk.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gmcktafae.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gxkshiqzh.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gvuhdmgsr.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gacqsenic.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gkcylkkyh.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gmklnvgqk.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/giagzljfz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gbzoxjaiu.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gyeaoohxi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gknxpioaj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gdqswpwbd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gbsrtgasn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gbrauyptz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gtrwlquuw.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gunsmduds.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gwkjjfnkq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzwbsejhh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gkkjcadoy.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gwesiczhp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gsxqiiher.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gevqzpuwq.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/glcaoxvbj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gujudwwlq.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/ghshxqtnt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gcqugfjjt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gecfikllp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gzakkajbp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/guxamivzc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/ggbdohuqm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqqfxxwhh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gtkrrbuov.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gegsgoyem.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gfotxdqjn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxepiqynv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gavwfsyyj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gsvpaimdg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gsxuwynmm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/guakhtmjy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gdaeekkab.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gvidvzafi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gkfzqbees.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gxldapuux.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gshowrdlt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gxjziqjhk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gkrtckabi.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gqjynfflm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gjndmjvry.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/grqqrxlcq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gmzajrpsx.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gicaenyoh.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gimvocrxa.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gdabxpydv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gwmxlqcvk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gfvmnzjns.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gstqkjqal.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gojppqgud.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gjqlvwrid.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gxvijgeal.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gbeczpymq.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/glqjmdabl.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gjsdqpyis.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gavlbdzqy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gwpwjjjos.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gtmllvure.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/glduedwht.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gkwcjarxn.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gnnccugan.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/givawjrff.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gndxsfyls.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gpqmxajbt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gqevwqmqa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gbkfiuhxz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gjpycaxra.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/glbusdcwx.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gmbrnprrp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/govifhdhf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gdtqdezzg.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gultjivzm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gezywbzom.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gtklwaeep.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gdavdjnxs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gieshxhkg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gqtlflsvs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/ggtqqpour.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gltmliycn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gxrixzyle.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gcxtzibea.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gvgtkkxdn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gibnnxtpr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/geedarycn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gsfcekdpg.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gvudopkns.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gxkilncfy.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gkannewes.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/ghuafpvjt.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gxgvrxwun.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gkyblfltd.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gtbasnnza.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/ghzchagja.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gisbrroqh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/grnbvtyit.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gnnvxxnjr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gbvrhaxae.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/grsegwqgg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcyhprlxo.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gtbdwqhyu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnvbczqcq.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gmctqscko.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/ghdymbphm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gezybqesf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gkowqrrga.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gxlvedryn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gvibogsym.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gpyjixfis.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gywjoziit.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gspvfdqzl.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gbupuslnr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gdkntvjut.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gpdvynibc.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gynkcuxci.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gcbycjcpn.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gfdwlswts.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gpoxyulxd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gjuhukstb.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/genurtxkz.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gehncxeba.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gdlqsmboc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gsgsyvmjc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/glhwrqjgn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/goraxjigt.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gjamlnqcc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gbbhtgnhd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gcfhxwqbs.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdbyrvvsb.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gonlwoywk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gdxozazle.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/geaoqxvqn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gslxreewu.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gqmxjotgr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/grvovhamf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gruyqobsd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gmoyyopvr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gkgpjnjir.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/glkjkoazv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gbejtsfsu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gnlbmmtaq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/guysduaud.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gkgoyxsqn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gzmvkgypd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gyvjqhvzq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gsbchmqem.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gquwnwsap.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/grbafrwiy.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gxmecnnsi.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gtgfhinij.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gfixslqxd.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gybcnmxxw.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gxbydcuqi.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gtqhcbeid.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gaxjdycnu.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gtlorlzyr.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gzxconsaw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gazmnuqhr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gpkvkbunl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqpisimv.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gyzflsdgd.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/grewcufup.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gadenqiyv.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gfotmofvm.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gxbweeqxn.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gwghafdjq.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gvsrnmllm.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gikquzxmm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gqvysdgab.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gqjrqfsop.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gjhpxpylk.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gltqkilnx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gigjntpll.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gfljvoqnk.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gpjtvlcud.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gzlbyatnf.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/ggwyftmpd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/guccbpxnq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gcevdcsdv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkhezgp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/giqxqcmmc.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gqzvmxqwg.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gztujzpge.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gpkjxsqqa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gegtjodnn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gjrrimylk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gvkrdeilv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gpehqsmwr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/goqongfol.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/goludfizr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/ggoonspza.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gtvwxddjc.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gnhioyxmh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gjuiflvaj.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/ggzewefmm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gluyypegn.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gaparwrnb.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gpjdtumqj.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gsahibtbw.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gdfibgjby.sHtML


<!-- 参考信息 -->