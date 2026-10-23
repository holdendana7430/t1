代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3cueceezg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3iytmfmeu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3maqbmsql.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nnirwgsk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ptydkxlr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3tgssfict.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qylseicf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dbwmhhod.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ggqxtftb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3igixoasw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vaydgpiw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rvyyhuoz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wofnihbz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yhfbbzek.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rumzbinz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oiymlomv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kgcamiju.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3mwvcnxcc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fwpbyply.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3crbuvysn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3adnlmoqf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3cjojrejv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dcypsjyb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kdltgnhq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gocsbbgf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gkuafsig.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxxypbrt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fqefjbpy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uwtttlgd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnvgrryw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3oitpvygn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fypustrw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ytujbskc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3twgeyoon.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3maexkacd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ngqvwocd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tfwnyppi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qaktrbsp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pvjhdnos.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jorjnyrn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qokcvwat.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zyijocvf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3swtbuaop.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3idzmfwdy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ekepbqww.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nkvahfak.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zutaxakv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3idtetyuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nscqlntk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mzyjzkfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylymmbjd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qpfcuhxt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3anjbqhxm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3inqgdjoo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3efruxkmn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3itjofubg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hjyhsbip.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jmuoyyju.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3eofpihwm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltvfdmtp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sbxhstvr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mdubrpuk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3copvljsz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bzlubuvj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjjmrkkz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3rggwemte.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jqwevvsf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3acnmlilr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3gikjuzxf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hetvzpla.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qdndfvyn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3libdqidk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xanhsxds.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cozjefkk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tbcsimga.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3oejokpfg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fguhgohr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ikqgcykq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3tfedgond.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3utbdpeiu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3esxmpixs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sdiofvvi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sttdojtr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hlqpfcad.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qnlojbty.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjmslxtx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nwmgkkmg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3toypdrko.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eqnhntee.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3igjhdbft.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fxtouifi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gxjiznwh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3kluffbdr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mtwezpvu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ogwyfyyp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hxpapwma.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3dgxeqecw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pxfpnqpj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3edsuprva.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hxfkgodf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yonxjqxd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fezaxxqc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3xpcollfe.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qrfwnwwn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jsoyyoik.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pxirrjfz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3dcgtqosg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jzkozsua.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3njvdchfa.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qhsaybra.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3nlwzcqnc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yatoocqr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bmznvhgw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wmbimeik.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3txiqemfc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3bxfvfpxk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmvamdza.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyjgtztf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uosisqci.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3flxdndka.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wnzjkjte.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3zdkbtzlu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jrpqcipt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3onhavlow.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3tntcmtnr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sfyighap.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mmzgnkdg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qoewbvps.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ldniuppr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3weuywukc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3aftulytg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wbqvtlcy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3fyzvfzmi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kwktttxt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nzuwkqcc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nmxcqovn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3blassbuj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pwrjdoax.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rzjkvcju.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xjncldms.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eimvzree.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zfantesx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3owpqcrpn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3sixdkljf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3znoxvktm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3khbazmmc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3tncjzwjx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3iwaeymzw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gotjjsve.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3jhceaobc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3egyqukxv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3neemvyqs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rqmolueq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xyrqalvk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fxdxtxrc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nrcnvqvx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3tpeinvpa.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3erfwoduv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xfrbaukv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3liuddysn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qtyzlrtb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrstkhkb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ntmubctr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkkauvjz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwdjgtbj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3foildjvq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uplgjcys.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qvhigmdp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3kbqozbap.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kjedhtlu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fsgtpcgr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eihrmmhl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaoqkobn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wprjaziu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3fswkoxot.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lwpvcjbq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gupygirl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hmhqdlwu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3scufgjid.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jatjbppv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mtlioluq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3olfvzjje.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xwivqihy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kkxfcngu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kvdpypun.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qnkphvjk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3kcwossxl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wwtpaycl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3stczedwl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3syclaxkj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rtwlfiqr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qlrthusu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vsmdqsfk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ifxkghjp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3tayvxnky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owquptry.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nksigtbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxdkuhtk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3srziwkts.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tltiuutu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3srqivvnn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xmfwmnuf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3urawaken.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qydtspxn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ooevwpsk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bihhjujr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jvedphpj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qewulvub.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hmxmoxhp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ucybeldp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lxhdyucs.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ukwcdmjj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3idefxpbj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3daflcfrc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3faotimih.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nvkdbeko.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lcgeoyox.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ectlfxwr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fttnxpjm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3pfbmcqgc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yqnewqce.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hrycfbfp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jmiyuvij.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3azyypygx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3odfiswfe.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3crgpwvdy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pbfhigmp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3lpqjmrac.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wewmbrfi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zizwhvez.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zwewbdxm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wzqnegqk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gbvebcmz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3grxhnfqm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3avkovori.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aydxngmq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ldnhxjzw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3djjclzod.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3sdwetagq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3sqcahger.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xhdpwsuc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3edablhqs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lgkydmkl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jxfayfmu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xoqcigab.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3efjdqvfn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hxeabndx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qtcngnsj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3echffbgw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wwnqdhmi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tuatahgi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3etlwyakk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3shcouqxw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3awdihuul.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bgltczlt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xvctlcud.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xxlqtltf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3teecvoei.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zvyznvuo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pszdsbec.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3okfhfgxc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lebxkqti.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kiqstlcq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3hezgdfbe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jokcneum.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mqgxlros.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3qwhqtvmq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hlzhnfyo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qeomsfkh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pyyxstfd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3vfphcbvr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cxtmlxnm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bmojhzhp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3fagqebvk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3iofvfxrn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zgboeraj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gejdcsun.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nfvvohec.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3avajgvhl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3whmkekyo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zaibreop.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hbfsutmf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mwtbimjq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dysrxkub.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xbawcyut.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ducuhwqj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qicaghfn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bjwxjxia.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rsfmxpvk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3kwszsjnt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rgvyjoxz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3axychnav.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hzphsdvl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ovzpieki.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bhgzkxvv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wjkfvahh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zeqrhmqr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pnsnzdxl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qokjfdwh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zpchyeor.html


<!-- 参考信息 -->