代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymysloth.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztluikqs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvhlupmt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3nedagomo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ezgbyggr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ftubeynb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3dpxwbuaz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3uobeylja.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uxilnofy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kwvcdbxc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3msiauxyu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mrdcehhs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3arwwulip.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gbqevxat.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bmsyqbgy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gvbchxmg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3cnuquaip.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzcnwkoa.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3souebsny.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tnmmiccq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cazpmupz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ikwfpiss.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gssyjiha.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3uqigmwyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlxxamhx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ymzoeeqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wypidnqp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tkgmvpbp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3cmfaaivo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iepjjyko.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ycnjascs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ywwfivri.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeqibdlx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3efsuasgv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3sobhzlrf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3beyydrgw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zhoefxdn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3adrwqueh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tgagrnrg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ckrzempp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dqcfvzcx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yjydjcrk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tvjpctxm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bhujfeaf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3xcrzdrrh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wfntukrm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3umwbmzcw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3aiyqmehl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbfuboqw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nsvkblkg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lqfdqktd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zbphqavl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ffulmmjw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3pnxnltwc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3itoaqcmg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vxyjzdyy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wlbgtitq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnehadax.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3auvkifkp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3alhauynz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3odmqpeqf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qzwlduvr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gnktqazh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3bramwhnq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lbecsmtx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xusvufvn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3heqtlfaj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kckiivch.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dqwtbsyq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zlcxcoqq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3pghqncgi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3edxvnpan.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ftkdnykv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3hgkxfqdo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3phujdwtk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3niofcrkd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qkphhjfv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fqbutsho.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vtekcfed.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gehlvhhj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gjyikzxf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ytrcpfoc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3snsahuzz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zifnwgww.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ohzqvprq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3iomcpwcb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fziqjlxa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3wcscvnci.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rmhwmhuk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wsepshpj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3oueefhqv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3blxssrjd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cnhzaqaw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vsmztzmt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dvtcnwts.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nrjlfekh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ylwodwtp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3galqclbo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qcvarxmf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tmobrpnw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnzgxgsp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vlczhete.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ybuebrsl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ffopjvcp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwickklz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3aodhgxuk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ybjwpbii.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jzhchcod.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hredxbhr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gwmvxzwu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rulfbegk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mpevjigv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xdefopqb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yxwqrppm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3byywsuqd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3csuqsyoi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3luqnasrj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3owtbsyjd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wsazzufk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ggqtfkva.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yirgdruz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lrvfpvet.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3aqrzpdff.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3hsinkgzq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ukyihdbl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xbhlotiz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vjhymmer.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3fynelppu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3owftjnop.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hlnagcnq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lthddrca.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3phgrqpaw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ppeufyli.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tyqupkht.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ltzqvczh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3chubtuhe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kbosnyia.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgyxwqns.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vidrwsbl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzngneft.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgwvabwu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3apwbcsxb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3huygerjp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rltxmjje.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tvwpfyrl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3tbevxooq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rpydjjol.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lzklvohc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnakeugv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3szkihlzh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zokfdaxh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sasjibif.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3axsgeeno.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ugxmjsdn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3byptrxyq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hiltsfik.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bhefexuz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cllabzur.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ovqwpxei.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ordhitnn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3brzufaiv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kzoqpies.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uimbhonc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mykchrcw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3oepobjfq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3yrwlrxuw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ahyspkuz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hcbwpngh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pfqdvuly.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gvrpenkw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zdhjwqhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efrawjnw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3tshegxff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgjrlxpc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ugchbaxf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ckdfppgs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3quwrxonx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fwhkxyuc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3azpueful.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wobqapue.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3nsquxtym.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3moeiuisj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yljohweg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eikbslrw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gagzikjj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uargpbvr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jcrukjjn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3atougpnb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qujigtfg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3auzofamu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ffbwkcgb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tumewvkr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wbcztynb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qrqpspnm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wkcgrxyv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3orqzpiut.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3umymagtk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mbmlqnzz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ygjjpjxq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3mzimzsxv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bnzbhfgz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ianrtftc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3sicuhotu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3gddtxbmq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hhnepkju.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3bjnawufu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3okmzzlom.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nwcuuseq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qoxxkfmn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3yqfvqeni.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3enxxcxja.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gwcqvpdj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hddgzgry.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3adjbfhzq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ipzmxhbi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tieqctoy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dnnrbvnc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hncsxdvx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wfuayjvy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3machfxkv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kdsptvkn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3skfkvece.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lpdpaqge.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3grnxiwax.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3kghtnkjt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qxnozmvf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kmzwvytr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pnpiljrt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zpompcqo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hzwgnthe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nzxkprkw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hqfzqczg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ilyvsrzg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bbhjhnyt.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eiwzcolj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bcjhtgtk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sgkhsmsm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xrilyvlj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3stubzeeb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ghdeoxgf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qkwjffjc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3msddnkyh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gyumpqjl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rhbneomd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sxcupdph.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uqcehcsp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wvfjhelp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aptlobla.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nqhnlkbz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xeziqkuk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3iipyepfm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hgdisaxg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3easctyex.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zyvoftuq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lpsdqwaw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yghsroty.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vcmowvei.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hcvksckl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qcqyeeaw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dmdjyvyt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cccsnosx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mgulxgcz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ydocvmzk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xpshluqs.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vlzslrig.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3gwjvgavc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3nkrvztpq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3knwxnvcg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ytiialwc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uaumhxxj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fmjrbkcm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3enypcxrx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ovaftfns.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lmievwkk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3elpqqyin.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ysgblqlk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgaziqcs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3slnadveh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hqnbwhvl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iosqyztb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fqkulkwb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yosfioye.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3yhuubazw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wxfggkeg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3akmwaeda.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rydugvbp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3acqndifs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tqxftzkx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mxnproaq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3epdzxptu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hpkzlitr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qkrrlnso.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3knqjbjaw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ijouhwtb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bvpfbebx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kuryovvs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndsuxldz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nqglbjdz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jzwmkcms.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kjzmyjzw.html


<!-- 参考信息 -->