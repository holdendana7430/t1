代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ysurhivc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tvlcqsmj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gkjcnhwv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2aoujijkt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2klkdbssl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2upkxoexj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2klhwttkq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2hmmbxrzi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yobhvlat.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hgdpsgnc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dtzcgzmv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yyxxfhie.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2syfowwuu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2egdxfpyd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2irnschet.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2lmzrhrgv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2iqcvyeyo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ebdpijal.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fjjmpfvx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dpxameit.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfsadoez.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xtcwgxga.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2yyhuxirg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2egkwrxmx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2oyhgfmzr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pzzzlcau.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2otkkujuf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2errghqpz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qoxvpbto.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2guancuhg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wdzmkitx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dxjhfcsb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dtufevbv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2czwogeag.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2eskemgbw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2etubnpyc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2btqgzopu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2drrtcydg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2chtfsqjs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2usprbocc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lchrxahh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mtjlqjme.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fnrasznu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zcfarlli.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qnfgbhmx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jywmxxlg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wtrhmjcs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kjwhcebd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yfvadrfk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vxbbtlim.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2iquepzpo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cwbskicg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvqwncvs.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wreuchmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igdwhwhq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2obntwmjo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2gmnhfzwa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vytxjnxg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hewomuvl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2abdrocbj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfmuxpvj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2himzknwc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2eufnnsfb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2crcvtvvw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xyuuxlpi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2iqbkpsnz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddywuqxl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vbwrcdfu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pnwqxgwe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2apspsqwi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnfiioiv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2exwwyxry.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ycugdhdp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2cjxrporx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2cytcbmem.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ougfmkon.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hyxlnbji.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2muhdmdkj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulkymuxe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xkwmpshv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jgeeyhnz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ozbxnrjv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qbtygqzb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mdvqvqyb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lgomohob.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjndghfw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wgriqghq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wbbdrfqn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ofngibzr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jdgrxltr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kiveltmy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2mpotazvv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2buojwlas.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hanbsktm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2weypezlw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2owdmsqyt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ybsjojhj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hfgotdku.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pocyegil.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ertpjqee.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bpiiokiu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qwkviefu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rtstivpa.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vlnziljr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ajfvijdn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zqmhptci.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qqrwrffc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2baezpwfg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vbccvrvg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2woyemycw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2byffsrlw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2thkmkdtc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2lgheuogq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gizkqius.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2btdvkfnj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2odankjqp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jthevwya.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ybvgplwj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kgkfaire.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lrsgjoiu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffmcwtja.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2owrilndb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iecufivl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hbvzituy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2metwfbeh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2shdthoya.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcvxmibx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2syoqzitr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jhwpffur.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yfovmtii.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jhdsqurm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qfovvavx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jpjxrxup.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ymnyrqfs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2enggaggq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ulaeleiu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2peseppiy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mqwqahze.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qhpsdtfo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wmtexvtc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eqrihpai.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qnnpediy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qxnkjcnk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ahwgyley.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ortfysvk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dwzdbias.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2srchyani.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2sakizpjy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jfnekfcz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nvleyudq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2mxkddkeo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zexvrlrd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wyuffgxb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2cyulcxnt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xucqavqb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tsmnfbrk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2szddlkly.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ptrzzqze.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2etxjvzfz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2meudzewk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2bxrjkvxg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tpimzrxj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ktmvflqm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2mcrmvdeh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2biwffooz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xdhcizml.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2tooktgyy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lkuaqyhp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uzoivsyz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xizqqasy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mkchanpa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2soshtbsu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gfpniwvl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ahqmuwpe.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nmduwpzx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ncmsypon.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gxeqtjen.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzfmtguy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wfzcnrng.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sqquyypf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2koqysboy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xjnxxpoa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2uovxyzxc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rijsqphc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbceejyw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yszhafac.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mfnkroyo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2azfptxej.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2sheaxgrx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zywcxxej.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2gjsbxbbs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lpizxnhj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fjvydeqf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yedemwrr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rygxkskf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nztakdnb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yaafmqaf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2zzkbxzoy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gowwhhjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctopqpbm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rwmlaxqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzwtyhij.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2koxnbbos.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jthaxnns.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lumkuoip.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mgsbqupx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2jfkpdiiw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xiswgpcu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hpwvyuit.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2mndxhbac.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2yjwebsyo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ytnaaaug.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ghxdlpjp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wfkocqgl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dxbjvwhw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dutlohwn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ssaomjfb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bdcxqwqn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rncqakvy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ltcedzlb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2aozwiwzk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pelitsns.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xubavwnp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2fvjqcbch.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qckustsb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wlroqnxy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wfnopbmy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wltkcyrr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fqmxwavl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rxjusuff.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2yhbkabfm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jtrnrher.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xccfoulc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wqjqypxb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fefdakdz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dykxxflg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xujetbqt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vzqcpmgd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2erousptj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xufkvgvv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2exrorsxz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gbbjuubn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nflvmcyp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ppavpdiw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ruenfarn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jabmglqw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cufvugaj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nibgxzbx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2isbvodth.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cmikxekb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2weaosscq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rkengqph.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vvloqywj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gubkcnvb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uulplrre.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2scezhize.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2migeibzd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2busuejnq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wxoavzhb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sckdemty.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xffpjfca.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bfnphwnd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lnhgbkxz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ishyfumn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kxvkzluj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2cbthjomr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nwavrfya.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2yqyhgbue.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nhfcdsus.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qlxlrynf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2uxwzzbey.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2stolmzmx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2onnhqdlp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ryewqyyd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vrgiwtwo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uensijfy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2josseqyw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jpxngqzg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2eavzasvj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2gvavrggb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gilukpfq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kmbdxjlc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cwhirrxj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2llmkmnke.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2suwhaczp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vyywxipd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fdfscigu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dizbdxhf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vqsripoo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2laggkaqk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2tuyfztul.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vrwvemdl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vqbygavm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vlxcguzt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jiqggukn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2hczagnmt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2igifxxov.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cocjfqdj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwqvtyrf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gnduxzyv.html


<!-- 参考信息 -->