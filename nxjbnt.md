代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2topkaakm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mkvjtplf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kxlflaca.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rcvfvigz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dqjqaehg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zkquevhx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vzyjsjnh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rpgexbfs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2offthvkz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2eokvchhc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dwbaysqf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gsgkarrk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2efcpogbx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ppjxiool.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2xythigdz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rdjqszfp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gakwqjuy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2hckziieg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pjlwczgt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2coxkknjf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffribvvi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2hnaecdjq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ihahhkvb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2aizfbyqi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kaeyoalj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ggudmdtk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2behhpvjd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hdmwayio.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftfqnecj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ogrrgrnp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgtuqjx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojsuwzgb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbxktfnl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gddgakty.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vcrujnsh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2biujfeno.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ebwrksji.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jyksczvp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zorbjzjd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xfofivff.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fzqdzqwo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ernsmwjw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ivrwqsjz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2itjaqaxp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2gsmokdxj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hqutwmin.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dylyevop.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hkfuildy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tchyojbq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dnfgqfup.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kskjuryj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gaoxhwri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kltaqxvc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2waxfvfga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lczjshad.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2osstnbya.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iokteejq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeossoad.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oadobhrj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hyhatgtf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2atpnxtay.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ejchoghc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xonbdngq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqctziwc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fptnlgnc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lihsmqqf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rmcplqcs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sxygkdou.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnxyxvtu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2nqgmjkwv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ohnztvef.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2apwkydbs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ohbupexo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2kzvkvett.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wevmgrhc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2idfourbs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfrdtpnc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nactsecr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2okoixksm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qfcexcfa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2sbaqgnyv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2euxkhpug.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wewaqdyi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2hivwbheu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vjwmywcm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuqfvgql.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zkixbddn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xsdmtbhx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ksyambba.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cicvfeyh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mmrygrve.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wnrqnfyj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hoesazsj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mdmcomin.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hfleuone.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2oifrepku.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rmnqbglx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2laoaidsm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lkznadrd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ljqbcbtv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2icoljozr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2aphiehfh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2gmapjnqf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kujssksi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jothiygi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gwrzgreg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ablapwlr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rfrduxui.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lnhspcai.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2trimnovt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2celfwunc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fmjijrod.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ozncyerv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wbfughqt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2karoevmm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2cyxotomi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2upitegan.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dnqiqtdy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kkhsekqx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2fvrgleuz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yizjdaaw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2apzretka.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdhkwuja.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lvqjgmdz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pndzbgbs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hwmzcwzi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2edoyqtdl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2nqjaxerf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2askjxoxp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fixlxdpc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2iaqnklvj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pscjlytm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2krmiuhey.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dpbqfprs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zqsphsjo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ygnbrblf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zdetvckd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2eebseoov.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2cbknamsq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2myjnimrt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nnuchtrj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lwuvpzmy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uyxhhkjp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2btioupdf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nnipfdpx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nuzglcry.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xwidfreq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lndtyptv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lazocsql.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ylftklmc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2sykyyjzr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zihrsuit.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ypmaiudr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2uhgungzu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ddxpsfhk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ybonodyi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2kqseutaq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ppanutnr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2owblvwsg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2myiloknm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qrxmuzrg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2sjkehexp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovonzcwz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2crceclmp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vxeeveqq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mwviikwe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dvrjktfo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pwntiphn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpmnbpps.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ymgrqjxa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rbrmdsgw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2layoknxr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfzrhppn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qjcsvdai.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rqcibcoh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rcbrkzbl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eextzmnx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hfasfluy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2evofaoaf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2izbjuwtc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2aizpfeor.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cootywnl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2tpvvriod.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ossrblub.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wjevbpbz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2azchqicq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gdsnvldc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ayulbmap.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jbyinmtx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zbzbznzx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ixcghptk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ptctctzk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zihpvlbf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2cxonycyq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wlypduhu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwvaubat.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dhivaddq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jqblwyoo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ggugoyxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpcsuvmo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2galpugih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjmscrzy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ortwszow.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lnwksxqb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cvuwdltx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kvcgicvf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2eheisazw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ahyccnmk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jwsscnop.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2sobkotfz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lzggdetg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ueobthrv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lpdshekr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2cdrgwamm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hdwbizil.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fkzsukcz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2yxnpdesg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tgsqtecm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ebazmyuy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hsfbsrbx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pqcmzwpu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zlugjxct.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ilqgngiv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mecltxkr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sfttrywt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xkejygvz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mvkynapy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ehmclgrd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nkcuahmn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2adcfjyiz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2oyyefvcl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2teewfdwe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pjomugvj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2znbnroes.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mxjujbxl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2luudoyiv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yhmaodnk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mepxmnrn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2djbchsbh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nidmayos.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2flkoqtlo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pacobzlp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xchxqrpr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2egjozqmq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sizjzaut.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gqgzvmix.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uryloswd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eksnmbfc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahqlfvvz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rxpimmys.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jxeufdqc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jbuxrdtc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zkldbipb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yrxmbgos.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rwdnzcip.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zorwizht.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2rddplpit.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tpodcszd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vwxpgymz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yqaabiub.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kuhyzdca.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sjmypzzo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2weeshyfq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rflqowyb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hbrodzlx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ddpjsmet.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fhbwtpvw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2uvtxyogm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2iemprgak.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wujbdlrf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2pqyxaxpd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vbjssbmi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwhykmce.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ayjjnunm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kqlepzxj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ctqcdwci.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ostekoai.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cxqifxrb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2raqppres.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qgsvbfah.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iielznvm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rgpzjvax.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ujcnpyht.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2egnyituv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wclsbwul.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pqvkgeaj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dlfckudb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xrnlapuk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qzuywcbe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2matonama.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2esmxjfyy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ayedsmfc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nwedapvy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lfklowww.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvtheyda.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nvrndxhq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tcejwaxs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xkxlukgf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2znrccltx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2otzgfehi.html


<!-- 参考信息 -->