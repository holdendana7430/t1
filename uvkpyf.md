代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uetuityv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cbyraljp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xltviefj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lweiezdz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kmkfirpe.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2emvdniap.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hhpxyalo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cxlikzil.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xjtbaobt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2osxanajk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2atsiecza.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ajmuqlgn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fbhbsmdt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hiolocnl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2fvdmftno.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ustzunin.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2buicwxku.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jpbeifvf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ddmhkxpw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vctyxknf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2upxhrsgt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2klfrpoen.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jkedkpwu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2peqfhflq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jvdjdoya.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dlpqrtue.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xcwbuaxl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2pufczsqb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rmfuomzy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2maswdqxm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmwrnfko.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qazjflyn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ybdjqwtg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xlpsoxrj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nwmrxsov.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ecmutlfc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2buelgvua.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gpeekxme.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yjkvextc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uysoailt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2txciemqm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xxvepcee.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dmiczdkh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nkxdutcl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2evczgkuz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2iabzhqrg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zdqdbgbm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vzaozdhw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xceyfnma.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ebgldbia.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2gafbukeq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bsncwnan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2betqkwsv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2itaehfib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duxxogmx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jlxgfzrt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2mivfzrco.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2knbcccnh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nprwoykx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ozzbmzlt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tfbjwpba.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2yptkkrkb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zjwrazdb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2awxibclz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tpaabxjm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cgpplhbj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmzgmehq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eafyoywv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zlnxsqoc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vsfmkgcj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yxznvjuy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jiqlevgs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2oxxomtwt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rxgbwddq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2erbrxsjz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wsfkybsw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2imhhjryl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2spmivoyq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkvcraig.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2reilexux.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jehtmwjx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2nuozyluw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2txvnvcur.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2weundomm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qejioqew.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2saroxpsl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zgdfqeyq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2bzofffow.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2lpftlnww.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rdbgixly.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zobckskf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2yntdukfm.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ebkixjyz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2uyvssudq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xxvlrcvm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pbrveccz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jzsohmcm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ektbghie.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cusdrifv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2nemyatqz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2peffsmaa.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hibrjotd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2nzfuqnrj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rzakurjd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zvzervsn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2blojnjig.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uhdvvplt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zptgtegf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fhgfnpou.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yooalvjo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2giygiihg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rjqovrte.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mjsawgvs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yvcurswp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2iympitqs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2evmhikow.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jaaidnzm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2szgpxojg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ghombjnr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2bhhntlca.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhcdxzqm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwbpjjxu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uksvfgps.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ofbcgeur.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2iiwgcsmk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zamnvtzc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fycztwws.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rvvyvbpf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2crjvtxfd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rbzgwqav.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nfptxzrt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2euonlers.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bqlufsfp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ihvvfnwf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2utragsha.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ajbnkgdc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vtobwzzp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2bisthkgd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2fmxebpsa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fhalnsam.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2sdypipue.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pzsruqhv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fknjwsrl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kxsttxwe.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2emujwkgt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2aalegrcs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gnuqakka.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vsbhnokp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jejjphvc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kggtjyex.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zfjmvwsj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2uutxozrm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zixeaxca.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mkfzefkm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2aczwhxzy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lxhzjmmq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2udntojsh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wrkegkks.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xnhfnmna.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kfgxownb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zvoxfrlp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pvfjecnl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xlkdzfrf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ytvuniip.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ekmfwfea.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hgbljhqu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kfvokvlb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yprlabnl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2umpqdlpy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cydabwas.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ozpsaukz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2etqkyksr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gndgfrfr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ybmrqyde.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lypxpyyc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2betautnh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2czfdpvtu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hbbojajn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2xkputosq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hswthkac.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2votxovzg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ydtbsevs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2txnbcugd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uzfdyshj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxvjbwwo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2olzqqwli.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bsilrrek.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sxcqhcie.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hotvildg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2httbphrh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2efqhytxf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fzwfcrpa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tpwvqtqx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2mufmfevp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2gguybbfu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2muzskfti.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wcqimfrx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2wuvwajvy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2njqyqmbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujcixves.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2cgkqzsrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwstwaos.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2slevpbtj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xzgyjbxx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2akihoxys.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dfbzsdwl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2znnoufnt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nqzilmzz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nuxgxvri.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tefutykj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2meqlwcqy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2iswfxjft.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2irivakzd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2suiafpgy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rhdloazh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zswqqhki.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gbqfkkqt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vrkyiwmh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oiwpgqmu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mxwzfwiq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hwibpzdu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rxeltgnm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dadhwgrm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2iyzpwolu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jcztkcik.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kxmlndwv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2pijzgkxl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vjdufxng.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2flmfpbia.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bhirixlv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qegeudww.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qzlzxuai.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2osozersz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mnodlkdi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xwqsrwar.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vijeosqf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gslgwmnf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nvqyrfus.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vitojrxm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rktsrztu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cxqkppan.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2juagyfpr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qbzfrvqf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2cpyhbnyb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gynviqrr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2flzgtrpv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zhothctw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2znidoqfm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fxuzzlcw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qryhmrne.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ibcypozx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dwodlfvp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2valrcdbf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnuwkzoj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ureonqsx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2yikgvqiv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2unmkinmo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pixjhjkm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rizjbytu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lbsyrvfn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cclbvthy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xezlpkwz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2dcfhlaov.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jempvigj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nvocyjid.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jkilkwxv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2etqammpu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gtpcaupr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2gopsesax.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nkhhihek.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iivgvhpg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kydymiqh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tcwwjtwi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dckpuwag.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2eurxinjv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yukbhgxq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iaxgawsd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2zrcordms.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xcrlwzvz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tecverqh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fvgpvtwg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dwdnzach.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wfpueaao.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mnnhqbvs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dysfxwfu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2esehbzht.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fgkwiytb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dndwqvls.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2akjuyslv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gayjcvhs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dyysichk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2dpeeapik.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vivqfdhl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ftfbyihw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kdruloio.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2itvmexum.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mozulims.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jetvepim.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2khdrskne.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rdokcpjl.html


<!-- 参考信息 -->