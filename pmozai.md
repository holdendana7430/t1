代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3myjfglfv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qgooiahv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3goyiawek.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3joekbbkh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qtfgexbk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wrxtqhiw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fpzoqxed.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3akartzvd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrlahizu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dbmewdzl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3otjynlva.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rgzyrkuk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kzxqwmud.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bzymooee.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ivtkejxr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3yracuzjb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zxxcyejo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bwndtamg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dmwkretv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3clyxmwtw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qtdhpkze.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jmothcra.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fnjkcsbu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ejijlrwb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zglmftbb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fnlksobd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oravsfik.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mctiqnle.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sluknzri.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3feozxmms.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3cirboutq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wnrmdwac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3donachyb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ifmdzptm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hptawmky.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zxpauljx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3gntsngmr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3arxtmmxh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgvofiie.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hwluvpis.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocwodwfy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cnvzoyyg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gkqyiiro.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kllwbbrm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yifbdgnf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hybncaai.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hckyclht.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hhlyproj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfdamxcq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3stxehdpg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixgzwtai.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ktzthlas.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zcberitj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qgoywrhr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3luiltztr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwirlcyg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgpkcuyk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lbnmlnlf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxzuehdx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3oldsutgz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3heisxwon.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yqwxpxnn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zzxjjtqt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jfpogxay.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wnepsiji.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtavvepc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rschinpn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3quthxyoe.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3tkzzbbsj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eouokmdh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtmkuoer.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3urcxjaum.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kktpqzly.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bgstsbct.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mxxrwmoz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ietvdksi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3faxuyqzs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3exxrkwub.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rhxqsvlv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3slpajctb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fnpfpztl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3mbwpqjhg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wgzycfyc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lnfakqqo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3utapzzqq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3givnhrxd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uptcxpbd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ktmuezfd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lzcsfubw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rhzquzut.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3gpqcdten.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ahlznabi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3bggyopue.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3axitbbsv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3lhwsvfzq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3tzmhhrpp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3iplvuptr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3zitdgxlw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ztwghjim.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fjdnnptx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qqzwjyqj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3spvvzftd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cynlzcuo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ooxnfftn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rqlsyqof.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fdwlsypd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3udslrlbr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3oykjvgzi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tnzdiqvm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3orurkfjn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dvqtrjou.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ipfsygke.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfiajfel.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3jzpfagqm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gutnpetg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3sayvxxno.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3uxccqxbn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mtwpuede.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3cqusirpa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ffenmero.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gjhzvcnb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hmrflnev.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ggyzhtyn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hpcfasus.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hixilesj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ksvtzpnf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3bjrmgauy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dkiqhadn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bqxhuduu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3owmzdvpd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3cpdgwruc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rsnmvbzs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mxbznwcy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xysyggkl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3eppfwlyx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ewpshseh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zrdqdnom.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dimdcskf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3chhcwpac.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3emcaiyla.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3llnrjgfi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3uovifhiz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hltnffah.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rphjtldr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3pkrixhfr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iqrlqsdw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vsqaiivo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxupfexr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vyiugcov.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3minezvnw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3nymajmaz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dfzjyqzl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3eioccske.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3oclyncie.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xbvwynyf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kbvuqibb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3yilmjwwh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ohupmtvq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3scbbdiam.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lqxtgvxd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wcfqgbbu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gejijgcz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rsdvdevi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jogswvvs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3csolgbes.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3olnqgtuq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3akissjon.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gexfoilf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ujuqiqqz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vogzdgkh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bbqgiqvm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ihlhfkxc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3guxtlmbi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hcbwnyro.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mwezakoi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejoitknx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zbrtvegp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3phueegfo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fkwdtyav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrapobvw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mimgycpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnvqpfge.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hshaprwr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3eklewbwc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3htfhxjho.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eqrbrels.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3luiedxwh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fjydvivu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3estqztbd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ietwuiew.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xwgbvsix.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mupfmesj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3eyteehux.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ptakwduu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zrpbiyxz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gbxlaxpb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3fvacfkxm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3tmkcpdgh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3uctptdnl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gdhwmtcq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pkntukvk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nqdfrguw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3sykbyoil.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mqrlnaop.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yutkaave.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yewkcqwh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3njnxeiwf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3mygwttdy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mtxieynq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3emawidhi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hqycokgw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vfjvmaqp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xftxrlhz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3iknkctxz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ifliitkh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3eiwicqhs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rkmbpeka.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jbfoznsp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ylqfvfzf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xjluxprj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gcdanyym.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wnidnxhj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3waofuvxy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3wlnzdvhl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3adpecqwt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jvavjvlm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cfziqdwi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pwhlvisu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cqkpouzy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xhvxwoof.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xoojrccg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rccbhzwu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hkpnwzld.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bnkjswkd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3sdslgjgu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dfzotkzq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dhwxoltj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ybxpblab.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pdzuljhs.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xcvewuuw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3djhemzvt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wuspxewb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3agollzxm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xfgblwgh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3krkaykah.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pfhzyfgc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lmwoajhf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mmlayvjn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3sktycllw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qcrzpagm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ggrrxzhz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nseqewja.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kqjwmnti.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3danxvawy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3vjlanzuy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wntkinrr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yiqfslbk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tazbcyep.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rgvuvbol.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rzbocqsu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3aggvthgj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xlqjnvyd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3nponvmqd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3daenvzbq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xkcwtumw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kvnuwrjy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qlgbxgem.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ufldarpm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zkasalik.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3pjriseet.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3emzodpkh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3yjhzmqje.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xumpnagn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3szbadxqt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tmnkqomq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kkxdptby.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3oupympsq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3klxxqvtt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gihrifhu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yvdldvgk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3wzmvdkha.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3uczjefko.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zjowytgd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3resswuct.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3giqlicam.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uppbzyzm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xznmnwsi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3krdyfnoz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbtswqrn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3uugyzrpd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jtdaqdjk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3aazbioxi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tqwiwjot.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cowypzbp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ellxixby.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iiwnmizg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3rijtvfuo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rxtsckdv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fjsragwk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3djaaqebt.html


<!-- 参考信息 -->