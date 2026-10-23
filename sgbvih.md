代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwfokanl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iqfthwbm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3augdfyht.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jgvfcwtk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zklvdnjj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rrbguytm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ysowyrjs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3izfuwhgy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jzttyvuz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nsjwfizd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uteilkiq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ddbkczyv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3toljehog.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgniudmi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vodlusmr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vyuxhset.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qvbclguc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xvfqxetw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3drmbdkgx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3omapokbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdaxnouw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tvgleoyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkfxqphc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rplgvhsd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3clohseig.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hblmsnqd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnwlslgp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zlsaxkwq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlssqowf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3wlycrmun.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3nckkqvvi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3muhqieum.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3joehrleu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uvzaliek.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sebbmjle.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tjmyfzem.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kmdpqivq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3aoodumgd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ycxmxwkf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3knpfqusn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qvhajgnm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ilttguop.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3rtzkzvsq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3eiawekzf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mggcmqiu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3izmyapsl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcejqlaz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3dobepcti.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bzzupvzp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3thdozmjv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3mlzuuxis.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hsmdyzon.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3snnoelyq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxcoggdl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3sngzaqkg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hjdbhxba.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ixfmevbb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3volrufmk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jjitxmcp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3sazfoizs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sjeounxp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xxrqbjaq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mwrixudb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fhmgibjz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3yeuhbovb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oxhytyuz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dlqqhhna.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hmtpzkcf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wttalgrv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bcbdmbyb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3rgszdixk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ekdmpkxt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dwwftjqg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rzmksovq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qklnzsny.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dhrlhcyk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rxxxtxtz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vrzujgfr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vexwnxrt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3amcqzcrv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3onpxhnfi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3vpxebhvq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3mxwzdkmo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3maxmjtct.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3gvswncjc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wamiyfru.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bibklien.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gsjukpin.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmtusnly.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3okzruvrs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nyigophy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nupvcnay.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ixzqquxy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rrcazwxn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mohxrzfm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3egagwvev.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvimiwwy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfhmdawu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fuqqkdoj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jahjwuzz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zvykmdfn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vjinjjsj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3scmpeano.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zyconoqe.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3uztonunk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cmdsrfkp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3niayozss.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ofynbuto.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3uwjthlhi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fwxhuqze.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3svbiyqyz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3kvzujyyo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mtqtctyq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gsoqzohv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fnbwbbrx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dsxyerjw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tzavcmtd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jymjplcv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3mjtykpqz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hgjzdlop.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xxhbzumb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3lcqfnhlz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xtujnbhb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fufydofu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ipnknvfv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hwzwhcxa.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hrkdzwwv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mnkvlyeh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3mflnvtde.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3mccvcsrf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3yfjkxdas.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3btbtwuxd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ioajoxke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oizzkojm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3htlqkagb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bugeqnhb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzsjnyoz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3dzjiitox.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wiavgwhn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3momkicgk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3stnujmpo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fcgvwycb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ilvakwid.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hmetungm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfocyxnj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nsrvrmak.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gohexamk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rcgvrcwb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cwzwhnyi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3wxqyibvf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gfamhkmc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ralvabdy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lpawdrkr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dfoddbjo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gjopcfyj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zvwpfzyc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wxgwtzso.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3thyqnvvv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rmmfuamj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3otedyqek.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3cujfussm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ydfkrtad.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qlisfpjf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbbhidbh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fuctzxjz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3refyxbqy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vxiuzqyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwjrsafo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3jwlexzfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifkkhfdx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3aktqecry.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ppltqqqy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xwsvncqd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kcrintbr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ctjwiyzx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vdtjqvcz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3oxexelbb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3nwrspgvu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3kxhswfdp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cvbyarrr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dauhqxyz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fwqyvnpt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qljbfbxk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oxyoawxe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rdxwrgof.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zijdwztm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3eitcoxgx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3oslfumxk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rwthhxqu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3clrhsijn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zttphfsg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wtkgsuzs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gndtlpar.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3soejcdgk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ibzjeiwr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3azhssdcs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jnhszytu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jbgmcugf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3errkvgyo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ivwcjkxb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3irrefkda.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3eatwosvi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vvxggnvr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ieemsaxy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mozjlyug.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ogezzzjx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hhspmgyl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kvfnmntc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hvqxways.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rgoxwnde.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3zktlrkbh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3howndwsf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3chsvouro.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nfrmlkyj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3shushgts.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3otempzdb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3msyfhtij.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ozizvqio.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dpjgoygn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pbngocjo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bbiqrect.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ulwyoazm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3iudmmglx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3tlpglcrj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ihbcilhy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3rjkkgsow.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jdlcbxxd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rqwsjziw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fhijlksz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wqemeazs.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3imcvnsif.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lodaxhxe.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zzkojwfi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3usonqwcw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3trrospgi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3atljogzt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hbvpcjzk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ccgzaldk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3abmqapho.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dgyapajm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bfoicudm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xjhxilqu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rnmhkluz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3umvylrea.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wvtptyuu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jqmnucxc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ipomxrzt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3nbrmohbe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3oehmxyed.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qxxqbvfx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3yblklbup.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zfuxnwor.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3fxheirmh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3oleapqow.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xnaniexn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lgjmckqy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ufoxatew.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zavuedzl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ydvfwhwc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ykfxeagh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xbuabbwh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3errwuule.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bitbsszl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3dgpovhwb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wdsyhzgk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yjcpixsi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wtpecrhr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qrtxqdwq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rbqwsrgo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3khtvokng.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dtxaliqh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nlrpnmjr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gyqoeczm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vboyjdvx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3whxyfcmz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3blzxgssh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xrqxyazc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3sknkjlsh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pvbgckyx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mpgrnwrv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yobslbbk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rcttjdtv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ffjbgvoa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zfwmbopr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fkgfabti.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gndvbjjf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sycqywvf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hmkorbbh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dtcgnrov.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iydwdqku.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gvgxaynp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlftzyak.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qpxptwpm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xfydxaqn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lpeckeow.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xzfnptuw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qjapoybo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3azvnsnyl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ltodslqe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ukwaugpj.html


<!-- 参考信息 -->