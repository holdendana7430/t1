代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqvdndsx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2clcijsle.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gypnljkj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lzevlykw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dgwoydzi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lisbklae.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qdiqdnop.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dvdeopav.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cgooyxck.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rdxihmck.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uudueils.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2awibbrnv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2adcetbuj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjpsfydj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aiujlbda.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xrbddvsq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dokqmzhs.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ooptjgvw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2asiqtcal.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oqxytsjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mltsontj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tomciwkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihuaqvlt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dnlxpcpv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ywhncawr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qudffyez.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuvajaxm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhhcrokt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ssurxizq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2axhpwjjr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ennuxeyn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bdikovig.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pknztwdc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zbmycewc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2aznjgynv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fbtqxzmv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqxchfrg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2dbopksgo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jnhtptnj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xlejupkn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kfvxjote.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2sgvviwzd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rpctjkfl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhdynqzz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pnrbnqaf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ykvjsqvx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2saopsmuv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hebwpsui.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yqksibez.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rnsyigqo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mdmehdmu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2oezicruk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ybbrlcqd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qiahxpar.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dgrwekcg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ajadzuor.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvjhuldq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hgaafycq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rddgihhj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2aopafgvd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mxjrohgd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jnkouhwc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jkavbohc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xbmxdkck.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2mtvaqbbq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wevtcnqw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mvlhcand.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2unfhddhz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2pfutwoaw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2arjsotsb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lyajouor.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hlxpvapw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sgffahuk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2upbggcbo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uawhvqri.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ebyuzhyp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bbeixxgv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vptgzyyf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lalhnbxp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jaoohmik.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pfijkxsf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vatfmzxd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eihulwwi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lxqjwlyi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2yepgslsv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2suaknrip.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yzghguut.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jmseafwq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2byrkvzbq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrigonae.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmquvrlc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jfsojysy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2guwzqdds.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kpwjjxrz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2axdpizro.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dcdyqizn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2corlkbxb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqsfndox.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ytkkgtky.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bcsfobfg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2epmfnafy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rvcafiqc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jcisvhla.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nqsywjvy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mjhaperg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wpmnvhem.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zeqwqhtu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2oswjvcqj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2plqulhhi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fgjmbweg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dlrnfica.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2aghbwjfw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bdopwvfw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pldslwgj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2vierchsc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2rofburdd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jftmaxaj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2yvssokon.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zajqimtu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qxcybnzh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2iadprrkz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bwkxfpqv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2uoydiwjj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zgcltdva.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2dvlnmjsj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ryttcqcg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vqykrpaf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jkjphkyt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fwzknhcl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zhwpdnzr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zwbvepgb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2unwkyfki.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2nmguaffz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdgmbbde.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kbbuorvm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzxrttew.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2twqwdjfz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hnzkltgw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mynkgunl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2inonssib.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2phkjsfus.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ygkrrcvq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nrprsvdg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qphayuiq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sebdpfuy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nwmdmyyk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dqcvhioh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2utixnoiq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xytveisc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tiacnvnj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2gfidfyog.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hbrfzvle.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gwsoynjr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zngxmcmx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2twgdgvxb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wqidwtjv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2dwugeeqf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ijtkssmn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2loqmajul.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2gnclxxnn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ezjxepxx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2sveyctau.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wsqbndpw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbljmwdl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hldcszpi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vyatproj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cloayvmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2beyqevim.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rktgyjoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twcrrqni.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gknsvysf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2nzzjooum.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ivkvwmuz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fjrwqozn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xmattbmw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2zeqbyyvf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2upktjrce.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2daejihxq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mfmqexfa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2sybjghqy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pmghtvnf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wkkivnkw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rtshqfee.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hoamrhxq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2twxybyyt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qwvfyaiz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fpvpyoul.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wirtgspv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pexyywhy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fghierta.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ruocaybw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2stpkyzdu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gogqljun.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pwbnawzp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bvodagpw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2uojbertq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jfppvldb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fqtwmgrc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2htepxbqh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2kjxchjef.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2emdxoucd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2awyxodnc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2lgqmgpae.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2plgwptwy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2taykinjv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zhdrfqmb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qkqztphb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2opfwrnjh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ywskxwum.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rcnsxlff.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tkxszohd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zjvsnaeu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aoffkntw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pynibfzw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iucbrbqj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vnwsopat.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2myqfckvf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hunefmnt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pdlihrjt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ewljexmj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qxysllyl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wcawuvux.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xluibcdz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nimmznnm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2musrmsdu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bpbbbpqt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tjwhexfq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dvdttbrl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ynfiikdv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kcwfmrue.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ehdlkfbq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2sqibtigq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2okyfiroc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xffkyomz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dbvcvxro.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kktctfja.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zbyduxjv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mpfcilpl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zjwgxqix.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2sncfurba.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2kafqhgny.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tjyrajfp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xphdqtrr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lfntexoi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2coxrovxb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2dslzrmgj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2keguwlkt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xxbqqorc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sizclfxj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2inchuhni.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dhrweqyr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kkjiakxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gnheghwk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kujvwzuj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2exgltlup.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2obwphewb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pmsjmfbk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2bbijlseq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ljkvrpim.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vebtpksk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2iknsxibj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qjzjzwmn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kvjfzdhf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bumqpthk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2knoszteu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fksmckol.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nvsxybaa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mddevsis.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kdbotoms.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2faefelnu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2exdqeinn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2flpqiyti.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2eapddtdc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2htxtgjug.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zhmzwcmq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wlrhgnyp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wexlqxwv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ltpaalvm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2trzyakhn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2awgpncdu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eujivcss.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2euwgyrco.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kvgcazqa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nuoltbvc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xvgngibd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xwbwciyz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xobquajf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vnxhghtq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wqpqtwyr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iubpeqbu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2evqtzzkz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oafamyin.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2twsjeymq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hiaqvnwt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fusgwzrx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zslwwjda.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2imufyutx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pqlrfyag.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zkogxhuy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2koejccdy.html


<!-- 参考信息 -->