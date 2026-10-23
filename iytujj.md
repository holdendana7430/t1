代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ncyslwqn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wbzihiub.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ahuyvfjf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ewihlozv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wamrqljb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3faecdibz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gndcryfa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zqvjxwpy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hnxtwqvh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jbovxkes.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3pufnoovj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lwtdvjiv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3kmwfeowl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rpsxslim.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cvdksnvh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qfeohjqf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjzhssi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ewprfeov.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ovqkaszb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3sfjeisog.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3nkskuisa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3yxucpghg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3biirhkyv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rhlacymm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmcrqkpt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tqzjurxy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3syhhgyvq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbebucnf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qzwnqprv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxsqwxtj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3stsckysc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uwfnmfye.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3knostylo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lgiuvkxm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aikdmaol.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3twxmftxi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hwkmialr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ualwaogv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vhsnlpci.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3kjcjifas.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3auymxgvr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3moixqxnz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mrgadddy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hqtpntmw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mkqcwnuh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gkllzpkq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uiuthwsl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qennezrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcpjqttx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pchlgqmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3biivxvxp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xuwhkxtr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xyqjhsoc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zftqwxvv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpsqgpjx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwvympwe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixbgppna.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fzzubkso.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hoqgbite.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdqhqhmh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bwhhaigf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ioorzvvc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jtthxlpo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3atbtxyar.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3inutytia.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wucivsak.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3okahgvyn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ljekxzyh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zjvcijvb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3glhqqstu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3stpagwzo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rkzmwrmh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnbtzpjb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3eunlluel.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vevxqwzn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3dahcfbmy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlfnvnmr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3efllzyso.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vwgepoor.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3bhmlvkyk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mqynnseo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sprqfbxs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3lvkkhffl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3sphadxgw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3uvtcrxjj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cokxowfc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vteypuij.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wskfquup.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jhfvxnok.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3msscxjkb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gjwfxxpx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dfomzkwp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3itlocadq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yafnmytq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tzfbtkkq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xpiopzab.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cgqttrhm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3hdsxxkym.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3sszaoyxu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ccotdmij.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nhkksooe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ihvabncp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ulhwjucb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3txzpwkjr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bdxopwac.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3psztktpe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zubedglj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vgqtywfr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3wdlpytdi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hegdynlo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hnmqyoiq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dxnyyitz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3psjxnmgi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3nnyecvup.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3nlxtreol.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vuvoqrrl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xonfaara.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwnlnuly.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bdtrclph.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yimmnrxt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3uxhiznxb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3valxyhos.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxunhcoo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ydtahckb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oflybccs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jiklwogo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rxhcrlkr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wgrtxdqk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3avvhhnvt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kfeejzyn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3casdrppm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ibpzfpzz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qeuaadgu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zyxxwyzf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3pragkdas.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mwtsqnpq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mkvwgiqv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rnuixypc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yhdmfkbc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vrtulgxb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iwtqwken.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lhmgldsx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zbmpaucj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mfcwtpjy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3exonbkym.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xnkibgjd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jcrguecj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mxqfrpzu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xeziesol.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fjhlghgh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tefrhrpe.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3njpvmxse.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zehbcnbr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hgyexpwa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kivsnpjy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pawmotxu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3efkzvdvr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3oaumeaal.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nnnrpirk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tseycfpt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ugpkwvkd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uchuwtcw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hiypqavn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mtkvnwit.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwppsgcu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3asrftxsj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3scstrzdo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3etywfubt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xjvtmnwn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3yanmjavo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gkvsjjij.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zbresuuy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3niilpvkx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3allseqlr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3duztodaa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rnqvaacf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3unxwjndy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3riegcsqp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ppeoeikc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uvigeido.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3afsziojk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aebmbztj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nazynysy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kymswawc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3etljfwxx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vskkssqg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3axlojkxu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ralapolp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fvbnqusk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rlzxkutu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jnxtzepk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jzwjboyx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3oftbrgyq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jbehqaaj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyuzylvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eobdckkt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sztqsczy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntkcjccp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vcfivrtt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3scypqehf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zbaeobtd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tnljtjrf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3mnhjgfpd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dbzpsnrm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3uubuizqz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3chksluhe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ykgyvpic.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3afibzafh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lovogwuw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wzuajyht.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3daafupro.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3juucbpil.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iwnbtgsb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cazkrlsl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3frwifjmv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3uyydqxwm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3nyzsdrkn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mmvvwhar.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ivusggrr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uexddwim.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nffhenkq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xuxnblcf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3enlrbpcj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3lxrneozk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lmbnipze.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bgcnimdk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zzazvegu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3evwhzkud.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zbzgjqyx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iywpjjlh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rpnqkhai.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3iibzizoj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zovyfstu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ytvpajxd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zxyjdoxx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3klhbnwra.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wnzvducc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bzvaleun.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jwkwblmm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qfyqmapb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vvhtnoub.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gthshskv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jfdcblaa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cgevijea.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bfmssrua.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ldctfivn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jfviluix.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jmnqhbhb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3khwfoshi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jzwjactd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mblrciux.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ixpokprj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lxrogiwl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wyzbcwft.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lkstmeuy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bcbmzild.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fdwnpyah.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3teyepesm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3toaapjvi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wesdnckg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jkialixq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bfikagto.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3blxbhcjj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3shwhiwbu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fskhjsre.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3iasqrikq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cpehorxz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mppohrqm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qarouvft.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3afngtypg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ntfkjbsi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wscnbdhp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xaqvmijl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tkjfforp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3eyogacqm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3lzzujzas.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rmgfdynd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fidvgedh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3luicyamm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3lyrfmzvd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xcnupqvs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lygqqfij.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdjhbhc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kyourfgg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uahesxay.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xxnxwyab.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3peivfjfw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bzgfeoxn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3swmbwtcp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hrmtpnsm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scifdktt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ysxkajqm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ubyzxslm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rzrjfpit.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnmjqdzy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3slxreqvk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zrjxvsxy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3bxlznpev.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pkrqycwv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oxzxfquk.html


<!-- 参考信息 -->