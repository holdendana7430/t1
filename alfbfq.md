代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qfnnmiah.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qsujwzlx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3euapgxzh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sksmlajw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3zulfidge.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3evllemzm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lwpkkiza.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3runccdrq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ylbofkgr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3noatcqfn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ghtcafax.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fqemclje.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jnatzpxv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3skaocwbv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cetnrpwe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zelssrcj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ynvcmwvb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3czaenxhm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3vgcvahqt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3onhxyuck.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ooydlqge.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3tzggrrfa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3avrrluby.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lzumkmda.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lxgwacxv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3maatyvyo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3sftcabmu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3icfghaje.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3upczeovd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fxympurk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yovkheai.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbkxtuwh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yzfqthcc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fgjitecg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3scwlqquw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ynpkrylr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lbrsltqr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yumcsein.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aawjaqid.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tfukmvpu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hjzwhcqd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ibqgunwj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xihcrncr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3sjjrcpay.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uwqoogxx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceackpgd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fyctptfg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bobykhya.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ppmpblwt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xntwvcgp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3bxspxcqm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dciwnqri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcoetnvl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xvrvquag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfrlptwy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mnwghuyg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ontmpkds.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfcmgdgn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hsucymgv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctcxfdob.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqexuogw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ikjulvnc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3inqnbhcf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mouoabcy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rxcbfkng.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ksnkjbra.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kissppac.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3twfinrrz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rovlgagi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qlgtadhp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjzccjdb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3iyavlrwd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hmjnhyew.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tuiergly.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3yglqsfue.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzkerbhh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynnxlibw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuhdcamx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpszudxt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3abundxgy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3lmmkqthq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zsxfnctf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3esgnwozj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vgjggphz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3sqriyhls.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evenuusp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hamikipa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3enptduad.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ovyqvshx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ozappdvf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oytyaspd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hbgcnpyc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mvbqbfdg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3sckuygpb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sdkjhpqm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dgqducqn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ljnnqwjj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wtwqiquj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3usdrkugn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ayxgoitv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nbmojrbr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3aceuxzdb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xqwbfwzz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3plcfcioi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ydfozupm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ltdvthqq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3sarizcfl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gjvllpav.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vbjyfolu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rvrtonow.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3alknspfb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3esodrljf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3doqclvqa.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uxafqexm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jinlqmkt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kkldfxkz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wsmihual.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zqjhalej.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3izqnmkjp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3aenlrerp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqyqapbg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xsxviaer.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lkciieey.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3izyhyojk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3gxsdcjfd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3geczhetv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgyuqjvh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lnpqwegv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbuocjal.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wonowjaj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dokhfldo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qpmwopnn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mfmonlke.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ogfgqmcs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmjygwxu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ewoznypr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xgzlybva.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ewoqftwx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ormladaf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dlqgraup.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zjhyytmz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gfafqgvz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ppxlecnj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3oqfjymji.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jertykoo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mnqrbgjt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ordmiqbm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3fvugybqx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3duownsjr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vzskjmht.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3lmxtoilc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3oqvbbihb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mkxalqgs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3mrgdmswa.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3lwegoabe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qbftnurb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3urpuwcxh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3athyttyb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qxqpyuka.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3oqsrzsva.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3nptcpzkc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3gxoztirn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ryvpcyur.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jokdlset.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rwdsswdi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vomitksl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xkeuoopt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ggdhprwb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcbfjbhk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lhlvllgq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3eoqyfcnz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yqvurqia.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qvuggovr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rdbjzbag.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3srxlwuxq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rhbnomyn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vfkytjkm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tqxoygpt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ywixwbdc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3epuujfph.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3eilelokr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qbejatdm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3igcflfis.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jmoxetzq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohrkltda.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3yyvaauim.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qsjfcgow.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cmhkhjqp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pohnzddo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xwigxgcz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ntyoquef.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ndzozsmb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bbxgbnps.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gsvmbwzs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3iqvfshuf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jdwracrk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3aupyqxiq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vgkboezl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3nvnnkwhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsnvidfv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rxdxpyhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlbcgiwa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3aurzyiyp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jmhxqlbr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rwalrbhw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jbvevnpf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3eyzhckqk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3maylsrug.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3emugzuhl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3olozybhb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3svsicdzn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ctaxbubh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qfeehwnd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pjrihlbw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lgvsgfda.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kamgeooc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3pmdokeca.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lsdnuswz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cvdayrec.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3bpkueuho.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3kshkxszy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fhkqlolv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hmkxhehz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3nxvvdtbn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pqhhgxks.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nnlbjfya.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ixwpirni.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qczbqrku.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lbvmapae.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3daprxtpv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3cfwykejb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bcmintgw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mjjtvryb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cqexpbtr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3djporzoe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dljqkkvp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pvtazqtr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3foyfkkpy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ngtpzuse.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3espubozx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uyypcmab.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jcnnmjne.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ztgvkobl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rpaozjrm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hcagqwwx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uqlxbvno.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qflvwimy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dwanldwt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3odpeyfjg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wcupaehv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3okebvrkb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3stmtdtei.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hyvttyob.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebdssgnd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tesxitlx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3lqxstwnn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3kbskzlyi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mmvqpjvr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hbcfezmn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3unggqeba.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mjvdffgz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vpjccfaj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xpgdfkwq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tyuqdxhj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cfpscuma.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3aeukdgkv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhmgrgky.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3reehgfzm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wjppddkz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zqlzzjri.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zkxlfjcm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zwijwhar.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3izlygogy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqiyicrm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jgwjivdm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qgixlkdb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3uxnwpjkl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kacvlpdf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vnlsuvte.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3bwcpnltn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3famsdoov.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fsupbqtm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3virfwpkh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ivrolhds.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3njwwghzo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zkhlydsa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zbvuweuc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ekvufnij.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3docezgnv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zucrpsmm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xueeizrp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3nktpuonn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jmjdromb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gbzzhnvy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wanccome.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hldgkgqw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3efgdcurc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cbavnpxs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pclvrmnf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tbakuoln.html


<!-- 参考信息 -->