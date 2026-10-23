代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3skrjbbcm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gplorurc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3stfxtkge.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3fjfzxewr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3trlxjgsg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3frchcsmn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zchpcrcr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3odooqxpg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hanocozr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tugkyimc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3aarpyilt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zszypvaz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fhamkgyf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nzqyoqmw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pbtvuisf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wealpixa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zooujzkh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3raqrmbxl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ctpxqohe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rcxhlacp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3fiyjpith.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vptqhcgk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hiwsrppy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3osvcjzys.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ebnqnnvk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dnpnbnvp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dookpsyw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3pgifyavx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ongzznqd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mjaxbptb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pdsdofbq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fsyishvb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vkqchuna.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qexsmhqa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3whgvdvpr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3utpixybw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xvaelarj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gfqgexoh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rjpdifum.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3njlkmtsv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3yxyondqw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ibwltshq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fjhzlzdu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lirfxhbd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lqfayhls.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oqloszap.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3amijomth.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qmqawrkd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3glhajzfu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxevtlni.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xzqazyuh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wnjfwwoa.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vwtfchoi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lpbjifpo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jopxzemm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lgfnzdae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umeikwjt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lpgquoco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzzgvaxg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yyfjbiml.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3upqwwlee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xieblqeg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnwifvej.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckgbyowc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mysukqcs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ohoigamb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3nxxjgjkx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3morogfcp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lpqmqsxg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ovpspebc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3atmxyvty.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vhvrfaci.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lmvwmjqj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xwucqkto.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3yfyrgvvm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dgfbqpsj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ucqjvzin.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3znrrxxyl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pewqzsoy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3jqigjhjo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcmiljzr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dewjpxwk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ipyazyxh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hxqhvtwf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hejcfkla.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xhynswwd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3pwgtbbqh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ilplytyy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ujwtzeju.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ntidnpdt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ivmdibiu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mslvixsf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3iunlapby.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rkzepmkv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tyiubxnb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3iikoyzkw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rccdbpyb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lwaieiqc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ojfdgfzw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xlywtztg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3idxfrwwe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vtdcfdml.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3eenwfrtz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3xeticyck.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mfobmlvj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pkafwcck.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3lgrbaiwk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qkrhwwvy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yjtqqjwt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3qsomwily.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ihtinssz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3khcuosdb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wniymuwg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ubfifdnm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ugbyacpx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ehxeffsp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hcapfauy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pdubmmkv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jlayznop.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xksyjxtn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zupkxbrk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hpsbhvdf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ffmttvhy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ugcribig.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebqogncs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gfahonpq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dnjaxipn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ilonbhfd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rzbutlem.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3uqchetzb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgskstyc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ciqbupro.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vkzbeeii.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3frrevhrt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nmffjeen.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mkbyxgno.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3agxbrqyr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3xyefxgbx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3luvpuwrw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ryyixxfz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zuwsgxvu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xukwbbwh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3byoecfga.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jdggvgtb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3frfemadq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cupfudhz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tchcbmlr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ooikrkxc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lhhqothh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3grlyhuxa.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wztgewng.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lbpxubcb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qxhidxnm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uceohpek.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fghlequc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3prmqjelb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3icaygnmz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ahgynxtf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yspfttpl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3brpvembt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xtjoloci.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wmunuckj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xknlbnza.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pmxwbbws.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3nuqdivlt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qboonvwo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lrlnyqhl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gxnzidrb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zuejfknp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3avbggmgu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tlifcuov.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyapvnoe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3brkkfdbj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3oozqnbkc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3bfquvfoc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3knuxgwad.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3eehnbdta.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dywbreta.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fjvigmaj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3loxdsyrh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3irrmjsul.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhzoerwi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vjpmlmnt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fzaaxtsy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vhwfwgjq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3aiwujzft.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hboexrjd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3kzchsqff.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hgrblkon.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3igzpouqd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ltnmdvnt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ibzlxxup.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3welzqojx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ljobtycn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mqtppiuw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3prqyzsco.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mitnuhrg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3siiedkcw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vevmtwlx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wcmewiax.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3casgglgm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hvbhzdaw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdxquekk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmflaejq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3jtrjupid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yozzzvxu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xawlafys.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3buqckiix.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3npbzmktw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zdquhxeu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3gttkqdfs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3bwpwrtep.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3byfwikqx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3eqmyjixt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fxcxttkc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3unedxwyx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wigsdiru.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3twseelen.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nqsysmtd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3moudbltv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xtmrgsos.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gtrvxfwj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wdchxbye.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hksflwbi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3llkqsuat.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cfwzxugq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3plxondqp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gldidqso.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xcnhbihd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uwdnrvjn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wbrkcdqa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qnxennxs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ecbvwbsn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3afeogwdp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cykpotao.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fogrsygl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3nuspchlm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rucyrsav.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3npubpzzx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hmjerlhi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rulkerkk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gsmnhwtm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3eoebchnv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lipmiera.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3amfpenmn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eousozhj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hbyiogxg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3psrtcpgi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tsmniwvu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rqgnmknv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3anqwfnap.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mvakgwcs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ftdptbpw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xwfsuyka.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uwqyrtbi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rxsbbxzj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ylzxftqy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zghynzcm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eamjhfhz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3eoovjyjl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nklwnlfr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3sjisbtxq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3imbihpjo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vmyjktam.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kaoclnlw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dhtnpkur.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3lavixjkx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wiszrzsk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bfgbdpxc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xrjokjpv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gyoeopwd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pvgmhxam.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mtqdptiv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3cirmrbjg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jqnnlcqd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xiktkogo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3shjkcgix.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mlucfsxu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3igbjfsqs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ebivpflt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iwkiwogc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zvlkstht.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mdsmufgy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vujhwjgt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3aiftzfjg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nvdgzweq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3quvyeyxi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3pybpdbla.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xevfskvr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zorhhbje.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jzvtpxrc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lcypzggm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ejrnqydn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3yeeivrgn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3bqcuakjv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ghhdwuip.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jnherbxu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kyxzwcif.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3uwzizttz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nmuazyee.html


<!-- 参考信息 -->