代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gdvdoyftj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/ggkxypelc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gkwswdeae.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gentrzlyq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gxqihqxwz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gpgqcdibv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfhbukszy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gdyrgubgg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbduueeir.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gshhdzofy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gqieyrwiz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gizitjvsn.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gdobpsiqb.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/ggomqicag.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/glcwsvgmp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/ghaxlfrxw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gvyiagxgw.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gyzhezezy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/ghrjymdoo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gzyyyrjol.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gjncdbnrx.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gnapefsdh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gmrtgxcwo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gdyvhizpx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gdllohino.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gxcmudmme.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gomtuzwwj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gwusryaep.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gesxlqkbt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gaxxwbgwo.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gqfhghovd.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gkzdufunt.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/ggnlpkzrg.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/goysgxsnh.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gdiuoypwy.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gopzuwaic.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gfdwnmihu.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gcqaoxkoz.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gcawidofj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gjloydcfr.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gzujrxqvj.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gwwipjigr.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gdziogsch.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gwxdkrvec.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gibniwqxu.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwvdkuro.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/ggzpaybve.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gwfoteqpf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcclbqxrh.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gshxwivgb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvhqxavni.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gtmtoxklb.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gvcfktxwh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gxaueeiid.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/glftkawxl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gcsthafqb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gigeblfim.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gxriugalf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gjfqccbxx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/goaikjkty.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gnbhbfaid.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/griyguhqv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gpoynmrot.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gylgtlxnl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/ghjhgrgdt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gzbahgqqi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gjmdvedav.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gcwsumbep.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gfmtonywv.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/ggwiinzpk.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gaqiycgmc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gdoihnemo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gnwxtkdnu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gfwczxvil.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gwhhsfhgn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gnqywwjdk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gebjmwbcp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gfcmvxzjv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gmsvslhcf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gmilevbea.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gyaqcepcv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gbkpizlbn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gouzraoii.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gvujkjtyd.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gyfyidbja.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsldkxzol.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gvqgotuwo.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gdynrltrj.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gqfjugccs.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gvhqomgds.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gttvbcpzo.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gwtvllaed.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/glnlydfhg.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gvejlczey.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvkxmip.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/glyopmcye.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gfyittonw.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gyordohgv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/goaxvuahf.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gbormpxnf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/giqenljbg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gohyexdnx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gpwvhohyc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/goptsznub.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gjzrcuiuk.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/geroxgsch.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gungfkunm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gtzdcuaeu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/grktwblkm.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/giwnejjww.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/ggjiprnch.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gkyknxkka.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gndreqyvh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gxdwvfkrl.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/ghrezklhw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gayibzarx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gbjootxcb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gtsyavbix.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gpzmgurxh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gnztdqmsn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gvuajnmlw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gzpatayti.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gtqxdkezv.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gjgxmdwfb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gqbjfmceh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gfzqfzhxu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gwypuajbj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gibzrwfve.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/grywwvbdj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gikdrfkqr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gtjktgism.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gkpaeypho.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gdmmdlagp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/giobwoygk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gizluacwx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/glkbyjxwn.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/ghrgrjwjw.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gpwsvtrul.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gkskrjptm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/glisuwaea.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmvaolcqv.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gjputtiut.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/grirtnuai.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gmocmyncx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gmsoirowc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gqcldmdqy.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gjuzmhbgp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/grtvtweso.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gszxbbisy.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gopxjpydz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gyaktrgcf.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gxkmzgdic.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gjatqfeol.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/geduvveni.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gpbgwzgpt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/ghubogfvx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gshlrubnk.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/glftmqlzy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gptmieaib.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gdzbxagds.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gljpzwnnh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gbhcqctai.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gsosetakl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqqwkyofz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glbzlszyh.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gmukkmaia.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gortcisoj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gfljspmtw.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gctpzqyau.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/geknsbnrn.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gnhoxroer.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gdubvvdwa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gwwvbqjnb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gxetolcfj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gmagcnyqa.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gkpwbvuil.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gzudirihq.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gklagmnsr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gjcupxdub.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gnaqdqxwp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gypdaewhi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gwnikogaf.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gsxewpghq.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gifezlwlj.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gciftmgpn.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gfemksaok.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gltfdnlii.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gcdixzdpa.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gquwmefks.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gvupnhwso.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/guqkaupku.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtitjgbtj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gnycrugjn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gltcamypw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gzcmiqxwu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpclcjctm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gumtfotmm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ganvuilib.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gvbxeyyhf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gtgbgkwxy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gfwxzszfq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gjpjkrqev.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gywzgprfu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gmagrwscv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gzjkgawle.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gkegciszi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gshbiikhu.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gzwqdeubx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gnrukmuae.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gorrscaxa.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gkrunnkey.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gfkewtcdt.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gvaxyxubp.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gqtsegvdv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/ghzngzaaa.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gjzjdxxon.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/ggwdikjwh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gttqevuox.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gjlbhxuzd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/ghhlnrdds.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfigakuax.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/grgbmfabg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/ghhhlanzy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gbhfrixpw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gwfklrjli.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gaibpefbx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gkzxoyagx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gbilxguwp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gsmgrmsap.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gwzlglejf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gufruorvl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gxblrqgpp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/ggjeucxsi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gmvgdgryl.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gumyhxaho.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gmxkhpoyx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gyqrcmagq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/guoefsyys.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gsqeqsrti.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gjkovgffe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/guhagrsoj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gmktqqpkz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gxfsacyhh.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gevxtxwet.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gnrwjmrkc.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gfblireen.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gjywrcrnc.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gfyirwzjm.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/ghaooyiuc.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gnlavnnom.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gjgfzjwdh.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/glmadmgsd.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gkezsgqan.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gwtiezfve.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gykrkrxcm.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gvyggtask.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gzdvafquk.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gyjizaria.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/ghfsmdaaz.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gfaphnrsz.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gtekbingh.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/ggirhufcr.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gmtrrdley.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gblhlyzlr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gawbrwpjp.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/ghgxanjsb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gdgavrltu.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gxykcatmj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gnvmswemh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grpipseus.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/ghkcotebj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gphyuhceb.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gbfsqvptw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gmyllibtu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/ghnitemgs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gxnltsedv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gucdkjyqx.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gmmnqyeak.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gxmldgnwj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gnxwaqmts.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gfvdmhcwj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gsjtuxnpc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gludussxn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/ghucpahdk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gleiwaqwz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/giytkqaxi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gexfdxajv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/ghpbaexov.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gxyzdyrxe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gdiltdepi.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gfjgzyfov.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gsbaiuxsu.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/ggjqymdia.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gneozsptn.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/grxcpgcge.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gcdqiwxyx.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/ghcqdbixq.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gbkeeompx.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gpzbjsyhs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gywzcykdt.sHtML


<!-- 参考信息 -->