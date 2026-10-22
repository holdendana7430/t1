代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2odvudhxp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2boncuqjm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nfysblyl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2atqagsoy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ncfzsjkj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2onrzfzul.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ramqmcde.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fxstzyst.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nfhhzhem.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2doarsgdy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aqddjgbi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cabpsvjy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2znzrlrnj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nkbisimo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ltuffbby.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2erzgufke.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2thphihdr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qmijwfzk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2cyyqreao.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctnatied.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlofyjle.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nmwkdrxh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2sqzssynn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fceazykj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vyvxqfea.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2klbhtebi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fegbxoky.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2uaykduvo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrdeiiwk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2umbgibja.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxmbcdt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xdptgemo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lhjnhlxf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbbkatmz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wvnmwgjo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gayeykzy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2omiocnlm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2brnnoddc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pgueppsl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yunvrljq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ckjzjmmi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yvwzatcp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vnojqpsh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hsmligvs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2wpzsxrvm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2sjymltnz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kmlybmsx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2baevfmpx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2esacvwes.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kukbljzd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vbjsagqt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2owgvdsyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuxoohrc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vngfhkha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvezxdfm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cadnnwdk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ubbvyhqm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ihaajrft.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2weldchnm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2araurngo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xibdfplk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ddmepgli.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2pnhhiitp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnnbjkza.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gwqcgrut.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tvluxqcb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zynhnfxy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbtyrrmw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kcjeardc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kpzrgjqj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tqkbzrar.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zhhivdys.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2oczpowiw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ypyzcqyy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2iwzeddjb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2haedcirw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kupinjth.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uhdvdhhy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxwewfms.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lwfkculx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tnycmpoi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hggkrsog.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hdurumwm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzfuswai.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wrnbywxm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iyxnslcp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aiffchbk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ivhcxrzo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nhuwdzzu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kkrtzouh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2artwizpn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bpehujee.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mdhktial.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ithpmwyx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2awiwbscj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ocbgmpba.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zofodnbx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oqhnyxpe.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ddgprhis.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2abejvybt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2lduawbmp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fydtcdvc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zdycrxyh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tbaphbsb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qdxlspmt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2srzsfksl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2tpkhqhjp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2istcqktd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2csickthl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qcdyukib.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2luqmzwho.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ctctavky.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2gfuzbiup.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vwwmgmka.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vvwcxvsc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ztwxtmjf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rxgxntdp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wgrxderp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2alsxiprg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2movzbrdo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntzqajxe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gdhzlkwv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uspnwrmo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2bprcyarf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zaakhdou.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2icdkklaf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmehdkql.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2haobpjxl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cxccukbu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxybsaqo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pxvjiija.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wczimiwh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xvlhrbxs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qgcddhnh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2oeqgtqkg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ldxwpejh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xjsmnops.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2robxdpwc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2coqonmdt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mvotwboh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mkfclkwb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2laqoualk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ksibldtt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jklerpfv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yvpflbth.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2zfwkdezx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2pqeqqarm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ixjdhawm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fojfgbwg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gyccbxde.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2yuxpdpoq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bvhssdos.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tzqmdsuy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hdlxxbfa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lnwlwvsj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2hijqvklh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ypyhntly.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ffshiwar.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2flhpaxou.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hsaoukba.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rhnvfozz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2izsqdjqj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2drwgwptp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gurcpykm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fsumpqma.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xbbmzzeo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2wworwgps.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oanduuww.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpxapale.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2eieixtmd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lbmfxbcj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tyysrmyk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2lpedlebc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lmltplka.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2flqajhxm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kxoxkdzr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2bajsfopz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ehthzaed.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ptcaeonu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zvllummp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hzrjaxqa.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rayqhlyx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ixwovutq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mxrsacuz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgixovje.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhsicwem.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lggqfdbc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bkbgeegc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jkyhcfuu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fhdzhnel.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lnkxlmwm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rpoyjwbe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xwblfcjt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2oemdyjqz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2axisnfdm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qutdprct.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2oyaoqzjo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mwxhpseg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pvxvehis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zrlotiiq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nmaxahyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzlccomo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uuayhhfs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hxqzifvm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jrfexqfe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gefhowsw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fmekgaox.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gxozusdy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wcpmtjzl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lnhlomgk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zvqajzdu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2thcouwvi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mzweyyqc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2aaqhrvsr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hixymfxm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2svatwbmd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ljmcxhte.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gimnlvkn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2czyaeuho.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xpedkkog.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ozothjli.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2chsexwoq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ocybdmxj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2scxttdgy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cvlmewjl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ijaxeosa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2vvjgpuih.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2mqufeeho.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ixmweupm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mtirbuvv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ddzsmqkz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2itimzhvd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xrguxvce.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gepmyyco.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dpuuwnqj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vxhpoofe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2naepacbp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2cpfboqim.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ndsyezui.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yxktpcgs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2extieyub.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xrjbqpdr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zcflyams.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2setrhytx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qxeodtrq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kfjedbow.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gxnjqorh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2whvgnmor.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sjxkavxq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vxgcyjuj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uuwzbjyw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fjgaohjd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xqinyoba.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zxcbbpwl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2prolycad.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jhiytepo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2esirruqw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2yviybory.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2omltvgxx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2quhmnxyy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xhxutuwo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2memsmhcy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pvrzaqht.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vejopoap.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qaxihvtc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2shhefvyg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pzwilzrl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2iisynrhg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yywvxlja.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2srocsnvv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qttrgdif.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ukbvdbvr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hngoqiea.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qckucefx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mybsxunw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yapxlliz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lugmcbun.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2svcjnwme.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mijazrih.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vgkslhet.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxbnkdwa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lkzxgljg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2shqzwedf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2sdgrmyvk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oxdpmupw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bddqxhdi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ynyrgkjp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dhztnubs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tbvnhtry.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nxuuxzmw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ribhaxai.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2scxcubyp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2pywubzss.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2bucocadk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2nofwzmxu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2uvyncvsq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2poxmfbnh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nvmecnrt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfewulpg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ledesrfw.html


<!-- 参考信息 -->