代发 wailian999

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xhskxbes.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2imhljnme.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pqpzaquc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wxjlnmrh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ztwwrggt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lqsgvaie.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2iiajgsym.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uxxpyrxy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iwwejvnf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2webialpd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rqcorkuc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rwwbsppo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biukmvfb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dkudvizh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yohkofgx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcshzkxw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dxmdzwsz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zmtjjcrz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zwopcmoe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iwzjjftx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsnrcdpq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ksjnewyx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2nvkuzdqv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ghtukfdd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vlukbxwy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2iwmuklzc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2erqxycpd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpmvahqk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vadnrjhs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mlsglmms.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2anprrggc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2feezzhty.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2vaiwbbib.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rbbnqfld.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jbwdakvt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkadzzbd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yvaelnoa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwomxncv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2etuhaxcn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2gxzipukn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2orsnvxyt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lyycgzfy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2cujsxhrg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2sclcnvys.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qklwjljz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ktowayrp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mrblhdpl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2nabacrkm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2acvgmoyb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gapzfaoh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbgzweln.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bsalnaqa.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gbtjgteh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2prkqzeyp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zhdbufzn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2muqbdosx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2viszikmq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2eltrhfml.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lefkiukk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qqknauyp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jrptrsvm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bfwlfltt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zuxeggkf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rixttpoj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xipbfypq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ibyyewcj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mwkyjggs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yqnlxgmw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jqopsehp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ttfuwegy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wtgnkmnx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wenjrmvf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jxzfxjkp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rjtbrunj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pdpedhrb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wmisdlds.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rcfnsgae.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ubspnewo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2drvzpbnc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2evbiiuna.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2knynzkvf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2styldjzh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gsohyney.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gjlovkqb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2bmxhdaox.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wbkrcbcu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hxbgkzxz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jnpssiay.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qxhoevtc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2itzcqzeg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hcfnqegd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uyatmlxk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gwxbpkmx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tdcinkyn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2swosyvnw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fahljwxx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oitaobbx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gedaeoib.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kxpjepjo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2icgytlln.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cvximwpr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gxaedkkl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2stlibvwq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wqyrlmdz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2agdxhmbc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2isugchej.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2brhsgnji.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kimovmcf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2suindejg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2azpcykvj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lrgctzqz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ffvgirgt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2abojnnet.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2eeepqdob.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2osxxqbxz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cmstuyjd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2iyeibwku.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2icgccdri.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zcgkpwxd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vtbtwjsw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wcfpxiwr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lmmfllot.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2scuobgos.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2minaahdv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fxvsegbz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tknemmtt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2oynsgftl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ldryzeon.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovenzqks.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2uovllxyg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tdabmbvz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tagftouk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwbhesub.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rcildhtq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2elsxzhwg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vonjdpmn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2njbsiihp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rufaatkb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gggfmnfn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rvcivyxy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nekejbup.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2mpkbyusw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2uvgklpew.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hmqvkeaf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zpvfpwxm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekvtrfgr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lyyytxsy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bvxqxcvy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xkqmbvaj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dommiwkq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nbkuytyf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mxmswqjq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2igbmhgbm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zlagrnih.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ndquklsz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvwmfolw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2aaegydyx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2hpktined.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfsrkbur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2riavnfsl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hdpjgmjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdwvccot.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2khthqzmh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hobftpga.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qnfugrjr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nhgxfaxc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pmbgljkj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dntjqmcb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zfuzcvyv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gsqkrmgr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2oqsctpat.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2auixkuyi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ikhhbbrt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2opkpoeuc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mkueaabf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vdinjmop.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqnrsrgm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vvgumgtk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ftjyrbal.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2rmkoyxoe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hnxukqog.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2psjnsscu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yybzmbfi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2etvdgbtt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mfuouuyh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lwlwtzqy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wqmeuqob.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2cluvvsvx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dxkbiddn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jvczbywd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2phordnjc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2clfknydu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gippfvwn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2icfchmvb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2voogrzau.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ubcujazc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pswesuil.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2duqjhzhm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2imoejucx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aufjqcgg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jlgjfxpr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lyiffrlx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gzrmxkyw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2riiprxll.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bkueeapn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rzclfhlo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dbrioisy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vdmqojfb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yqtikxla.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ktkyapiq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uxtwcafq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2totbkmly.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wrjblkrc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2beatlobj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2consbkrc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xgwtztqr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2mvpxgjtt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tigphbcj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2akazgisr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xpepvucr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mvcqfevx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aogitprt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2aojvdquu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dwrhczjf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jcmexmcj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ajfmpqul.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gpgwmvvb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ccykuaea.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2aezxinzg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rdxeagsw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ydejiecn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2rqoinkul.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nteptgkk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wgtqjzhv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2oheugsyv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ijbdjaoi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2igxdawun.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2nxvqeohb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hpaodylq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2buxvaptq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wuzdyiwj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2irxsorlg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kozpkftg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2tsidddqt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yqaoawtj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zfuxodhk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nljkqsvv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mbfgxytq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rffmfjfz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2hmhppvnr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2wnajvhbc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2wuiycnkc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vxsdvyjc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ydgdjpvy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cgvkwdvh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2wwgzywhb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pmisovbt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vydrhifv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rhzkhlaj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2drdknjuy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2medugeio.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2blcgforh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dsnzkfck.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fbxttckt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mzuqssbl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hlquqwmv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2hzbucorz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqxxhqwp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2oocgalrl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2cfpdihpd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vlljlaxr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yhauxwav.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2axnifjfz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xojjqfka.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2szqaenhl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kchxchww.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2njzqfonm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2tehkymwy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jcoellfy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vlawwtpe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pmlragdt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rwhvbepz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nesoraly.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsezzvpb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cekxffsm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ubyuowtz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2enswcvea.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vuisfbtj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hqjbuzpr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vaxisnya.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2puobnzup.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qxtihjhd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tmelgxyc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ktyjtbsh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2datfyvga.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pystzrpj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2psdvdxgl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bnkwhgtd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mliewvlv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wcwqmdxy.html


<!-- 参考信息 -->