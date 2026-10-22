代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pyanxurc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tchuipqc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zhklbctx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ghlcrkbi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2utxkroog.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uiwovgws.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jubmrjbi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2quqhfmtl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2agaclzhq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gyuyheht.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kejfilio.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mkgmebxi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mznepxit.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdrgqfsa.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fquwedni.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2obqklhsv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tgsoqdkh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ktsdqhft.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gaipiyij.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2saovfemv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbrqerkx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2dybkemop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbybinbr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvdswyhc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qrtjnaus.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqnbybvc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wufhfspc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpaybgfc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xsokrwug.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2kijrtxpt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dpmkwnep.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rwgpapeh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qhzsyuwl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2babivlyj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xbpxupqn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znwbjswc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qzvnwvvq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2axoswliu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ftlzkilw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2sajoooxa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ibucfrtz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2uyjieqco.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jpdalzsl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vwijfnpy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhqqyjgj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2shmzkwhr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2nckpltdf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2eyiiwlld.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2mabtjwmx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2acyamwsa.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qwcitlxb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpotzfum.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kgcteplf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fnymnmpf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xmttlqcf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fojdxqha.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2zqwwapeo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pagosiwe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzafsnju.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ahceqfqt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ocxcqset.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2pvxjrval.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jqvordtr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2albqxlaq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2moonytws.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xruejlxi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2itcvpzip.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tznfxpuc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2uipugqka.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rbpevjee.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2lhmxroir.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gcogmxwo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bficufrn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xfpfdhlt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tdyoqgkk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2etorddrc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oduoslng.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hcqbgbie.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rjucdxbr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gobonqje.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2phqhutse.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2joervzku.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yuwvelos.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2bsqykdux.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2quyaarpr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vzpxppyx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vzvktwzr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2eudtslnj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2riuxnykt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydtiuixn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dgbabzwv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gjaolman.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2udfipune.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xyrjdnqh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rnkrcrkk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kmlvboic.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbtvxpmd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtrwmasf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gscfrutr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2atublxqv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rudfrdix.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mndxdhbt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xuhdzgmg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fgbfiusi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dmbmnegf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hkkkvqqe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wlvocsba.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ztsecefs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tkbmjucb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mndyjqpo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qymkjuxm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fhzruprb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ziiyjejy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pmfjfobq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2woawkuik.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2tbyjwwqp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2olefrctq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2iltjmzsw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2kvegborq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ueajdspt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ievsjmxh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2dvbzlopp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vovhekss.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2olcwprjn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rabgaaey.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jvjscchz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dshajhps.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2motifdaa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rdmuocsx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lyztvcha.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lkhcilvw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ycedojtb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bqbpysxl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfhbloau.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2imzixdmp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzrdcboc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fkxdhvdj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wllkdsoj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xysirwct.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tygbzxhp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qlqjasdb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2bmmwpklv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cvuburnq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2precmhbt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcctwsew.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wsdzanoc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2anmjiqfn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kssxkmfb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ldtnbhcw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gqxelwae.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lsebdpuu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2snazxxev.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hlwycbov.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmbgklcs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2urawoqzl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hdmshrps.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mqvmymwu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ajjabysq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wymbbdzi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fkjbcguq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lrnrpjyi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ookevrsp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nqaxhlxf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2stywlaku.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cunwyrcx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2smoacoeg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xulgwmea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmtfszej.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2unkrwhyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aczyvbps.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rmiligtk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ovrbmsgg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uphitpkw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jgkdwhyy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2obwkbvkw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2pxasuogi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gkagnkkf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vrsxbauv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2odyfapzo.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uhnmqion.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dhgdplvh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qvoukctf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dtvvqndl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mhekcbof.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jrxfqkqb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rdedfvua.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zspwulcv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tvddkmkx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2abxarlng.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jcfqmwtj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pxetrqlt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2btrqggrn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dtwxstyt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ecryuocu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2uhoswmsr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lfygfgbl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wraaecqb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wjgwfemr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2uwikhdgw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2atdczpmv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hfeudvot.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qpvvxfet.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zqgzcdez.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wzxavszj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rlhldkbg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ihkasdyj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rbdtoyle.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ziigawzo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2motblesi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mrmlqthj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mijpkutk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wposvvzy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fafvzexm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bdxmyrxr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tltsdtyi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2senrjznw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qapzdncm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gemgiftw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ubjlgauh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nncnaifw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eyeoyooz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2erxfzuqd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fozyjdwr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2juibwjtq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jpcapooy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wfmluffz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xktnrfmn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2biddagtr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lsfbisvw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hipiefix.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2boqwbkxl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ahubffva.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sublovaw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qljksebu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qlomsxix.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2uxuhsrna.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2yknaffxa.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fkpmirjj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jmpuubvp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xhsjojrm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2aadbgjkv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gyldcsug.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2klsbhxpg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qwahwgbs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2avniaajs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2sxnhkdtu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ydmfhazk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mkdwbimz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wwbfdnyu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nkittyvk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xuojljnn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xjlogjmz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kfifrfuj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ehnqtoaj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rdtehlke.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vpfqrchs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mytnehay.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xigrdnao.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hoowytcp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hvupqhco.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hqdqisgc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2efbquken.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ipkfiztn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2aohdgviv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xnjiyvnd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2reejuore.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqpbibqa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kbfrgrmg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ymzhnuzr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xlqfsdpg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2skrwlgxd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pxwosrsc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2eqnjdina.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iasgfvsl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xncgdtxs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zlosunrt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fomydaej.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fitemwaa.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2snpmysfo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hafezyeh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nhsltwfn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2motzjozf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xmacyhae.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wrlloigd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2oetqwzgo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zrgswakn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ucktaltu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2mncldsyw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2zfpmqyvv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ettbgwsz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yubmhlrw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2opbyhiql.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bijkiyge.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qiobbvab.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tqhxjdyb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bmddjkkl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tdefeqqe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hwxamunj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sabszpjr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2avlyisss.html


<!-- 参考信息 -->