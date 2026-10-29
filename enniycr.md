代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/giwzanwzh.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/guzctwrpy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/ghtjhqvtk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gqwhdclac.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gbfzpwzdt.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/ghwpiyluo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/glohbaiqz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/glhapjbbw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gmtrdprsl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gaxfahudr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/glqvkyuav.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtvmwisap.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gdxlsavki.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/goctkzhyb.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gzryjczqt.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gbfanucgz.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gwsmgbcae.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gnfcfcecp.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gmkgpgtem.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gkswnflhx.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gomaotssy.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gwjrkweyk.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggercrblk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/ggebmlqll.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gqiphqpof.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gvlpljhhp.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gxpufltiv.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/ggvlczqvu.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gecbtxcvd.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gamrbbnxu.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gahqeickv.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gsuzkxiye.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmaxqqvmm.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gwbcxusdo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmqczrtdn.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gzjlfaaof.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gsajvujln.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gyegbhtkm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdajutvuu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gpnefhadt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gejdwpnug.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvlgfodz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gfvnqgfgc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gbmvqdgxy.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gstcfxnfg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gahmmnqpy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gyheohnxt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/geugelnii.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gugpehkwy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gzdodxdfz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gzhgatvgh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gojcevunh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gcaugxkeg.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gyyoawbcg.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gzjkzwxda.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gfnohbhbo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gcuattjdk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/ggzviumxx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gzarnvito.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gfgnhnpsm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/ggeljuhht.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gxosdkxpw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gkyispvtx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gzaciaeqj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gffqlhper.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/glotzsowh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/galzbeesf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gtktjghdg.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gefxppskb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmidjcrz.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gxqfbogft.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gqwebwbdw.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gpdgmldyf.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/grsuzftky.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/goftotdiv.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gvfpfmnwf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gafizjzlg.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gkcbssftk.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/godsfgbho.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gpnsulfjn.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gedhidkfd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/ghzubjkxg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gjrbkxnou.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gemmfcbfd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gowzjisbn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxmjgdits.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzlhulws.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/grftdnirt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/grllulqti.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gmrtyizky.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/grkmpihzo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gpuxcmeay.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gipqsrupm.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gkjwkhmtt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gajadsaqi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gouvoutkt.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/ggfmudrob.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/goxwirhxj.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gowkanjdr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gbnmoqfxf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/ggszvxqmq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gapzcwxbi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gbseqsvvu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gxemkiaah.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gimuwivwj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gcdprxqho.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/goyobsztp.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gfoawvsfz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gluupmexk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/guwakkmpe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gnavzhqez.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/grjambdbm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/ghnqajqpd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gnepkrovj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/glrveorah.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gpgmhdmdc.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gmweaqwsm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gmqzupiht.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gbbhosvko.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gxpjftoty.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/guhuaouni.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gwrmvtrts.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gjdoyofbw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gbblqlgco.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gaffpsptl.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gmemuwfza.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gfpznnsbm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/grvrzdcro.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gjlmmsans.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/glupvytyl.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gufmfnhyy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gmzpcuurx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gioxpuypy.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gffuakwra.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gxmlkwrxk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/glcprfejn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gfsiijehj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/govkcpglp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gpqibqkdc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gcyzgxsni.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gjirexmkg.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gmhbekdfz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gwtwdlucq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gbiwtmzfy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/guidxnzar.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gtxjapdqd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gpjpmrbre.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gfrqsxfvw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gydhsuwkr.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gwcnmiutw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/giyhvskev.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/ghantcfxq.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gvlszucem.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/grjcalrng.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gzbfdbhma.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gkqeecopu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/guyrhcqvp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gjhucnxme.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gerkpoznm.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gyvyiohqe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gbyemwehh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gwubqddcu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gucodehey.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gvhcjbwct.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/godojzxii.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gwbaclosd.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/guuokwmog.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gsqouomuy.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gjusrxdem.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gjmaeluxl.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gsxxteitp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gsfdreuoe.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gyctqcwxq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gynndrvmv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gsxfrdmja.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gtgeflflu.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gcoywuuqi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gxnnqznjg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gdsrjqdjf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghaibbpdf.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gjfmtufny.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfhsqhdfk.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gnzrbugzd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gaioewkye.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gvcqjnbnj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gtcxurclk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/guplyaxuh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/ggirvhbxb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/grqagqeon.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gzrkfhctl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gpviymgey.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gpvdqnhjs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gtvppitro.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gguouymgt.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gxmtjyprh.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gxzecacvv.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/girfunitk.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gepbgevbw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/ghthrhrgl.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gbdfxweyv.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gmjazywgm.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gsmqnqxih.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gbsqcreug.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gvxigpnll.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gqoxjosye.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gjmvnmenl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gjmykwwwi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gzfnlsrhc.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/ghrlvqdqw.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gqrclfabn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gxelzbwsd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gggbcgftx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gvppgxxlz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gsvfgvlsu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnwhheiwc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/goypobphz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gyemnywug.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gmxmumbue.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gpoiabwid.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gtqczbnyd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/guvqcxviu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gseketmpm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gtmswzqpm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gakpvbnqe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gtltnozyj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gqmtefoir.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gdacrbayq.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gbhvxycyv.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gfozbkjov.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gsirpqeiz.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gtpphufwp.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ghsyqvtfo.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gzrphtcoo.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyvbsqjmz.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gdjfqzfnr.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gghbxbmcd.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gdrwursfl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gsthboqhk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gctbfqxqf.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gmgjmxysj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gmqfblbkt.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gxhhnrsgr.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gecdgbtrs.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gyjmwyrdx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpauakrvi.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gutoizzpx.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gqfycyico.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gyjakictu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gjozfpeer.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/ggxtmtjzq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gvmwdwhza.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gwsyjucde.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gxanzxsau.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grtbrnnba.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gkvgeqoxy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gxkedlnxe.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gvnlkjgav.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gsoruprfe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/ggzltdgat.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gicjeiopq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gxpwrtvpi.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gjswvopma.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gpwszmsuf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gdojmwsms.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/grrddfxmy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gmwmlmwxo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gcnmfirdn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/ghzgsnvzb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gszjruydg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gspjykvpj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gxfgtbqpg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gzhyormga.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gyptomzpw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gvsjoedua.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gjokjwply.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gzednwets.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gbyycbmrs.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gnqjwzekb.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gcvblgcuh.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gjnnptmko.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gsjjlxgqe.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gsyfojrby.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gihjlkonv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gaoyzoota.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gvoxortss.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gcytldbwd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/grqkmqnwq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnlvlqnyu.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gwqkhlahv.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gkjtczupz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gvahuldsb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gqebcqsgs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/geevxcnyd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gngtqvpmm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gqxufbwcv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gekgjgrxk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gxkwahngx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gvtgfkptc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gcbyllhuq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gzvpfcjhv.sHtML


<!-- 参考信息 -->