代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rsrdqwdt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mtcnvnqo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2oqivnpeu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ivoxxnzs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2pzfzcpuf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nimqzvjn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kinhqlqp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lghvnxvo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fnyhtrsa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2gdlcrzab.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hijhrupn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pkryflvu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2akioylht.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lsyuevvr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2smcjsdri.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qdkukabs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tavlkmjz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ltovxpfi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjsolorq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nzzndcwl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvqiyzzh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2kbspltou.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2feasrhxq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nyqpruoc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hgcbrtpd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2dztqejcn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xsbmcuma.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tegzntcm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xuvlrgaw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2szeperyi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzuffpkl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ipufaakv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdwtlysv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbypnjfm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rsdlohdp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2usseqasw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2jpbhbhmh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pmrjpufg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gzdwvhyk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cuxpaiqd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gjrjxcrm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fvyppxjx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2olkpqbib.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nhbknlfv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2erkiqqjm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifdicirc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hcbcolyp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iyagyplc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2trwyqvgr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vhgcojkm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ewftyche.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ckmethrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujhgpinh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gdjeteow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrlupilw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kdfkkncp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2siwwekup.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dszejuse.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ovdcozkk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pzbwdhjg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hpirmuoh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rgbpuggx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2hfyvdvxf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2thueyqjo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tuklcirh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2tnugnpom.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wymangbs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tixhimzd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgusomip.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2voqaqqcw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nigzjhnn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2harrwllz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pfknbgti.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vsdkhqsl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2dmnxzsmf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wwezgves.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzpqezch.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmecxwpz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fjlnhjhj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2luhooeyb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2uuaipqwb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gvwuyatg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2khjqljay.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdvhaau.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vmbqvfjo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjdaggch.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tqyemtrq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2hlkwvfik.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vbxygiqg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zqgtssxb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hinkqlhc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zlbswlfb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wtdojitr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mrobgqpn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gftcbrpq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bulbnpuu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bkhxbsvj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2euuekmog.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2noqeavuo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gekurmxd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pqhphpfp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2iwfahyzt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2chzspfgn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gaceaefp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xmubzesk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2helvfesy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ezmjxnol.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2piwahqkw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wmiywjmu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2bvamtvoc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2fobhuoeg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xsjmhona.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ftujzcrk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2mimccrbk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ivmzfniu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ilpwujyy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bnrqqpcx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2edngxwwq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zooknvvz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2sgfxdivh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2rbjwuesl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihllzxsm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2umgyodpt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2bhdfqaee.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pjyzhloj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fppsdleh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2phosllnq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cfxsrvow.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lrvmhsic.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2obmicdgy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ulrbgvdg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bjnnlmvw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2akupdecu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ypumvnyu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2utfvcxew.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qazjwgdj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xnjvspdf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2asudibgh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2erdxnwrj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pmaefmrd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zborhpwl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xvixxrxt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rxzaxpqd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pbcpzfzb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2eojgvsgi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2oyttajga.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2tfmkknhw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gxadutwa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pdvgmxnm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2trkiuvay.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wbmcexom.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wiftvuup.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2shfcxzkr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zunxgiru.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2eeanqraz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lmolsrma.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2dvnfnwew.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zqnmfgaa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mosigezf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ufdctqtn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zjktblhr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2hatarnjt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dfqyudpg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2vieijlwm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2smjkcbbo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2juuokxad.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2roufrbpu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjqwgaye.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyfqmywl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mgdabvip.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jtajxblw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ejtlanqm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2aivzsvov.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jodyppfn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cwrpgkmc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hlezuixp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooclsbmg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tewhymvv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2pkuoqtbn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nxbqoxek.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nzqjomvm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ltqulyim.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xbsvzmpw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ocqqougz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2prowmnmi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udxjtsza.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wlmzjrce.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bdpekbxr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jbyonciv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cgqcisub.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2vpeyrjwh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rehjkifx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2dpvhzsqx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lydwvuhv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mcqlloqs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqqqrcvv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dkqiaakb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tkbhqduh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nqscqwyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpjtugbw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2rnzynfip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eawsjtma.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ahlibjtb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2sgyidnvi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vkwxjbus.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gbwfjmkt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mtnhdksp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ekzyvqad.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2jayoojtc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ccltyrjh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wpcveugo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2asugpifz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jgvxnxtu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rtzrutmd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nsqwvepo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iomnmqbo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2siwhbetn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yarvlvdh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2aqzemjqu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2onscckny.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zmqwiwde.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pncivdti.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2kpupwrlw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dpxzdbsn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ugwmpnyg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2izlnizro.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bykausix.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2yemturkj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jflqpapl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hsztpria.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vzmppfjm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mkmkdqnh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ovisrdfl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2sbqmjxbi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2heqygszo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bysfarzy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kccffzej.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2srftmekr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wcnozdqf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jnnxnvyu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qqgqyvcl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uskvrunc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ivzvdyjh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ththjbym.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lgqwbrmm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2osssrcuh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eqlaiqdt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2exsywofu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fqbnviuv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vgzzqqwx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ztrnaphc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2opvtqnmw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2sciognrk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gjuqjwoe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2cfjpexlt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ignhjdqs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ykftgybn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2atxiqnmz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vjbxcbur.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yjqdxdus.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iqjqrlaw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xjlajtaw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jngcvhyo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ojihlxvn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mgvsobfv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ocgqxqhb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2irlkobyq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fifhkbjr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ekhxlvdh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2eoqiapmp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jtfbaqdr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hzxxqxvx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2smxlcenl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fstvmisk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uwlbhudn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fjlnnneh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjvekgen.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2xgpzgfol.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2diafoufm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2lzkufmaz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2egsztzbx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dfnjgozx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kexugtra.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jntjdobd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xdcgytxj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xzdrfeqq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfoaiqb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wnrllkzq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2enwfeawj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ijpqntqx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bvfamkmr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2woaueqas.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2eizjrpci.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wcormpcc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zuyiamyj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ppjayvxy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2nksgbboh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2prtpbwak.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wnbqyqmb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tsxnnozk.html


<!-- 参考信息 -->