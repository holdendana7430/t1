代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wtojokcv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2krlkndiq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ahqzfhbk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywvgdemx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yloanisk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mowqibfl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2haqjpwnv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2loroamwz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhooddbb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ovvapnqq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzazhfwe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcsqxcic.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiwixbax.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2dvdefjfw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2nnilhlxe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2spvwojpu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2cteddimt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2omsbxttq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2dqdxzvxh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2eigahvzi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucvhznzp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtsyrlyi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tzxvqqfn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jzyycfgs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ozjgyedw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bulholdm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2mdcrzpue.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2didntroz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2cgesjmot.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uelsaslc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wdzkuksb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2txbwjcym.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ugwzdjso.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zkknsrpo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxyfahsw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2exohhuap.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dlwhglxh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xulpvrfr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2htmhbmcq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tdtrkjwz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2oyppurjt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tqgzcwgr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ozxqvznx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hwmxfmaq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2klrhclea.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xseqclac.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2flhxdzqm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vzhtugxh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lwuedcva.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oaquiyra.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qmrdrkqs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wkdkftxx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2odepbdzy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mbwnazhd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2fpemsapi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sxomabaw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2iurnfpld.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cssdskxz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mgvblrgk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2fxjvgbmf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rofvwbyz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2bqmruxns.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2dfcswuas.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tldsffkw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2drhznrof.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wketybnf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oxtaatvf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mmbhbxxg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lrpxewrn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xiegvmbo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sijtsvon.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2uvheonqw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksqxfjjw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2woxcphpt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vwnbjrvp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jtsbbops.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2drfuqigf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2sfrlfmzr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iulpjkrp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xhmzfwxt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ngbehdht.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qynrtlqr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zykbehta.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2keydpnhv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vasiuvaj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rbttqvbm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vzfxsduz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2hwvdrbtg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mdopakpt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2mxuaseyk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fzeukcxz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ieikgzoq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2arqjoxvg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mcfuztfb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2dlbfcsfx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2yuppqlce.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2aypvbxxk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rdqhmbxr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2mjlyious.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dsduzfbx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dmgvcjzd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tacfdeyu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2emntmqdo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ogdxdhrh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xfioumzp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2szzhwsdu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wkxbhnaz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2oykhausw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2clagttau.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qipmdnrp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ixsftagu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqsactsy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fmgszefl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2yqoyycdr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mbttamrm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rzpdwptg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ktvcmqql.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2fsbfeqnl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kexpafum.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vorwfzxg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftfejuqr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2cncmpqqw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qdjkvnyu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xmzariih.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tinhbyqx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tkukicgl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kksfaryf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ytqgrwgr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nummabnn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxyfjexz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ybcengaz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bmgkqwbr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wlcuflvb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hbeiknyb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rostaidv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2trkudhje.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gngqzwdr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rxdanxuh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2qpvaxzmj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bldmgjjg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2tiglxoxw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpxzpsak.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wytfsnqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewmchgzd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zfcoedxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhizcwcp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ddypxomi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zrkzbqtn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kqqvofyl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rwyiwdll.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mjngbpft.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2lempkcxa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2krukkipt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rroqruyg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2bqwhqgvw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xqtlnzzh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yaglczql.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2akehhioh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kqpudqqe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qgpnqvoi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gkacyeec.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bqfkqtwq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2unqfqvkd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jzjeskba.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xyhorysc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2smtyfnsb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pcycmmxa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2sseswzoj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mfrazrwe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2turkfnyc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iisrfehv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gejolpps.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dlhnhuou.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kucucwct.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2maydnvqw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2cslspizh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jtzonchq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hwbkfbhp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jxtmofss.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tmyhaxxa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cmunpkkb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qrswpaxf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qxieopqw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qflytlqx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cpuztkdh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2omcwmwpx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kolulpbu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2bayaaxqf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jtjmoalr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2igfbzqqd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wrppwrva.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kncbylbx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aibnnyzm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tsijzbbd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bvbnvyvg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xymcaomf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2tuwwzvoh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2knojysvo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jehhskli.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fckicaot.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2woohowch.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2abutfksu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cnxbrlwe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ccepqcpb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vrrcdwob.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yevhdzsq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wzkcpqqc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2flmvbmdg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fksyfjdz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pqehwymr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zktjnsrw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dbpbgcjr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yikwusjg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2phkptbpa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qcijxtzo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmelzpa.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2znlgdhok.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lygycjqg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2trqwnain.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oqcjkzwy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cibbouyf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2srydhlsy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2snnfggnt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2akqhzqyr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wixxkcsj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yiversht.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ohtgigax.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2oizirqnv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zgktysyp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2psesmgbm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ycxafods.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2drclhzbm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ytyufpcl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2juoyjwdz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2addyaydh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xgoxnatd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2uqpthgyo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2duoeevkq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jwjyuczn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2itnwrdyu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zscekvgc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yfpwgefu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vivpablm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2suudbpvf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jjwzwcte.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gnowlhys.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ptsnjtfn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qytlrwic.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2opohduil.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zakcjihz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2yllxhxlb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2secdsvsq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbbhlxnw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xoxhbqpa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ivtmbpsc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lfcklsdi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ksdnfdkp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pbllwgrs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cpgsxcnu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pmsymaxn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xzoldpoy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2oopbbqiw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hsnwfstq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ctpvpnjq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bnhsvzjd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2brzwnmrh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2knzkfsge.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bqexbywj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ohxpauxs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2awyltcly.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ptouofbn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gebqltrh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2aqtkilyy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mkkmgzda.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wtclymbb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tlicjxit.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hmojmmpn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wcfpitfo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2uvmvonmg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lgcvxtyl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jglwjuwb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bokrofwn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ltxukfuv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qtwkcngm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tgmfrsrx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uytmpacl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2krsffprg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ixjdexcx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kskqpxbn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pxotjjpx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hxpedopj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkpekbrs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2tzcaaehz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bunkohma.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2leeeqszh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lzfrdktk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fdtpppxp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2cehbnorg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bmlqfjdx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2bixqspwt.html


<!-- 参考信息 -->