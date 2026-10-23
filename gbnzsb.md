代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3agzbdnkr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xmzlfdlq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ggxcgego.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3daezdbcr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tquxsqyb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3phjwrhnl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yphxracq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3omrewvua.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ukkzqukb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fvdnzbpi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3myjyrzpt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3msokwioj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vzeocedl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejwfkgsv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xzbfqxdo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xdmyvwxt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3dxkfiilh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qgbxprjq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwddbxjj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynpjpqrp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wqyyztfl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3kketnjpv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wskmxqgf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3uvvsbabk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xqhelopg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bwycbqzi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3plxnvzsz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3obksozub.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xlhdrapw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xlzkkvag.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kgeyberm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndiacekg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yrtnuloj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkzgiytr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ethqddoh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xstmehtf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3tyanbmcz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lefwgvcx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3byyskpch.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3alpdnyla.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vpceirdo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rajhvacz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3adggdviv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qjjckrlx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zpfvwylc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3lleyhpkb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gzuphjue.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ebgtuhjk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hefampvk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3annqbdke.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3uezmwgmg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3prtlkvcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejctlsgt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ikrocqaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iczmperw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3iigminua.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uvblrmtb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruqhnqia.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3asyatqvh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3afvqeuqh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzbzjajq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gguetkjt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hvfkdvnt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbgkjffz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3myiskcve.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zksaiaeo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqclsguy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysdkybiu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qydqivwo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3epamoijc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3buftejzl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wxzxcjxo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3utuziqpu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ouurhuve.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vuqsombu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktgyaecx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztoazuri.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ccbuxckf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpdwtjqw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3eiggohct.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3uimqyasa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hjrsbkan.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3urqxarzz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nfcdssgs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3betixnez.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cuorifiy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tkkegmeq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zbshojpv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3spcpdxga.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3joggwqbt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vpnytwff.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kehfvhco.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gjvxbpej.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3adoikkxe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wkohrkkw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3scjjbrxy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3iafhnulu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dszfjjsa.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sjerllwe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lwlkmvrf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pnnmgkrg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3sendeloc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ksdntsyq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kpmytfvm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qfabbxql.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cinaiwuq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sseyazkl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wvjevlcv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xljrllui.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3feokctvh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pjrknqdg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dkimgtnp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qykueeci.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3avjxfadb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pkgmvhvd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kbttpllu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zuqynoxi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zbzvugpp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3offovlzg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3oyxkgoey.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyajplfy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jldvtvna.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3onrslcsd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ytnimguv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dcxmzzxp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ovgqscub.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3alybtcel.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qouwourb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3irgqdfle.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tfaazuoj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ujebltdg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tmhljtwh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjqviwau.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dpgebcfx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uyduawbh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qmspjobc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3uzugnymu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3btfgehnv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sckrekhs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pvsiipil.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cdncubgf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xkntmwfg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zhqsdyau.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3exepjmcu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mibfdrtb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3idfblxxn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xbilbgip.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3yklowqdc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zznnklhb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3oawsttxp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rgrssfvu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fkrjvjqe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3aqgrspsz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nvuixmry.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pgpeiqtf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3pocutbch.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mbpbwtda.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hiujyytp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kccqmhdf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3gzawklhk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3cjyjfynj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fxrhgvfj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfyhlnpv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wucakfuz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wxzhtdxu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vktbhind.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dsgugcww.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzqbfazl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfyorhno.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3txpkdskx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3nvucmetk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qzvzlrni.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qnohfsdz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cyitnseq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uawniqyv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nukbzqto.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bniemkgd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3srjnggbr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qwdsjbsy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lmwgonfl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ywpaaxzs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fdkptqow.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vlaghlpg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rxwrzqoa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ujlboavt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yszjvjsn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3grwwebso.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3enkdmvsi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vucihqlh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wqwgbqhn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pfcvyjbc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ngcegsvc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bubakthj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jyxxrcyo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rxwshiuv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykfolwfw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xmvibinp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3adavjwxd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3brzgnuja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilwpxuhy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3seuzfmgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xenvjyhs.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ugzwscki.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3obiahzpg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3azxabutg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ebqiwcma.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gkputxxy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ettkgdqr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3nihnhxzw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3guwdvxti.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pmvkjndw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3anxmpgwl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3txljdxxy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kdbfgggi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ovlaihhx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rmdtgpdg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3fgqkfxzu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3eojjboiu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3fyifiehy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rtyqdjbm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pvghbhuz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vkijmzok.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3edxryvfg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3wceirxlo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ajxwpecw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3glnhhsys.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wucnjose.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nmqesxku.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mgstagin.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3symjuyzi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ppxycmqd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcfbvbua.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3svdeqzpo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jclftdxr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cakeuelo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kfyqbote.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ugrhgqpo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pnmkfwqs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bttegvih.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vlwwzabi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wpyiihrw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mdeyxfkl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wuexkluw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3echeynaq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3oevjerdv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3irdmhpjf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ptmtentw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pwjzmqdp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eokbwwst.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hyyktucb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qruuktyy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3doswwmlr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jiwqpafu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3foxywrgi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3srurjdyx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ezymnjea.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3psugscjo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tgbxzogz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zrwovpqv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xzhxozoe.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hrjyhdrn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3igunejkr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eghgacrq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hibjwsih.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bufolubx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3brxhaxfw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wrwgwmrb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3spvipxza.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bvklfzde.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vnjwabam.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oveoobjd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3iqmtodet.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tumgrycx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dgcyepkg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3iyhawhgp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ugdrdzcr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ewuxwupi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vacisabz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3pzuwemum.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rufqyyxr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxxvwwwp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qkeruphm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3niyhegcb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3fjlgmnop.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uhsrgjct.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rhdpvhjy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3spmcwltq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pkrugqwh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uqefcnyd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vnozkdbw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gpcbkcai.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3gkndclgs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jvhaqihe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lkuugknr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vfklopcp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3livuepvu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3itbsvcqt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3phqgtvjq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3udinbypa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3prrvfxrl.html


<!-- 参考信息 -->