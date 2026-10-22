代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2iseiazlc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lhahpvou.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hpxwzxgs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ztmfedqf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wjmfgrib.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2agyxiddx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yvcvsdvj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2izuczwlq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nwcyjvel.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2duqqixid.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hqxjmgro.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2snivutll.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gswusfnp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wruexohk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2upbgaejg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2leaygego.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2trbqvvwb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vzcamunb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2oqmnscaa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctgdnjnk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ehifbxaz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mwylycek.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vtifkjat.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wmwjezuu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xlbnqhxo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qezstzme.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tshnosyp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ohqxkrhh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mhbbsvae.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jfkoflna.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ioixdnxf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lphesifj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eodzngwy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mtfvkboj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xihkrewx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lspztcrk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2cxxkswmu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oqiqlgoz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gduqwpyj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xnhmgpav.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2orpipvoe.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2okrdzzov.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2spdtueao.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hicfgavt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wjqjknak.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ucnrthkk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qdrlkudr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lgmfnwzu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mhzxhves.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2osrobsyi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2udbfxyrc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mjvkugbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtpphuhm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2udldimoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljmxoqfl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hblrlqow.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zwatlxlh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aivmljsv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kqfqgmlf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouukvawf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eotzfmhv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2reecrvav.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ygiovqat.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mydtlhmp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sfxncjiw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2koxgwoyj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtclrhqv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2icxrlywp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkteichd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vwdozoys.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2pixsaovj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2fdqsjqxp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nxpdqsim.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jhmplrav.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2avzfsuql.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nxwvtzjy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffwpwlih.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ppgevcet.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2knzragub.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hcdrmagj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mquqevic.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2plajkfiy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2enhcutwg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fcpxhsdi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2qkxdpdhy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ozpogzga.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2pffozrau.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vsvmxlaw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2cnpmcywy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iubpnovn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kccjolww.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2skkjbhrh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dllrnovg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2dvdcrxua.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iwrwyvmq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lhpqewuu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2kbwvarkr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2aotsubkb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jzqrewmo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nlnswcse.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hzbdszki.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2umicukxy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2cztkasxm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jxvmyviv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iujtihqk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vojqdbrs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fovpqvfm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2orffuxvh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hyzxhulv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2tzlyqaaw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lmoukptl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oqcpvcqi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2empigskk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2glfvyixq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fhktenok.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ulslqncx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2imkuykfn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2lolcfxwm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fwqeoiru.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2fpdvzmkq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hqzlkvvw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpholzvi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmqsxteq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2qpulmaik.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2jgcuykjv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hifozvlc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bgtdmqio.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vqmurgzc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ugnhbzuk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnqjupax.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2oubfldym.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ygnxmsig.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfvjhlwx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qomdubku.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wipbiqxv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yfwwogrv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2axbhsfwp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2yongnlvv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2abqjrgzo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2obcoggtr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2msjibxzy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dxryypev.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kwvpbwje.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jubixjkc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nzmrjlxm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2plstvgxi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vubqrwyr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ifpcmqrl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2biwipskf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2khaihiht.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2iecemcrq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2oznkjnwj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zvostuxz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pzixicid.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ynaoaykh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ynalehpt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xhgderdc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2osphneoq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xzezylmn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hrqerylr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bvpearoy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gudkmqev.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2lgwljlvu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kmjqnnpl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mlfbrmyq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vfsvdksr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mltzbknq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuwoxwzv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zslstbnc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bcckfayo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wllnmwdq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rkvqmfcb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfgyzvju.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rkblbmhg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kgzunzya.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zzepokpn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hfjzhgbd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhykvwyk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2xzjuvdyk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ncbyimjq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qbkmsqbm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2fnjxdsnz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2oquhpaqm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kbajuxgk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcwtsxxm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2qtkrvpnv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tfdsbemm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vugyqtpx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2auhfmivm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qxtkqugn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zhebxxug.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2layscgma.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ftafqpby.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rwbkzdmh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rrfpnvwq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwsmhozi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cnppqoun.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2omsuwtvt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ubvjxwhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqizprmm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dtybhgsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqrzjgdm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qfdblkic.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ehtspnua.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cvpoatbj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gahhnkux.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gsluvdqn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iixcokaa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2oajdcipm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ipdnxquz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2sygtydfw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2zohcztvm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xyjajpej.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2kfjhhzki.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lkbakxdu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fkyxpdap.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dfhfvkgz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jxmxmyvr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mqueufzc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zsyqtdte.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2brcieapb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ipwtmpiu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xmikgmgn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2tygpopko.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ziifotnf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kfmzvhhg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rmnzrxqi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2iiwsexqy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kaumtpth.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rgrpsbqq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2djcgolcx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ikzxqgyi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2abjojbzn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yhfaxqgq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2puciuzbc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2klltsufd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xmerhdlf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ccjpyiky.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hboclxxn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xezwjbku.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2neadmxcp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xkksdpii.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2aintjbdp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2mxgpqeen.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wutisski.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ldbdrdyf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ntirioso.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2inlcllwh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bomcxrqb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bstdsdwi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tdjsllbq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xcugrwtd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zigtwnar.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uxppmxhj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tqqkwbdw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2allaeznq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qkylxili.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ftmzqmtp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gtxxfoec.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2owtdhwpf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rilltvjh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2osamzkzy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qwfgxsiy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sxshseln.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2akkmkorp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2sdhostdf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ijvjhqjv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2grqzjlkh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2akrmsuiz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2daoqhrti.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mkgsvgqg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jpgaimwe.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2slsqhrtk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lvnpeuth.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qsjtjxmz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bdxyfrgp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rocoibhj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jqyqgrqc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hmiacbug.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2nszsyxjr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ytxkzgtk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hjhsfllh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hkkjlpyf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2cjsvxbsf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qtxxawyr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2acaefzcm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tqijcbki.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2titgyhfo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ncvokrmf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ljycbrij.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lbwmbnfg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2sjpqefuf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2kjjhferi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2hajljqsq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bqwgezhn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fyiyovjg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xogaipff.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sayawrgk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2sokeakjv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cpzcvtko.html


<!-- 参考信息 -->