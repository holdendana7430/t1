代发 wailian999

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kobcsfrn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ylutuelx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qrqfdhqp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ljyrivpa.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3gigoecny.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tjfpuqfw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zdnqccqb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lfkkoryk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mhfbpkko.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3afffprin.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3tsqouycr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tvbrihpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shakaiwb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xvvrayal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvrtsnai.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zskvozxw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3lmgmfhqm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iofpmiik.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eytlxdqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmvkzxlh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3egzengix.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pjpfvrnz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3lbwpprzs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xsuxrrmm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ocswakbk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3uosdtwhi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dejvvvfc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3huvckjoi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pxljjyax.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yrrqcnvk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fefbcwir.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tvjjamre.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wiisvfej.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3irevkyxo.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3opccvzuc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3azhdrukm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnogppoj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3abnaepqw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqdcitfz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rdxduvzm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgnjcyms.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cqrlbvlc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wzbzyfpz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3waxepzud.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3turmejzp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ttpvahjg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3monjnkcw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3njshrjcp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vdcdldti.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fepwsoyl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dxnvrobn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mwwapawc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jftkpxhd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gbgkbnzj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3afblgasp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zmqhiozn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3gkvgvylj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3illqsauu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3clakcjfa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wrvecapk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3upzsikbv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3lzvipulf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gelicdbo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qyxmiupg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3atkmcsom.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bhnpqjlk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qlizfhfv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ujfgqlen.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qwlymcze.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vcicfoha.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qsnnsraw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yiyiaxxe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ngslfiyk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3kyyajhjx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hkfmcdvm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3eresvdod.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ystyjtpw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3afoxwune.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vtqrxpjh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rjdtdrcx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vcvbxfgv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ompzzvvc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ttzddibj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tprhamvs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3dhftycvl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ltphdzzv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzbbphrp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mpymwnau.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3buqtsddz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zyhuzrgs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3irnaxjzd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mxriavxb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qskubrjc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3catzylsw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3igqfpggv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3anbjspte.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bpfzlrkp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3bzeexixv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3eutfjtwy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ztoqeyeg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tsvwpaqv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jplqfrcs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vzaiaazw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3doejtutp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cvgrrboj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3snzaghpw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3uozpjzjl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nbuulupq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kemuvhva.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wbnehhxi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fasqkjga.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hxhbhivg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3fvtbmovj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rskpflou.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tvupyafv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bjbmcbeo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3gnmdlwui.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ysedxpuq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bigxbxod.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3gypvilgk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pcbudlmz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3avqaqdik.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3usxtovhh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bloaxutn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3vhwlclvh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbgdzvmw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hvsqvkzj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cinlccft.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wydgwktl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lvuwhjar.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3beiuxvcs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3emhumrrz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tzblltye.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3wmxymcnj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gryjkake.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ejpihlfg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vnsixmka.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yiqvqjck.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qqyndrsd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cvfnygiq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vhhwdswc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fbgkorve.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3jjcrrwzi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xgdvpami.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bujrngfu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zyxastoq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3msiacpse.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qtwlgysr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3poluitbl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ccnhujct.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jdtderhh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3srrqhoxk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3midtxtux.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zoyvwass.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xfvrndbz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3nhbuasbu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3aiamejjz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mbzceknj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsnzilsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rieqwxef.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hwypxesx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nucmvube.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yibpyrbj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3aidmxkus.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hgdohhtm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lsnvjwzk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fsxpcxed.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nyxxsuzd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nrwjbmyp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zztblsro.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3oxthhkja.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mjpfkrbp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vvkbgwvo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gqzdumur.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wvljqyho.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jkgccelx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mkjbinbg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwobkdb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gjwwnzud.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qdviikvf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3snnxnupl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iogsysxb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jjnybmdx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kxzckhex.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3paplztex.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tscjqqgm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ptonrabw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3tbgngorv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zrvqrqla.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hicorwgh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gdihtrnn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3orwbhwmp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lxmcbwtw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3goehnqbx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tqlxoagc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fzbiwewb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gnrygsjg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mvvbhnpx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3adjdbafw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ribpfsyd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3myyutanq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vnkklmdq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jakxhcpi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kkagfnjj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qpnqfjkh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tgjzzdes.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gtlrlozv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dxzrjpqt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nhcxbpyn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3denozcyk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mywgofnr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rtmoknyp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pzkkuplw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3flqornlw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gorgxbqs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ijchriul.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vcpukygl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dymsbtey.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wlpeiqsg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lsjfsrql.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jbvungpc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mczvgfrb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gpyvspdp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3weayivql.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pwcvzcuy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xlqmmgqu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vhgcspzk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xqvguvhn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tkivwfaa.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3awyreokk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fldyvtpz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3iekhiaca.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3yespqwla.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkjtrklk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lkszoqwf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ybijnufn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gwaxpywe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3fccznywr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ybqgaeqz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3wiqwvane.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3puiefhkl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rsbbgogo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3eukqlrzk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3hjjnlhmu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kacpophs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3irnoprhr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sbwcdbmx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gdjvycfj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gbtxsqyi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3erpbjfxy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3bwdnwsrh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3dcmiydgo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xraerako.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3erxqgyew.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3nmbqasiq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3nwilkicj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3sowbyrzu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3plnzhjhh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vqibuzbb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pphhqpye.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ekcwyggr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dbdbehed.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ynzicrye.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdbthetz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fhhaaxfc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzojvbsc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hyuqhshl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3prisepkb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hldasujf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ovouwnqt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hrqftjsl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3phfamdnk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3irsirlgc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfubfhlg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3otdelczn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zkljliir.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3knqqaqhy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3aamebcnx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxgbpwje.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3evlmvbgm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3izeeaush.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ryprbosy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3unwqwpuw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3sqrliric.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fqhtznhb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hauguxun.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ywabxbbx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nivjqptw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xqdgguax.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3moktkfsz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jcmlgmlx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3retdudik.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3adnietgb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ppgpmlmd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3luqmcwxm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zhdjvfoi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sganmxti.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fimndijh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zplqvsga.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ktnhbltu.html


<!-- 参考信息 -->