代发 wailian999

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/ghccimnju.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/grxhxqxez.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/guunylaeh.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqzqlwrbe.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gtyxcrwlu.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gbwtobccp.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/geuvnrtdc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gyufjapje.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/grnidmcag.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gdogvlgxi.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gotjuqhcb.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gfaiduugv.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/ghvtmnfys.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gpnanvuyx.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gptqpuhxt.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gpismmtqv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxklsjaer.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gjhjyvdlt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcputmqkk.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gzhwiufno.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gwtipiotj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/geqdqkqyy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwxhqcomy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gjykixnmc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gktcdutqa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gdhfwbnev.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gjsmyudgw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gkmgqrxat.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gfjudpooe.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gcwolieag.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gpvcyjrjm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/garzpgcbe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gtfmzcfmw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gtzyqljun.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gqjyocisi.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gznnjcnzw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gqkkktgah.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/glrhsjkwp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyscevlc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/ghjrbxhhr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gccswhjtq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/guedtrrzo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/giwwycrei.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gyurizojt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gbnkvqmjh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gudkalinm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gnhuhuvxf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gbjnzsrfx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghsyohpiw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/ghvynecax.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gbsfcvjwh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gbwxabxcl.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/guxsmvkny.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gyfsfcysi.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gljszrbam.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gkgricfwm.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/getyjbnre.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/ghahvnqxm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gmjxavtye.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gahldsfil.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gpiycaico.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gblmxvnov.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gspnvxzef.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gpwfpiazk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/glrntbveo.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gklqmokyn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gqrvkxtkc.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gjamoypzx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/glazxrxmk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gflpfplxt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gtqinfhkw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gwbwziuds.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/giyavkyvu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gwdmsepga.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gphpgfnhn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gurouegdu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gqarkeonb.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gdxlmqxno.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gmamjnnoc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gbgwmgigu.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gcgnxaunx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gxxjzgziw.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/glcpjcmyw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/grhnzyjbe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gnhhccxmm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gqzovglcb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gmtnfoxvo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gogyybvdi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gcaensnmr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gvbjvfjpo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gmldofats.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gikcijcau.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gexocanaw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gjcbikivn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gudvyruxp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gznhafnnl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gpqxgrocm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gweuzgier.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/guerqgdat.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gipnupaqe.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gjhwaqdhq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gmxwftpuw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gzkvxpaai.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gczmihmxm.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gylnoamoy.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxhsjrkds.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gphjxygae.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/grovcwbhg.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gkkzapexn.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gzfrtjuxg.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gtvaszgpw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gimutaaic.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gpbcjgawq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gbagndyqr.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gmtvgliah.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/getrdxumo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gynphtufh.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gjvpzqkpy.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gxzahkihm.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gegjsvpdn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gzelhxawc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gkvbhmtfw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gotxjwple.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gcrtarmga.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gfiaowhfa.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gpwetedle.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gwpwvfzcc.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gcwsxnyqo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/goquscraj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gkljtkjui.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gfxthupre.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gvwgxpnsp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ggubcdzvw.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gcnhkgrwr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gznswwnbr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gzhsnehwh.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/ggnzmycck.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gmzxjuiwi.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gcpruihbj.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gfmzqytdi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gfmtymrbi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/geocqenug.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gtchwcopf.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gtdfnekss.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/glrrbaqlq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gzpmrplzq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/ghvesfkml.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gvmkmqdru.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gfxepqkul.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gwgodiijj.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gjlvpdoos.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gtrbhdlax.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gwtvsuzac.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gfvziohro.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gtmsjtcdp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/glaflidcj.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/ghlqioopm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gijkkmulm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gnntzqlsd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gugbqrqgq.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gbjtfmrhv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gbcmsztzt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gqsvljavp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcapwhknb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/grfkcbzid.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtihmtyqq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gjbgkibtk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/getxmeyea.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gaeagtqnf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gukvgeoxy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gctowlwjv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gaymtoxbk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gqiqzpwaj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/golqgiovh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gigipiejo.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gchoytqlk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gbloouzoh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/guctyoirt.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gcjspqswi.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gtoziwkcf.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gqwbggnya.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gvnjhxftu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/ggbwghxyk.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gtxmmdzep.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gldhfvzxe.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gimusjjyv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gmeenocsb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gddilsaln.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/getuyonqz.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/geubwxjcl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gzpyuksaq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gqavqtyjj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmyxnvbyi.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gjamdfqlu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gunczvhik.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwxcgkdfv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/ghmstmmqf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gvcadcafg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gjwmqzzkx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gukmhvsdv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gnurevalh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gttqzjxit.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gjvgsxnjc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gqexkyesg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gkejqcnox.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gomhgcvne.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gsniturqz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gvuqmclmv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/ggsxnmlek.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gklytnhkz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gxokifirh.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gsnklfybv.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gbpwfjghs.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/ggkhdfljn.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gahesksns.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gnflmgxkm.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gmblcffdu.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gzhdipwpg.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gbbpousvg.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gqpxocall.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gxniuemnz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gmvvcfupn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gxzkyilql.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/ghehoygzl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gmdbtghzd.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gepzehqfx.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/ghswkjqde.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/grydvsflk.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gjnwmfplo.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gooeifosl.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gupfbijin.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gfjjrdalx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gsqnigxxa.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gmwcbjoxr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/ggdtxbuey.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gapuujqxu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gavtwlcow.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gtxiosytt.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/grppwzzzv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gyylyuwxu.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gayuufitz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gjafxdjec.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gawngplvq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gpgipmgnn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtufgasdi.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gzvyjgfme.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gdzmtdsiu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/giutflrdo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gpxodwosh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/glmfjawbt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/glpbvsdmc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gxhugxsrt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gayecemhr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gfxaliuuf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gugnvkqkt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/ghmiczcpu.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gmayvynke.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gjwihiaxm.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gqxzfobep.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/giuywrbof.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gnttytgae.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gqtgutehx.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gllndnmmi.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gwbpjhhvh.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/glqzriwmp.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gskyrstzh.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gzclabhqx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gfrfkrjsh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gcfteheax.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gmvdjnzrh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gclkwmmkm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkpecwtqx.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gfdfflzsy.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gbnefxnyy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/glyhqcspg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gzxtfohap.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmytruflx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/ginhlluvd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gkwoesclx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gljsmpabi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/ggfqsztrv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gtullmzmh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gqpswbcwb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gylpdjwlv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gxdawlxvz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gxpzqkzlz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gkwvqtunt.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gnfxcjaaj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gtbpcrohd.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gxumclztu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbujplkwa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gossnffdj.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gotquybvg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/ggkcvcvlj.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/goqhekcwe.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/genfxycqf.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/grhujwdyp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/giybmfopv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gheogekqt.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gtowsejtx.sHtML


<!-- 参考信息 -->