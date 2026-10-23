代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qwhhrnuu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ezwepahv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3leosrbmv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3mvsrucmq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fnviolxf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ckfbwlwl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wstmrhxa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zfcuwqyg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sdimagxq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzsjoshn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zenxusrr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cahuffuz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pzsppetm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmglwrzo.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fmssuiwk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ssezwavq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gkjampxh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eqqvodck.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3flxfkgkz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vrknjrrj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rrnaxlgp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3szduqjti.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dpqunkmx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gvtshrau.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ujowfseg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujlibfku.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mwzmxykj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qifeupkq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vgpurofn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nwsdgsca.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3wywskupy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rgfdgilf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmccgjfi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xlioqlqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvgjjuqp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ansxxdez.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fkdingfp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3spboeoba.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vxsfsbni.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jscvvdex.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xctyomar.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lqfxezqy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ikvnhpcu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rybnwzka.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3usmgshiu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3scqywfds.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjajamwi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqtysisb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmeidioj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xdileoiq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3appsuajn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dtylgppi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hfhovxcp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3fhjjvlan.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3yjhazgvc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3obxcxlyo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3azupjydw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3impvmawk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkmkzrpo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qsarlref.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kyncfcjh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3wfoxivue.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bfzvugfg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3pqvvxgew.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3rvawnsps.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcqtbcdo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3dgcagcme.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dksmicfi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yfsvtuns.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3reazmozo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfkygixa.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qgcgaqgw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uvukllaf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3kknycazy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3brcwuctk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tvcfoexi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3bvbplnyi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ljnpmtmo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3iigsszbp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bocokcnk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ppadaero.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3urwtofgx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ykwxvfry.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tafffvyl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3khpuggvq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3khqdqcon.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lmjdwped.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3snkwnakj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3clzkhdme.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bumxiuau.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xjgpgfbc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3funhpskb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3koumtaqo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fmrqzpgj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3enkjviua.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3svjphbrg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3atmxxega.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vpyvpcje.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ftxtcxco.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ftywrljo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtilndmy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ugahppmf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkozkump.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3rnrcnrvz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xlmmmmba.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3sitaurlv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhzgexsr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vowrundv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxcrrct.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qwpckowp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jjlmamto.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tpaphqxn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ideaabnm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3gbsjyfpe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sunfasbe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qkhclsev.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hmqfpywe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3skgohtlk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rsvqcwvt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3lpgobbpe.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3peqqsxxm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3huntnpss.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bfhjxxnt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ewmqnhgh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3suwfeppn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3lqgztxoa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3kkfrdauk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gmykrfjy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hnuvcber.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mgovlszw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mveebkfq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mgpognwn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qyjnrtft.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pzuzfgzd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3hxhejwdq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sfvynoas.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lyhpozxv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3szbqedoa.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qqxalrxu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ixsgtltb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3lelvknst.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wcbzwaav.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3flhovszo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3dymnoxyz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3epeqkldm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgpjwxfu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3einhujdr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3delwdxau.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxiehrdc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3pldhbpml.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3rylokshg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3bbrwadkc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jngcenbw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jqsmqiyy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3soduuykc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ejwpqzif.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dppbehdz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lgukxynd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xpuqdori.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mpmncgfl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3teqjzwgr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qrjqvamh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3fvvkgpkh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nootpqwd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtxzxqvd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3cwckxrxt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zmnqrcae.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kspscsna.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kxaktwrx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ctonjuwv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wofvruzr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3yvodrhal.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zzysnkzz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3adexibov.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ybbqmche.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqphgdnp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qlzfnqub.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jinqpuxc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nofghazx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbfqkwmx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uvwowywq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prkfsopk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nwwevard.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3eblzplsl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ccttwwxz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ghoxyxqu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3eeaxldph.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fyycaejk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nakjxjxx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iecdgios.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3aeadjgpu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3uvnjdtmh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wzympblu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sntyahqh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lnpuznhh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3snpwpxgx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3esryiedt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vjbhzsui.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3bnyodupi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3shxspwgo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3osnavzxc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lbzenbev.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qsajzyrg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3xusfcxhc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3albfmajo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lcffxbcj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fzipfpfp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wwrfrrcf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ctfrcbca.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3baaumuay.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3csejvwfq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3brpwmqxl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3anidufuy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3nxkbxxvo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rpmwrstz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ihqiptim.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pnuffkze.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zozqvywu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kvyepubg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3epcmqroe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eaviwizm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rmfsiwjb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qhdxxazd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3pfogmbob.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xgdizppp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qqmmimft.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iqpmtqec.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ccvmojfy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xnhdprqs.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bohmgyfj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vhbwqqsy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zcsflvcc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3yxznkksz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rievqwbx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hifseldh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3stzrnvcg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ovkcztvy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zwrevspq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mpsewtuh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wlgitiam.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jisznsuu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wshgwieg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3atzhdhco.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mjepcedr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hstgjoaj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3egyrvqbm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nsbbmlqz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hiczidoq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bxmbnlyk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gojbkecv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3xkxuxnxa.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jfrqfjvs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vasgbust.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aaarkqge.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fwpuvoyw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fneqkdye.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzgcyckn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kruegkkr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gszgdkow.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dvyoljfc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hwxhitcg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3trqodxau.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bfsemzvx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3dwyiyjfv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rypsnhrl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jgeqvjjg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ccpszgnl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ldkbczlr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qqvfblbb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3wenctfni.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3embpkkha.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qxlsejpz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3cozarcvm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3biwbfexa.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3twwedrng.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3muienfmz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fgkndszd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rrgfrfvc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zvaujqer.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iwdtagzz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ncijjkpu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3owxbgbbx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3snefvqbx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fanuixko.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tetvasuj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fknkichu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3vrlpsejr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivpcgrqp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ylixotdc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3immqczje.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ksrhqupi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3swtlkflp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3eadilsqv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mxzyadie.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ftmcumpz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3rnnvklck.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dwtmehka.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xewfzggi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fksoozjt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rupnyxpd.html


<!-- 参考信息 -->