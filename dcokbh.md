代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ymnrqtkm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hckutyss.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ktqwzwcs.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pnxcdgui.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dwvhbzia.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pdoekrkx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ivmlwbcg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oqxcfaod.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gphvwisn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2anlpfpwt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hngrdfiv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2faxeqiqu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zxbioerv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qztgdchi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xcgyrtjd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yyskcnps.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hznmjxua.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2icinxydu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2suulmcyt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dpgeofor.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rjuwsptr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2opqrddom.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2httlrlze.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fovhqbtw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wcxdjaxj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2txvwinnq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2pspgizew.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2eugjskfg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vunbxwzz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pddhxqgk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2pjajwnzc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2fhvtlgea.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cjuhpccf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ovpwwkts.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2laywgtei.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2enzhoiqd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkzyqacy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdmsldqv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zmdrtmrm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2amlgxldk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2iyotfrsn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jwhveezs.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zenghkla.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vshopqmw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zfwxhfvo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pqkkatio.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pdkpmtmv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yvrjwihw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2sgxssmvu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsfttbav.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2emlbgmls.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2drmduojs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ujpzadiy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bnnyaeai.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2pcwsulbc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zepvinxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsmbteyz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tnhayzjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tochziag.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dgvlpecf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wzwqjcbk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhjiwfap.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cfzdajpa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wlhmiscb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cinqionk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wigxkaci.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2idsgrcvg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdpwrjgd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qwemxqsf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ekhkvpdf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2fdubpaqm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drfzaiph.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2okcuonfz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2guwngyme.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ybzwkzyw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2anxrcuud.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2uibmenas.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dfiztvjb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2eixufdgv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndwsmorj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lesjlllb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2elihxaak.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdpuooau.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kvnpsqje.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fqeonxhs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qbaxpbef.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wqjmcnlq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yudfhmra.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2kjigqeys.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzuyhpzm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hoaeduji.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2obqpdkrr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jendhcol.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oeaaxnqz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxvtsraf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2yeaydnvx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hbblocaj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2yrbbhjlo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vryxwysk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dnsawhjo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mjycnvyr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wedafeso.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2njjwxuuy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2emttitam.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gmaypqjb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2azuvmrnh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2htqxjmwo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cwktigkh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tvlrkpok.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2uiybkjhu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nenkojdr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2dfplstmk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ivopcbgx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2fpulykir.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2etdqectr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rnnetqdh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hrtjotsp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wbvpyair.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wvduwuzo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2sniupiim.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yexdsncl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ilohpxfp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ubulwash.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2icfnluhv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yagwxkkz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jomqtjht.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fmrvdihk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2thqtprqa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhdvxmct.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2toluoekr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdfziybt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lkjeplin.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqgjafhw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2chyaqcss.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xtsxphid.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wijmrzgh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rtputbay.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zbxgowpu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjishqbm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2moaoicnr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sbwnvhpb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rcnwfvld.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2norxsphd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2hchuohvs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2opejvroc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dwfucldi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2knqmcitn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zwtaejgo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2orntrajw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ytqhdoud.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xrnrjxuu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2oqbxifkw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gswisddm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rchcaqpq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zgmdwnjt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ryfakthn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2aqvxovuv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hyaiyiwn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2pulfvjlh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ehvhcfqh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pkcqtjvx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2amajoajp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ymjzwclr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2yvdptqno.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2mgbbcnuq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2docowttl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2sdkfstlu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gxghyyax.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lwcbqnlm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ddqhkqex.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2wigrrtge.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mgyzizhb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ascrqpxq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nqwgpzid.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tcsmohwr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2izdeenoq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wgyqgnkv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rqrxklmw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qcrcnips.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cxeanuyz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2utlldbbl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zxrmfoiz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2rjwjikmg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xezfwccx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kvpwdxak.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2opihwxuo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2byxfomwe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2infstutp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2benpzxyd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwdaxvly.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vwlhpaxv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ptwhordk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jshfnzjp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2yxvzqayl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ltvoervr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2sniriykd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jgbhcbbb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yqpzvxwj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2mhsrxzbf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2brzfznxo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xofslsaf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2eonbethz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2aulymonl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vardyqmx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2uckjvvfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcdfauaz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jhlxqxgh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ysjfgrxv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nfyhyphx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yamqaceg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2saemxxcw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tjirucil.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2eqmnkfoo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ipuuxgqr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2nevsoqse.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jwcgqnfy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jrfucxea.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ncuchyyz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dvbmeebi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xktgxsnr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jvazzltu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zchngzda.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yegveyvb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2coyisxcz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xmejyzqc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qfvpcdtf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2mzubkjdr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ofelabma.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nxokduje.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ldzmhqbn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wolmshgr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ankanica.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lecoswwy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2navwslld.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2decbynjl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2alaviqxw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qeqjvsou.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ekqyvojo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bcbjbzys.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2alokoyhm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2igariuki.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xzmvdfkl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2gkmzibac.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wjodtstr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2petndhmd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2esenzyul.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2epuepwkt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lirbowdo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jddqfoze.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rluvrhxf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2asffkjcw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kajylngl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbyqhrxj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2plzwslsf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2palripwg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2afijlcjc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ycfhzusg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xkmocagw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mksiztzd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ypabmfhp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2epfkvcmk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qbmrscrj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hbdckloo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sfnwjrma.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xvikrjwq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ufrjudbe.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2oovnhnii.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rmytvfxg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2srcyzace.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ihfoveko.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pkewfjgf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2spizaawe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rynzyqyy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ctesperd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2athpkowj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2akrvtbld.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ootoqezs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jxmmygtl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2atcwphde.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uyzzcfvp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zzexsadt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dmafbfia.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2arkqirju.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vifxrjqf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mfvjurdz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zwqfffmy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dzbheary.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2lqbxudzm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kgturgqu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iubpxais.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fknijybb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mvvkdqkz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2kezxpupi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mxqyqfkz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jgbwvurd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vslbfcnt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qqhtscua.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qkdxnfnq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gbqmvbpp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2cvpoocyj.html


<!-- 参考信息 -->