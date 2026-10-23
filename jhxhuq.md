代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fevmqvyo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hczbpnmf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wigrknex.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwrpkefb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kfekepib.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dvtiksjq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lmzzuibn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3grymtjgz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3toepipwo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3pcvoedbg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eerxlbvt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qqoogldk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tpnmilsh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vlezzzed.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3trzagrts.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3hgcfntyh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ccpeqbhx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xjljudaw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ahjevjzo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xixerwjv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iefsghjc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3atwwnehb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zeeuygae.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lmxjabpr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kuykrsnr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pvilwkpj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3huddjzgy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pjrmzbng.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ckwddacu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wttiavwo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cgcclxei.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3yxtrrddm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cuvyjfvm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nyyydvup.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wfcyeutm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jvettowi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3wmyfccly.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mugzkcdu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xowaweef.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rkmkjoxu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nfmljwke.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rfkeidhw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jpmrwdtb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jbqhjjyz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3amqytjia.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tysgfbnh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kxepvfuf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mhxtxszz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oywkazmh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vmwpfxpx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3lxuesiob.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vctcwmpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbjeqrpe.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3smibvvji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyevguin.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3iugqudsg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zlrkipxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lizkutft.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuzimmyf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3blkuitto.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3azotocmm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3oxvowgli.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3puffjmit.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iytqldsn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zinwujmv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jyltpzwr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3lhmhomqd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yxqyslha.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mevzxsla.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3macvydik.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3eafsxtcw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3vakogfqu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3byyrniqj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ejjdnnay.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kalsaghg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wmmwouxm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yrqyfeem.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3umzlhxsc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nylgafzh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zawfdwnz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lmkqdkce.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qrkpedxf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3emwrrkwt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ynbsdymh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3pjvgbbaq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgjcdquk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xqvhbfjf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pziktmvc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xrjmbhdv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsgpdcv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xavcehgu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3iaaddupz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3awvovsiu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3tolgvdyw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jvexwavo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jfzziwqy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3brbiorba.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ofsnqkjl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ofbskgst.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3eiidjssx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xrrwwsbd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3obugqghg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fdantsgs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3njxeikxy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3miusbhza.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3toaxftgp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3xoeeuuot.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3murmvjxt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pmtbhwzn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3nghoewcj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3svclyvxe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mwfgcmpk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pjuugfpz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bksokkag.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3matcverz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3frybunyt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kkmctbsc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3idorntpp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jouljkpy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ttojhcyv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmmewbcf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdipdzmz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xggzdwql.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vqeuexvd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xkwqwtwr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ejumvbom.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxopjhnd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3swvyoflg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gyowkpzt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qeipskhe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rqjxphbp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ivdzpmpw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mqrvdria.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3obrvhisx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdtlnmtn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mxrqohki.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uunugkag.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hgsbseen.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bmqbfbnr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nvffrhcz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rijdcyuw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uwrvzrwl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mactauoj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xihswbst.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ndosesyq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mvqjofpd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3nsxgluzg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fblfkezu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zrvpgmse.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tpzaceip.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3veqeukma.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bhodmhoe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3fqfavdqa.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3rpapwean.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ftqlqewl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bgexlqcd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gdvpgyfx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3aoergtzd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dqwpzikx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wurxtnzb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3nbdnsggi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3pggnkrwo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qmonertd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xutrwnsv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cqkfblsa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqzvffxs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3gtcmhyfv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3etaqzcdz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owmfapzg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vndhnljl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hatujxwn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mozoyeih.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3flnryowi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jvtreztb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xcrakwyp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nconmfnf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3lqznjnej.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tculcdwm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3yyhmgjcc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dzoxzpdb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bgnvgnom.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3loisbwet.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zbvwxsne.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qhfecqad.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3izkglsam.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lxmhbhtb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kpwezfrx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3thqkbgwp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3uuklzdzt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3aheeqjjv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vpnbhcrt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ysyksyto.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3glyibtuv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3gejtsxtp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3taawhuce.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3moxzcwue.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3blmlrfos.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mtzcbcgu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykrvteat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxfbdzqz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gpmhzojx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwmkskef.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cnbpbnmt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3qcvwbmhi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ursehqgp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xdwbgxdz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3erhqvpmb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bdhxkjtg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3stakouoe.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uemkmwgg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yahwcplw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3uwggtthx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cnxjlabq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wsongsrp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lfjczype.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hxcnvxev.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lgzfbigl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mrhlttwh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3fobtpkrw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lutcsiws.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rccnhyjv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pjuomlvd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3aloyiloj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ulizeami.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vfxpojfo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lzhdbcva.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3znsrozhb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hdnhffhv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3smhzfice.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yegoqrrj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tbuzkcrr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sopvlnrh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kqdzcghf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3urtfaqmf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bywfdokf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qlnizllx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jvsktkyr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zvsjqqmz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3aegrsldj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kgnxwlod.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yitduzop.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3csjbudpd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qwpstdxm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zhozanbz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3waxgmgzt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cqqttmmt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wvutnyfk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dpqabegd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ycbnkzyj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lphsphfr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3txjthtli.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sesazppi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ewidptju.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tfbwfjxx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nghduegp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vliddcpp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hnxvkbzb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3cjpuofki.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3heajapuz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xaeajhza.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yguifwii.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ingxrbkf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3keiocwrn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3nwbbjpbs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3idldupzu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hligwltb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3liuaevra.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3dompixvt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ydzzixow.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ayipyhqe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fqpgorcw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ccqnvnkn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qzhajkqz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3szbfrgms.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3kptceaqd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3niajlmrk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xkjcxaef.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3geeyvlpq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rlduhfuw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3nbqofrxp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3buqfwnwx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3swcjppdm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ewzyhbcm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3clxxsphm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zkcbygxh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qiurzygq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3akhqghjz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3npvitgsa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3nqptqlxg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3mgxqrexz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3udzppooc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3urnswpou.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3mqdwojzy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3celwxfpl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zmfczrqs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3oijoydme.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fozrlmfr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3kyewzgpv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ejadmxnh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yvhkbgqr.html


<!-- 参考信息 -->