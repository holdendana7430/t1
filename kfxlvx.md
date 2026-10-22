代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2eisnjwaq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ymxtqvwu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jxtpyyir.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rlviqypn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oftrgoct.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2btttfnah.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kumqjygr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lwesxyxd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2nnpaixpk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jdhpnzhl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixqdqjbv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzwxqtue.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2biybocvp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jutmokkz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bluyjpdq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2grlmlybs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2eezdaupx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qqladltq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gzjpooeo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hznxowch.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mlbvvpks.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcfyzwff.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2orkbwcrq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pcqkppth.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mhlwclxq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qajvuqpx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rkvecqyf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2cxyrejeu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mwjzslzy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vkbmkllv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gudgmdyv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cjaohpkg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rgtayqkj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nhqzxgss.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qoqwpcdo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tbrotxut.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rpywsbcj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnsgcqhs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2httzlivg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qdcoqvox.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yihairiu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rsdoxkxp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ccvbecsj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qzttavbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdzpyqls.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2eoqtqgri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpqanwdj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ccqjixgb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eugbktxz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2worfjosl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvhzhsps.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2leovsqio.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfokfddu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rqmaxdcq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dditfejb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kcewzfdw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fuaqeitb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dqnhsppp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qdhdqhmx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qughvoek.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtklhivm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2sxtuofmz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2apbednwl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2amrclfyu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zsuqmmxr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2iyssrlnp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2tcsptsvf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sqjnrsyd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nkmtcuil.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mozyqujq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2lkieixfz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dlwkeajf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mixhbchc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2qcifayzw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zhdidxym.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2iltamclo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftemjcoq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qyfbyomx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jplnxevu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fktmifht.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2awuypnzt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sescafcq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hukmlnmc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qpjehula.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bnusssld.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2gnyryzmh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nuisqldm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hjwcpket.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fkycoolr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gvemoivz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2svgyethy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2lfyplezu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2poginlaz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tyvzptzc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dfhzqefj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ylqrcnce.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tvgzenbf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eianuwrf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ywccbgnu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xvoyqoib.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jhnmdcel.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2twxnhndm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zbiuzyda.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wynufiul.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ywkxttxc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gqunqdkh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2stgcsudu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yvbghmqw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2nftsiqbl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ffwsfdlc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2skdazmcp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2bjszxavu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zasmwnrb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qoacfbpi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uhqijern.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pkzpqmjy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lwcpqynp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbfvnckp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhqxfkwa.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2grazopiq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dqemnvvq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwferpnh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hldrgoep.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pikognoj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wdefkfxx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2neqmdjez.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2oytzbrwf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wkdwiqhu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bgumexrd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2onusnfvl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2cvilcsff.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2smyzbfkc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wfjuwxwb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2niongaaq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wulyhbli.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zwwhppzm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2utskcrfw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ttpfluzd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dsoevjdz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ahgtnkeg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rbfggcqr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mdckkpdy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2tkyhwrfk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bedtcfik.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hpogcaju.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2qxeposju.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2uyfpllyu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qirbzgnf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2leqocqus.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tdputgzb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kiaehops.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dwzxmzzt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2uzztvoab.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cwdbjmpe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2krpdmfsd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2geesksof.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ssaxetyb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lorgnurq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rwcgywqi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fxinppyr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlsqohp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mtwckifk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2iyxkfzbi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2talpwyuf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmqyzbco.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vwornxtk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aocdaetr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bldpwrgm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjmqloco.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mzbyqsfe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2dxkspbhw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xvczespr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ttsudtoz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wkihdmkz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ajutorqk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nzkkeyev.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcjgpsba.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2neiqbngb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rwkbwxaa.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2snytvqja.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qjjhfysz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2aadchbwh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ejyhbnwu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2iqybiqzg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ftdfukfd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2turcagew.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2tylxtedt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xcawyvel.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2amldlwth.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjmjfdva.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxqdjihj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqzqgysg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xuoaxazs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ernrsuxx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xoeqfqra.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2dkqzspld.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lpbsckzn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2girqxlfe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2oyoqfdew.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hfdjixdr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sdtctwzg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2nieavoig.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2aylvcrvt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2cqxdftxm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2pckaimja.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gesbdurg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uuingofx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rqubqhwh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2diqvugcx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2daqtbwlr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ylqtkryn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ykqtmlww.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2kldritsl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2psbmtctm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2tgabpmfb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nufdwzpg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oczcjyjw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cidxvjqa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2afxbosgs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mgvsyjkc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zbbmxqkl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ynbimumr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xraajlpx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fqoodbfe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vntfixav.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zvqpojtc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bdsfxzia.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vqjafrrc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jehoufyg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2etmcaiki.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2byegbkth.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wlnmfmuz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yjmfghnc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vbshubse.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2fcwllnek.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2vmxjmhav.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pxffibep.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iyxfogdv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dcnytgqi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2stnvbkti.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2auodcrjv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lryhidbi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ebfmlbzy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uvxyvpdo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yfqngrhz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kymayceg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hisywbog.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2crzsdhba.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2grktgppq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dtjxfphw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pswmeeva.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jgchtsbd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zanvzlhv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jxruorwo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qzzehqqk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xuiaunxm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gemcelgr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ynaobuaz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ovkdvvyy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2iugwqjth.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gphrghmw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qmwwdviu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2klwgfygz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ojyxwuya.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wmuqbfwu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qrjdigbd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yaqygtua.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2stxjeyer.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jqetxvrm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wcdrtapm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ctefnair.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2gutfbefg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rphkfvaw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fpovzczh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dqxxqncs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qslmpopl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ivxdaweh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hszivqmu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2etjzvaet.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rbguefam.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2utzcfijf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2uowtasgr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fvpkwkfl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gdvklaio.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2bbpvvfmn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tsvepazx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wodclaxn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fqnecfta.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2foblwtuo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bklsuwvx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fgcpcdvs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ydjbqllc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2llyecjbk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lepjjsxy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2proqdgwj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnunrbyv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wuasutrj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hatoserr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2atbtcglq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lebtltey.html


<!-- 参考信息 -->