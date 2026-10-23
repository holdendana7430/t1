代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3szlbyvuh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ambhoiyo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ireagiyw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mzpnynuq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zukivuqc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tarejdci.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mpythomz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vrounfjy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3pgzccyrv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3fiwicyog.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfkeqoj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mppavszc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mazftubm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3grrlujld.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3tankupzh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3pphytdmq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xxabsaub.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ozsitgju.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hbuqraax.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3acpddvgt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jaantxdx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uysdkhdw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tlhoujlf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mabfwinr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rzcvofti.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkllpykp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vmsiuzof.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zcdmkxys.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ewmrgrju.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hknlofos.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3krsidpgs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3naheprbp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ifyickta.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uxgsuomk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lsbqszak.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uwrafxjk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3serzbcmq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyechyhi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3riwbyzxg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3efnbjyng.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dtzoucjb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nlpvknyd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fdrhziqq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ugcyhtfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnlmccta.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qfyirubx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhhbzyip.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pkgkeqdk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ikgigqbh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ojeetgng.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdaggclx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vjzjxymd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3unxgmrtp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3opkahxku.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ohdmqvjg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrjqmtfu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sglqzkrz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3djsspisk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usoqylnd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwvhshak.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbwikwdk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3bpahjbik.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3flgusohp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3nnmhmyfp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kdcodnwr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mwuxezmk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3urllyogj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lkxgvsra.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wppbzjjs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rezjatba.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3dpjchsbv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lqvmzdsh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lbdaigrm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3sqfwfqxo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tthduoik.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ldnnxgxz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xksbjxil.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcfriyik.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zomgoakg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3snlbhnze.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3chyzravp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rqowfpbt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iymgklcy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kydruqos.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dplghvwg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ugkxwmxq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3frgwjbok.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wioffwqf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fktpvilw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3odmskmhn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yzcemcvp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bhzhhgnj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tkirrjva.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3empunlyu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bzwzbyhx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rzewdgkq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rizovhwd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3qatsvjjg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3urenvhwp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3holgsxza.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ahobbenq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3hkggathk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3cshaygke.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hmlgwnpv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3wayjsthb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3lxxhmtxc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sfiyjwdy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vxbfkmas.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wequzgnt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tnrtsrcg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3awbrkfbn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hvxinjhu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cyqhyeqh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gtqnjeyy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cdhcnazm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3jyeswauv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3usfrhwua.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3otsvdfex.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ospjwugs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kaelnkmb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hitzofno.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cbuqzhmc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3awyfhyze.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ojqenieo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zouckyze.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3azedtdwd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pqtwzsmo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hndbbrqy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3nuhvupex.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qjbohtdp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3npdrknkd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ceyjexht.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bzawafdn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vjhgvivu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jmkzgfln.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ztudknxi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kpzkyrbu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3rdqsdanv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fkwwmbfn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3jxnxmxzi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zkbvncsh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uojewswo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lbxxjrky.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3klopxhcb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3yzrjkbtk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wprhpglk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3kvjijkdu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3jvicospf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3cyaohrld.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hlccndlw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gopbkaem.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bhhmjnts.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3juxleomm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bfhicnwi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hihspeyp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3jyilzzwg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ukhmbfbg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iayfxotn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ozzbigya.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yldcuetn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tibwyxvh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3hyaprwna.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hplhuwve.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tpjovkda.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugeavshh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3wbtqmmse.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iyfcthyc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iufbrcvd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3scfqwhhy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzbkpxys.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dcjugvqa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rihfxdgi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rczjotkg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3oipogsym.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hfuzjbta.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ribzypcp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nomzwovs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmelgnhc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gxefcwbk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jrqceekz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3eriawzpl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3fvnhuqpw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ktlruufm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xxrsnyiu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yoledpie.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zchkslfb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cuqmcgmj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xtphonrm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wzaocvwh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3hvslxzld.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pmzovgrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlwooepq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3uiuovnod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cheajrek.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bmsxwlkb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pglpczdf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3svnzwstr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ngdeusqu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3znnogrjk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xpdneiqv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3msnmccma.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3grkvtymy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3csgfpuxh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hqnebepc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3nqlsfkox.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gatxtoer.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cecuboxh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3urkwazln.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bssjlqfn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xnftmogk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3uuebtvbs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cpesekuz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bthxtcrh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3sqcforos.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ljtvhfyh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xbiezwez.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3udrangqy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3akwsbgjj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3gdqtoxpi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3thcfvddf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vsxrsmvp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wvcvhizf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3umkwflmf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3xnjlcmat.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3gtkphceo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jzgkeepp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jiksatau.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3imjxjxwx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mggmikjt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3crqskxvs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zhalicxd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vngkqhyn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ajwegtbg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3orhigtor.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qlguerzg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uyvcscdw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mkszkmbw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tvjgqjrh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3daftpcxb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wjalravd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3owlcgusu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xvlwghab.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3htosfsaf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mjgpwzdb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3uqiqdtod.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mtqfugms.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nawagius.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3udpimekt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xvrnvzbe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uzeomdns.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3btzrceqv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3icglvrzg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bsftukky.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3swfrzace.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ticclclv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hnvzyumn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dxsqzwty.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3llsgiohy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxuqojv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kjkvnntg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3lcfjluey.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kpaissay.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pzdpwvon.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gkgcgtls.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jljszgow.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3onrkrmjl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3noecjkna.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lmslsbcj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yfafhrbt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zvcjdajy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mtktjtai.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qjxbhlgg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tgmkahgd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3skmfzdia.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3dklvaglq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yvxwrzau.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lmushuvj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rqojvhvn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hvbtrcpw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tsdangie.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qfdlwjxd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kiomvrqy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kxqgordx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wuxolhkk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3bpyhlwnj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3csahstpe.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jlsetiko.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3oxcpqngs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lohgphof.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sorvugws.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3huylwavb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pwiaxnqa.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uywlvmta.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pvkglhng.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3uwlqqdcy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ccpyqdyt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jqzobezo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xzbpdezd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ytffcmvr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jokofqpn.html


<!-- 参考信息 -->