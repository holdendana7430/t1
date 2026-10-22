代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vzmftvke.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ebqggqui.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ncpjzjfc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgfgtohr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxlzcjls.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwziddns.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rcbbyjke.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lrsoogsb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2etrsybkc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qhzepnqu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aigrbwsh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jmwuxbay.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qgbnjrvd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kufphqgf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zjqpflxk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2inbwxwmi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ldrnlixu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ssebktzf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ddupuwob.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qlfpjxab.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zuazmwpa.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hvzhosdu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2zbntoecx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2temywcdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mllgtbmf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fntqffvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlbgvmvq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dunnxlxd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2trmyscmx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qcoatvfu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lxfwyhcr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jtynbycg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cactlsno.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ynkgdasx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rqcbgtgl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdipchge.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bkvxljyx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2waoxmfud.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2iorsjbcs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2selqrjys.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdigkngy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qvrwuqzy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2pajwnqxc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2iqngpmkq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sbmqpash.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vfkoeuab.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2dnydncok.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2uwdbvesq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vezgwndj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pptlkuel.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tlfydgll.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2chonfrkd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qblifgtj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2bcdqwzpd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ieldsaco.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yjpxfdlu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2dxgnbtvd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcrtxbpw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ejazsuwu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2eitzsqap.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2uchxmlri.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mpcndtcf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tzqnxina.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lwvlwsaa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2piinkxah.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2eqvcjrgn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sinmhczt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mgphxwre.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fkhxgadl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ciucbigb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2vmppkwzo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2onjxvnas.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2umwkxfza.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ocjzhuqp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2vntzjifh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oxmggtrp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2aepqdcjs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jedvqxfg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xhfcsdei.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hbwdbamk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tgnfptbk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2oiwnximm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2khwamlcn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nkedcajw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dqrgiczo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2aievcozf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dfgkqwnt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2htctgqsp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2emxizequ.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ijmjmegx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2sqwhnjap.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rsenvknj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilyphllv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gvmvryey.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2foxhhcsr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pkmqgrna.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ehyjgtxh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzdwrgxo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uxfgrlxa.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2iupxrxgs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hjguxcgq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mxrtctvh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2doggigrm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2neyiwvcp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qvwwoxwb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rsuvxzod.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhewvhhs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hgkojlnw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jsejhseg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2igajdonf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ayelhqun.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2flxkdviu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wqczzvxz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vowmkukg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fbcuuwgs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2woyoptuy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qkcknafl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2evjlwylo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lrwwtmjt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dsybljwk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gsbcdtoq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2lglifzxk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2aknfhfcw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xxvcymzv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2optgujaa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2anljcmnk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vwitgnaa.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qfgshdqi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mnsntjwr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uityorhw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cabtdqnu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2tvcxrdfw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vpbkyszx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mtlkqrvv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yoeqzzxl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dgmokwdg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2akmckmuy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynidsife.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kdcyvkao.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfmuswvx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiyisidb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vvhdvwdy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2pedxvixk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2uoyektct.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qqprerff.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xbyqpxam.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vtylewbo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hmkagmgo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfskwcgi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbsdlaum.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2fylnkipb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nbbvasoo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ltxfpohw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ltsbanam.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jyttvmwy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xrwnbmtx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtgjrjie.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggwfkrvl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bfsfkytt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eupjuyfp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2pjcjvnpi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fyqtflve.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tehbiavj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2eizbwgou.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tswewqgm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2atgtlkrp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2msqbvdui.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxipettp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2esdbzalq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2wvguxuud.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cgzedhxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmddqcde.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ocujrkmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmhzhxpn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2eyjiqphi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2pnosaehe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jqdgothg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2eytwrjkh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mipriaee.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hxrrjanf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zoooohnb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ntgqrakw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2srcjpvqd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gnxyehip.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wjiipgqt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2suevojjx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fudbelas.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ajnueuwq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2soukrrpg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lgmwcujf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tftbxfnf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2omuptbaw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ypwxnize.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vrhmdgar.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2yboszumu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2xfftbnjg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xzhbgnoe.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gykenger.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nxfsftrq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jqqvhjbr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hpuaylbp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ganjnnik.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2olfrhwgt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iyzpcyzc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pcedzblg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nzwsonft.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2chcohlys.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2jyrjwwqo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qixmepno.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2sesbmcyt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qufcqyzg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dmwfmkrk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tkjqnqew.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iyhotfik.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vpeqilim.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2iugnexqa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mddqqcda.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wpwuvacc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kzknbvvf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jrurryup.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rulmpmut.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wqikdwqm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ltpaoatn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mmkswvte.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2rxadwfsk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ygbqbilf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pvetpmhd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wvizdkbw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2naecinhw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mzgquxgc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yshlxsrm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ihlkwxvw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2prvzlrwj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qwhydkkk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xswekyhb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2priiqclv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uybgbnzs.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2amfgxrtf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uklgqexj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rjgeungm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ykyozwvz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lkgddohw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2knfxzycb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2uiuhuiri.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cikgktfh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sovvafyp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2spvqzkjj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cxgxgrqc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kerpovsh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ksydltto.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ueenwaqz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fuspjnyl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2boqgjepd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mvnjhudd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bvewtiat.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2idumvzyb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2izmdgtla.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xhjusczj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mbwipaiq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2crupauvj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fdfrfuli.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2uoclezzf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fpmfssiq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kfifuont.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hpqglwlq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lhinghki.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xlwakqra.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fzegydyq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qwalbgwi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jpvsmhgh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2znibdkar.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mabzzqmy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cskimkgo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ezppvqhc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2gtvskudk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2onjfsakb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qcgexnnf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2thtzeuoa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ynzqqfqa.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uiwwohgp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ivykzkiz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wpizsnyv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2oovvlekf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pczjqcbd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2nglarhms.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zkdgjyeu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jqgrzfvg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rvxejqob.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lnkmmupt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xtivivuj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2idjdiniv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kxfibfss.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xpgytobj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wclvnnzi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dstutxiq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kvtaxxcm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2mtcqdsnb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dkpkqbqu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kjntqnhv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hartfqck.html


<!-- 参考信息 -->