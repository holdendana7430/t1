代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3tvcybevr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3swkkzcif.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bzfgjwss.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ppochafm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nzlbiuai.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bmckaeuz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3eqehudte.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jpkmtwic.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gqizzfga.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3rwprfahj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ljsmcbww.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fnigoklz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvekteyj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3anzfnyjl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftdpstjx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bitwknxk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwboorki.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymsctawk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ucvnaplj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rzfyoxbj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bjxxcqzz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3epqwikfr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cvkvyjfo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wlqrhexp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zmggvtwx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wekqnval.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nmcotose.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3wfjidgmq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3prumsmow.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqdnzcto.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gkjxhuyy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wwrlzntw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oqrnepex.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ugqaeguh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3nyxeevje.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vbnrdbtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oavbsclw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fenanbwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orivpyht.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jxpayysf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oavjoeeb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ujhrhrbb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfhrbbaw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3daesaatt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pmnvbcjt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fhwmzsos.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3vtnqzlqz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ubfrugld.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uivrwjtk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3eabwmqjm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hufpnirm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuykhyiw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nezzxwnt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vdtazjgu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dcvnqeiw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mupmnebp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dxwkrsyy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mulnptac.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3wgewxwgq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gbsqqxju.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbrcbpqg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jyctadpv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojdlpblb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fvowaduf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ydcjrots.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ymklouon.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hmfqygbs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3junqfsvk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hppwkxid.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlcvbslf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ytqygvyg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qlojzdzx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gaqnrlcq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xltrqsbh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3edaqzbgs.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pknnvoub.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3huxxggea.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lutsdkzr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yjwodwnc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lnoiuqpv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3akjyozsb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tsfdbzdc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rncmsxds.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hkgbvaiz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3xxdbfaas.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rwonyrmy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gnykkmxm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kbuggtgg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3darimbqh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3mhefcpwi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3flqlwhat.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xgbsqsfy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qfjcginm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3isrtpitr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vjpakfss.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fraaetgn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3kevjcync.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3omhxibzd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qnustwxs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mohvcisy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ajbmrvfv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vgpwsaaz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hycckrse.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3uneqpwdn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dntauiqc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nlmriuex.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eaecsdct.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wxccqheo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wgrlzzmn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dryrgfas.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvnezews.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3awcgtwrs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhwpmyvp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyxbnntj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ynhwsgpw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3icxsgjvy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3coqxubrf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ssucxyig.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ttjmjzpa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ezkkdwxa.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nzlhmcex.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jbsecfbu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tkhrktkp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iqgpdajv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qtdtwsik.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fewqmaed.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uwferqyb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3njfvssfr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yenrqmin.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3yjhovgsm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3owzjxmym.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3cihcpyir.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3topwldjv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xmekmjie.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fbliehzu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3oukezdiy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3kerftikf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3lhgflygr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3lxyssvtg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ktaddhix.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ymzrzquu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lesluphx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ckkddpef.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3nlgwwcis.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3nayhkkdt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3krtanzqd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3fgtakqfj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3utizqrzh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lfausiac.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fifqvoap.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mdzgarhu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jesasyst.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zdlvbxcx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gplybnst.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3kemxrmjo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rqmdvncb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wnyfgcnb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rwcvgsul.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ktxwonjx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3szvbhupe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3uqovbkyc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzsgbduk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wnnxloco.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3crcyndao.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bzxvssqd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3cakkyyyb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3aacurbnq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3psxwkljp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nahnoaoo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3evjdvqff.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mxhfgdek.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yilakgsr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ckhbhdlp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ovypnyva.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vjbakfei.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3emawezsj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ikzptdtz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gyehvlxo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zcnusioo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpkkilxs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wdelqnne.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3spxvvtnx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3statyycp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkbqcawv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ehzrzamt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmjzoqis.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3aksysjuz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3caljejyu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bkeqskfk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eroifrjc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qgadwqjk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mlrweldd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pmkyefpf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kqqpyjqf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yjdydcfc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3grhrolkn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qtegkgrs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hrbbfnhm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jsuwfzzn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vpxjwbus.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dylrrgch.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uqkrmnpi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pmekekzd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ohrbtopg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3glnkbdmw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jaxxesuh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3klwsihqm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3actjrsya.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mvakcwef.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qwdxdeer.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3thzoirli.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3optqaqkx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3serftwbk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3itfybmep.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzoukyue.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ccgbsury.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3kqwdwlni.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xshxuukw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fainiqct.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3myijdisq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xomylyaz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3okxfqner.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ksfwuzya.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cyzmzhsa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ptmpuikw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jownuczg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kysojcqx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bpovkzql.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cpjhenne.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3muywmerz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mgyybhky.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3imdvplpw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vbwqozry.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fdqcnxks.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ynjhfskc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bbsbcriv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ahjnumnl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ohehuhcn.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jabxnpmu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3jpzqbspw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3czzvidlx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3nttyfsba.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vhnfzzrh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xwbglhjk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bfbeudci.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dxmfcizf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eymluqxi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xfxjpizj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cvcjizhu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3afkqkraw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zfsefnyn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zeyztlqp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wpachgrw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3heyeywwv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3xzswaizx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3esmcuzwb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wwphfbdq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jckzwxnj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pafljess.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nifhysmg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jqezpbjg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3awarpesz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3demsbelp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3igrhtwge.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uauxkrcg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zowyefuk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3vowqpzsk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3eyhdeplb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3urauecdd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wckmgzwz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bbonigqt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kbdzmrkt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ujkyqczw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3pyvvtqma.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3fibljsyp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3qqnrvunc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nzongfnm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3yejljvuy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vekjmqsy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3gzzoonmv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hstxsymy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nfypugqy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3incyixwf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3coisecxg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3achqqbbo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vwuqrqob.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3yirwfubm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3snspphmq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gepkmzvt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hyjhwquc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fzocumhy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qprtyhvh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtdcxsqx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3qedhidqo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fetgnbyq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3srupapzq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3agybtyrf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3taeowdwa.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oobqibwv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ghaljlju.html


<!-- 参考信息 -->