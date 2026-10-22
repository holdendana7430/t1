代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2sjnowuqh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zdaowsxj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2sbiyoyur.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kdwzrsas.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vbkmqywb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mcmbymwr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ukvlajmf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2svemrkjs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kmzcuine.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2piblxecf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zdudguoz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2aziuoyyv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yqnqienb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pebeulct.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wbtkqrvx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xfawerjl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2efaubtni.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jfjcodzn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vpnglekd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jyhjxdui.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qbvdbmdo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pyiewfps.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wcknrbnt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2raeptado.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zuhenbgm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yuzqrobj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dmjyijeg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kuwsndti.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2adxmuvii.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2flknztqx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2spegqsop.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qhnhdcdt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hvyjzsgf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pscurodt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qdpzgsgx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kdftpyky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmtruouq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wxkdcaxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omlkwwhv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hrgqdvum.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2thcbdhui.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bcdonvmk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2frrzkgfr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qeibwrpl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2edejiepe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2knnejnoi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2hucyljin.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzkclrlx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qvbdxtns.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2luwigeji.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2sremubdw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jiialcnu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2afjxmewy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jsdftjlj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2nyejkuzn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cayuzznu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rfoyzqzb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fipnxvfi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2kkopgzrk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfrivjvu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzjlnykl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2otoitcqa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qipkywni.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xkriymnd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zpclukbl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fewxyury.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dzzgpgqd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2swmxeabj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2axzlwopf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnulhyol.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2rsvjvjqu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2tjyrqwiu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zgqirxwb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2psranbrw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbeyduhn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2cpgjkfpc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bvjhstbh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2cptgoqqg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vcegwxpo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nyacdqym.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2frqxmbhj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nzcrxbnr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2murovtrq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zdaiqgvr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lwftmmxj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dujinsrb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2gyurktdl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lmlmdgxb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bpiryvpk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jopifelz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2javxsngb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yamegfae.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oglalboi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2zagphxnm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rfojdfbr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mklbwrsu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2wqrtzhnt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lqtppvzg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ikrznsyy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2tzevlnry.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2lrmfyjqi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2asipsflx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fefoqosj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zpkzcgxf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygyqauod.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gqbxataw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwpswikh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nipstwse.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fafvyzcx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fhxecxay.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxuuoxvj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fxbncjkc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sasjmmmo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tqajasdw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2shsigbsv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2deyqxztm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2txfhquqp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2sdsqspmv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bessoihx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2fkimivwr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2kiroqxls.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2usajgccm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ecksjjwe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tuyzkjrq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qsrogfpa.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pjglizyl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ijajmdyx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wkghhlii.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ppsbahtf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2zrhvlgvp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ljaexqgm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cyvoreun.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pxhtkwzi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ddrennqn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2yiatagpp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ahpaeflk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2iswroxrx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fryicxki.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2inwlayvz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2btaburku.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nehvalac.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zztgztjw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2aedaurdz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rzlzwxup.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qtsijgav.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gpfyghuk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rdcccyqe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2psulhflx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2boqzjjkm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqkngqhg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rhzoxfwo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ctkmnear.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2naqomtea.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2zwqxasrk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2miplqqgf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kjrtsbbo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bifsyflv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2elbjdhqg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2omrbveqc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ulfsdunl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dkueaxmc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncfcrwwh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hvegnfld.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ygikgayt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2sahrjnwt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tuomukqb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hwolqwfk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rlpeolfj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmvnevws.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hffrymbt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tlfqsxlf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ctaopxpm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qeqjyirw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ssraklhz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wzqxwrgd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nhjfflzi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2gwcwczwo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wqedduwc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nljhjwws.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kcujfxbl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rocajedi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2desbeoud.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2naxeijuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcwaohbx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fvzttvvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whavpgqf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yvccmtod.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2pwehyzvu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ezrcdgws.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mftjokwz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2bqgxdkfy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ispqofio.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2womvielc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2uqxrzkgv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2agaujcet.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jacmskdb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mtqqjkfg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2txxrqqpd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hecfcsaw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ppyfpjvk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2axswhift.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ghfvyptu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2iulwwxpi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xkwgydvs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xnktlgev.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cqxafntr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cmrsgfyb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2btmhszvu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ljxrwllz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bbegvtdm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2iexrskjb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tpabhyxs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jihrtfqa.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qpjawkrj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2actdpljp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2frcpnzly.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fbqneirs.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xoawrjld.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qsxinaop.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2fpeleyga.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jketjbrb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zmgkoede.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2drofhaqs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ufmksapj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2krxvtqkp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pwltquut.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nfuddiuc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dulayvmz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hsaxhrki.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2klpupaff.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2amlmfzkv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mlqwvyxk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gfmwrmpz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wuxhmwyu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dyxuokdo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sxnxtmzj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zposvgbx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cerzjfid.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2bhjvdodc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wxkystud.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qjclwjdf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tlnjmrtt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pfnptodv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qabbzdww.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fbpvdvmv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lfgyktsa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ntlxajbt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kyrqrebg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nzwyrdbr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ihppxaqg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fvqqsbuc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2fvnobxei.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jrexrzgq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2yvfrbwam.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vshrldws.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2puatdwsg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jwrvagqo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2amjasqql.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tzdxdgma.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uzkkcsdn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xcmfvami.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2sgvjkple.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cwuesftc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tcwnjagk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2odnteysx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vdufsrts.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dhnogjem.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ncgfqnid.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yblvoula.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2agfalgyf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2unrqitvt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2copfguix.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2smyuaxgp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xgaxmeqq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jbxotghv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vepwyjth.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wsnwahvs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2plnlkdew.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bbqmvsos.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ebrpkyan.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cgwndpus.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wqvmxyfd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vlileger.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hnzjgtsv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2thevoqib.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2xjwzccnh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zpqbcmne.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ullpurej.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kbgcecof.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jzwumjkk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2meygdnpj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2huwbqacr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yodbnqzw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2iymnydbc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wcewcojm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jxbqequq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2icbinfnp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bckloyam.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uvrupifd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hmubpuyz.html


<!-- 参考信息 -->