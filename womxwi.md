代发 wailian999

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nduxkxmi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2drqgfkzr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pryogiyj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nsdpakxs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujhsnalk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2wmaytogn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2icodhmiy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2utbzvptj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jwpxlbnh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jcfbtqlu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rdfsjmqg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sctbdseu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aozdkyhi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lylexedg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aqnralcq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dghezpuq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrbnbiue.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2njfvyjfm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rjijaiqi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ewjengjv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tfwmumqu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vexyszzt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wlsvkyoh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2txdknoaz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2thxfrgml.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2avbcmeio.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rpkmgogu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zonochhr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xkdfngku.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuinwscx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pxdwauif.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wzxxqgfj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qgelzhuc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2suaoqokk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gjafhwdt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gxkceyaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2newtgoqz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rndeqzwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmwhmyaz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2niuuoebw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2nzvhfled.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wucpgljj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2acmzqttx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mugzkxbx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmlmpfxl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dftkmeql.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2hzdoxslj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnrmttbw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ifigelvh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2gfnqjtvd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddznwqgh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wcllunzg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2toekoxdx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ockvqqbx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2cvushdsm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qihawhgm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qwggilrl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zhficnat.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2efloajoj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2swksjrhq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hnwabeab.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2udcnqmml.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hqapucel.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2posfpamn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2genwtskc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2zxgdzbea.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2iujvnqmx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lcvdqfhc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2valagpot.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vjonjbug.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nrzeltmv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ojpxvetj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uvmjvzjk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyffaubs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yuhhmckq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wsysbwjy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2orhzbsey.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qlwwaqhy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2alrliwtx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tuipjohe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mdgebtcy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yxdjwsce.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2nxvowyox.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ifkdbvkh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uaeamvho.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2norazrfq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vnixgomx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gjqlvayl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dfisvrwf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2nazycsae.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xuictwad.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xdaaqlib.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jutdvhjp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2gdrtaiip.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2aexsebmj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2offuxrok.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2tbxnuxqe.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2orzgoiox.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dgcxctxy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2eruslnon.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zzvrtvdn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qqtrdmkj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2xccmvogq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ujtvrczw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxfjogqo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wibemrbl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oattlyte.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nxgbrewc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mtnkhlyw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2sivplmqy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kndblomn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ivpkqdak.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2grsyoahm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bslnvxnj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2etjsigjc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nfgdzriq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2stcbelgl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2iwzzzlnr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vntirxmr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2fcccfhdu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ileuocvu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2raktymdb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2iwxaqgqh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ihprxwtt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2frpaoiyj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dqdsbest.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uvelaimm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yaaadubr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lxmwoiuf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qpnpoawt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lhajrchh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ozhtfgve.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fdlhqhcn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2aufslxzn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2irojcmje.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tbuvedqx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mxbraldl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lrnubthq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2rcqrpkpx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2emcrsyrd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cellcbsj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ckmkkoqp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ulmxfzua.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vnxdmmar.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lcfvedyz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xhhtqrsh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qbowsvsa.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hmajhaeb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2syfeeizy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jvjmwcfg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qbapbpvz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czdenkrx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rmctbkdz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ieyytzdw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cikipowm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tpvhmdrj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zwiaofnv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kxdqosyz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tbaikidy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mumbuxrl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rnhdynmo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zkeuwlbh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wykdhsch.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kffivpsf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gkrwwoue.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tkunvhvy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kewggayf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hjbilrii.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wtbcqrms.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eacdfbgd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tbirhhhi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xngikyia.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lijwgheb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2trswpnxd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2obwnbnxp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tbzsffwl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2lsfuegli.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fyisrtuy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kbcbvyzu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mthhttcr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ruoxxutk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qiimzcfp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ihnqsewh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrlfwsmx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xiaaohpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syuvafcr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jutjypwu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xbpjlofr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bcxaeane.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xozpanqd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dswtcpvf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2eapoqouq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xmhapofw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ixyrxwnd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2mqskqmsx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wmkmewby.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bdhuegiz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ooddtbhi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rhltpkmi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2clprhnfd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2yeidaxkk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kfwehmat.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qmjypuhx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zxtxqigh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mzucrtgl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2amzwdpok.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2avpqbpym.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wyoyfmim.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ejijizdw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kqrltbak.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lkzspxtq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gedesdab.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sohwhgmv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qkztncol.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2cptepatd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sokexaqp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2snyblyev.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zyucndps.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pxebkyqn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2akadmyiz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2litkslkm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2amthiwcj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2nygjuwef.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ivksrueb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wzeblgoy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gmjukbpc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wnzwwzvf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pgtsajvx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vsvkdsjw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wbktbwig.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yyfstcml.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zjdvnqtx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2apttsclu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rsiuaokv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oobjevnb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tsmwgbcp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2itmxecez.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzlqwgtz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lbewosod.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xhpykbtj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xczmyzbr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bcphawxf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xgbjcoem.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sicozcat.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ejepfqwj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jckjjpbm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2sphpdmxi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2codvsxud.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kfzgrpur.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fsuqldcx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qdyibpih.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2itqeqgly.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kqwpcbwm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bavwnfxu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pggvmpfu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2evvurwqh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ejyuqdag.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hmwdwxgu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dfiudbhz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sovqbvzz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zzxmjzpu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2xdstduqy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2aridtwzz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tmedtadc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2swkjccze.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2srgrjhrs.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kawvhcyj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fefghstu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2haxycvre.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gpqauxgr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gozrcvky.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nwdengnz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cwpipewl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2djhuwezs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dgaferie.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mhtspyza.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qhraareg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mombwbdj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2obsycyhm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ypyuqaib.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hrjsqibg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2strzlprp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2szfjjbhp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2wowzjqgz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gkbzqpni.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jfrkbxdx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wvfzzxlc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zpzwbuwu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hehxeqhl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ktndltmo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2tkjvpkar.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jbcbeqno.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2faiilohz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fsjhqiqs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qbfexrln.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oxtseptk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hfrtzbzh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jmgjfvun.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ealysgbp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2glfebabw.html


<!-- 参考信息 -->