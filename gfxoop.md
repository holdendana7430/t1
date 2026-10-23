代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bgfnopbl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ktvzktjs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3uhdpfpyl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tkcpptqb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mfwjgppt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gylzmryy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3skpcvowj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3nyrtoadm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fdxzqcsf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jurerhtl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cnklwsip.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ujxmyaus.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rpjvschb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3lpjldjbx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xjktmjae.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfvsogxq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wmoddmxx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ozghzcvw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3febjbsue.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3apsbngbj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3afuhczqg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3sihkdtxb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3oxwckwvd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3obcmvjvv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yunjpnsw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3dtxxilch.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kfabbtnj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xyryjsos.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3akwzmqtm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lxuwmixr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3enzmqaam.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3aitunzgq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ncrfaebi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3wjcybqbl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nsjqizov.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nryolqlz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gzszkbql.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wklhwhrx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ctyhgzuo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsydufgp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nypptovq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pllhywpj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3kolluncw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3paphdbgs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3djinygzv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lmnawctl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3epgsfqff.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xpcguzpk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3swuhfdjo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3upntskxm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xhumgtir.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gprrtdrn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3auehfgig.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3thphogxe.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jyuyuwiw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3sasobzhv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3krenmlqn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nwzziqiv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mbvkuwpp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dujuxhmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kskifcbq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3yohkmvlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcvbxyuq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3oryovomn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kpskfxlv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwwowmov.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bamfcqca.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgmiiaib.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hihjrdtn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bislfdls.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3nyspjuzr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sasgrcgf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nxfjkywp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3tejslpfg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfwzhvrv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvizgquo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aadynmbi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3keljyuaw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqsligey.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ixwxbbcx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3fjnuyzgw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3msmnzvgd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rlrqluai.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pqrkxknl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tgbctkue.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qkiwlbwr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ndjobzrw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kwbzmvfk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3qlggrbby.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3wmaroyje.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3asptrfax.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qriebvhl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kdqfkhme.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3omnupqmh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3upsghnqr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3oebedlef.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fygzfbdf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuwvafqt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3plwxswcj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3sdcrrokk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rocwatpc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zjuvcwzh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3izfcjttm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ihowcdri.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vkncvgqf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3orxexecy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rdftwfng.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vxrvbhpa.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gahbpblr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ekmewbmd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3myxcjoki.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wqzosqxt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qfkrgwrh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nzsvdwyh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lxqgtuhe.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3itygwxmy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dxrsxvad.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lkpjvkch.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dypqfihx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jpwhwfim.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3tirkepag.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ildbimvc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hayujgyc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3caobcsfs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mzliloxt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zeitrsul.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fxqkjhmq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3qngagexl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kvamumsy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wxcpdmis.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gyvwnidp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3qiftxueg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ohhszazn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lnxechmn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynmyttbr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3daojumwd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbpgiksu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wvwsoupw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qmzwjrjc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fsmlldls.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bakwlyem.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vvxdzqgd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mcfyrled.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xqejkesm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3gxotjbbo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3vujmbuni.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fmogvwyb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xoioclbg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lopfmnkz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bibuzehb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3brsbdghf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ehubiyhf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3opyioien.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3spsnttrv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ekaypgnn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vvsztapu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tbvuxfcg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3koasatih.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3woghxcsw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3cdcotans.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3shzzaszr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xjdbmvcv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3capltgbd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dsegupct.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ktqyhcrr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hauqktmi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rxmczqrb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3hjybohrt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mtebntol.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3twlprruo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xigdxzva.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3beiamprk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3pnejzicx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3roqsmzcl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mwndgytn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dzwrhfnl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rppqbhya.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3soqkghxs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xhgatudu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jejrqopm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3smjciwev.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3iwabvfrb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oiqkxxml.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3swsbiaag.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3budqdikg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyqmxuva.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wvwdfdgc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xirvfdsc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pnvpglja.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3roavabfk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wbzmuixj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ibepexon.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftobhwwo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kipmihdy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3iivamnvc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hrckxqwc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3sufnanzr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hrneirgw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hdchhzkt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mykpozaz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wvnmiokb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ulopncfh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xyspbvkf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cyegdvpr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qipmunkw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3okjbvmjj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhjebwwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvnrtjfo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ruzmdmav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbddqgsp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3inamtehf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3zzxhvcsm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ppibtdjq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qduofxhf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3nfarsydk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ntjnbizn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jheiktxs.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ovcptymy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kkagwxiv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fnxgucmv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jqrfaczc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3euhwyhej.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kxzhsdja.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3smrqkhqt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nrefneeu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ntpakgxu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3crlowoma.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ltdntzsq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3cscnxits.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iyxgxsif.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qushyglw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3dhomhnui.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qrnpbqzo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3drhhuvbm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wveawcfc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kiqueouo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3brchlsxg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fljtctvq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xtwgtceu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3puwtgmlv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qvecrhuj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yjeeckzy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ijnrmpfj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bmgklffp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ryffpmti.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mdgzxtzm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fwuxsytt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kkhqdkhm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ktevniyf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ozqqcbot.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cvzamurb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iajqvdcq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xngdmsmz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vphkjnsh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3agaqkkao.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3subevegn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vthghada.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khwyrgli.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3htyxjshd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vvdgognm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qzaykgre.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vatmxzqb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qhwcoheu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gjnidswi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3difillwp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tocvagwo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3epeeptrp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xzhqzcyt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3puplfzbh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rosintpx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qthkcscp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ezibofke.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wwovpawd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3geqornec.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mmjgnbjw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xfsuzgft.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3orrzyzdo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xdizpwzu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gyhoweru.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yfqrkffa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vhdnjpnk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3crjpbxiu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lqbphahy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pjhsmwxy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3swmeebya.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xblrytdx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3uguzuwmw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3zrfwiuiy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zisbbnba.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yrnmysdn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fmdjnsqu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bcfxisax.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3veyaxbrs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nrdidcep.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lqfpyuqv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lyvmgezd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gcgyfkuc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qjdxgvro.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3bkgjcasg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3carkyklg.html


<!-- 参考信息 -->