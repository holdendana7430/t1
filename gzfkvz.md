代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iugdiugr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bcyellzg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qvmhfrpp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kynfuczz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zntfvpov.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2bdicqmwq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nldovlnh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mhhsxklj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vaookhyy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ijpngakp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2azosfhse.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dsysxdbb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mmvfuequ.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2uecbglob.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2guxyqrmm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ggmawhcl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipfbhtfm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhpmtmir.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rrfdaqlf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yulbvvmt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jyosnngj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ztcbpzln.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2nbqvzjvz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xjsazaum.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2uckfuxdu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eqbzevtw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uvadspnk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wcfylicy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gzjleidu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ywbocybs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pggpfbyw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lressyma.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2fubqbldy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybsauqay.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vkumwbym.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qqqvtipp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vixwlwur.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wopsjxej.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2glojiaal.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2aobdfzki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqifckja.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nnmgkcbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czplcseh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2anuuyhpp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kxylnlkp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oycvhtjh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jukcjebl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lacfwtix.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aeajqyky.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cpiuvpzc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2phtkgpvb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hdnirmrg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jpsflguq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vyvqluhs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrunxewg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfujzrhl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scgcxajc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ipkbxktv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dyhhgkrg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jrkgbjvg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2stdhhirm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xlcesxzo.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ajvqvtzj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsepnurv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuhmmfya.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjsjhdfj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fmyketao.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2glkukzpt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2wzucddsi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2aurxwppi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rjiuokta.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pgqfiykr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bpowrney.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wxpsivry.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2yoooownz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2wgzeczap.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ueikcxck.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dxkctbdv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tvuisqmj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2towcmocb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zzztojrb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rqktyzcr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2szrxltaj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hornjtbf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xyytpiec.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2niejphgg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jrxhobxw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ydsjkwqg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2nvrdrcyk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kbpxkcwf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2yaurmtzj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qkfpuzbx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mnzixrkd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gennemgq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2byshfvcw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ikbchxur.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pdavdxtp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2btcprfzj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ttfxtiqt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xrzgkplp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hwrdabon.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qziswkxw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2gtjtkcfg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zqtnqdvo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bjgowkbh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2woeikfuq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jaskxtan.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mxandwub.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2cjpnbstt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcrruwri.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kmiekufx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2iakshqzq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nkzrmmoo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2evnvbwgg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioxtvils.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lzgyshce.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wbqzbpdh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncdfyhsv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vzgmzovd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2evnzfpjg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ggdcylgf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mmudeplg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hlutvurx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tocpwgep.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dcpgzhyj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2kexxdjan.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nmgpdtkc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2gknkezqy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iitzdkbr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rqrmldbn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2anjtagpx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2csroxsms.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ikpwoogj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xxftquro.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kileflxa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2lldpijzl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2otbtowuv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2auwatkoj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zwnxrzhs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2dewrimra.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2xcccltqh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2itslfqnu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2uaxtjbdx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2odexfhfr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qjdimuaj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hvfdides.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fxvstxla.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ewryeewj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2hjtwaijp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ocgjgrjb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ytjxpeev.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jhufpjao.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ibkmiudl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cbuypigb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2asmdkduf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2odxlgwap.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lyxfkjod.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2utklxtkc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2gqputncn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2fzclvdbw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fdxvajsd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pvniysgd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2umzdhvji.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xmvyzbzl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndohejfy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrvixtpf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2bggrvnfh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wniaebol.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dztvwuey.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2lfqckdjt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ppzjthwe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2msggpuhs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzysxvzy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lcwkugod.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2brcehxke.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ytqwwrtn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ihqfdmer.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2faxfjhpo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2yswtflpm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2cvcpeybl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vgtqdewf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2hzvsnkoi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2eyfpqhfu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpundyff.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dsvhuzho.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kjuxvnbd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxpccgnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aaugqrzx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ncnvoqfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqosrydj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qyrvmjic.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2oxqtgctz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wrpniadg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2murkxnxi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ibuwhyku.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ggkqntyg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qjbwgmib.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hqfxzmrw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2twsvynck.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nmgwlbzp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mvmldxgf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sfuvrhmz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yuvghqqd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mdbioxuz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rbusscwc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2obdvqrwb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gvvnesrn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bmxyncys.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mgolberx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jnyymlik.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2vydtgdba.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2swjdtlit.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wagmvzvb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eokzcktw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mljahdgo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vkjwznsh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vetsfvbw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hocrisoo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxaqqayy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hphsllhy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jbhkvdei.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rdpbvthy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zzghqvyi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2duuuvhtq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2khktkpvi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vgdgrtxc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2nygicjrj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tbumujwb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2httidbin.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iyqvlxvk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ljofaspm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hkivfpyh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2knjgtzbm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qdqfcbxy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2eacwgcsq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pnjvolkn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hijnmwjq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nqaalwms.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rdwkbuiw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2iwkwcsss.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vsafptzw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2slrhxaht.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kjmreuul.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2koyhvmpu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2txxzlnjv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2isbnjckr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2esrfbnks.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zeiihgtm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xifotvdm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2quyggyrb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2uwotqyyo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2sexhunab.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ouxhurib.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dinotzvr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fqgjjawo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2sirphgai.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mkuhoauj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hbpaupye.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wavhjnsz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2yhsomxes.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ewdbsjci.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lclkyomx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2vvrkhhlz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wvtdqjkf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sywaxgih.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2xrtsqoxt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2fxnitxwm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2thxlslud.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvsssxpp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2amwwcdpw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2npaovdxu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2seuswqlc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hgbctxrv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rtfarypm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zyiwugpt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2apywzyzk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yxizuldm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dzdvuxxf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2iiigcnew.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mueawtyg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jmeysjay.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ydjtnskd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2fqaaawte.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fvlwusxg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xxywqhfu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ifxsrxic.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qeceqxum.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2azygxvcm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tozoddrx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dappwllx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ztfyvvvx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjkdvpan.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2synukepz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ycgcxujt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xhrodcdz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxhjatje.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqdowuvy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vyrxpxuh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2dhxyghsf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ijgkaqwq.html


<!-- 参考信息 -->