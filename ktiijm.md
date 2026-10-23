代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uvsmqnte.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kbcqztse.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xpcimezm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vkljzbtv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3imfqjarw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qzbnlogg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3uouswfqr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gbxupwev.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgjjdbxz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wiveumsl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3rpbzhsoc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxjynem.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dvyqffee.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gdkojfjz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3iuhrgiyp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gudrlcga.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ubxwjgko.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pzqbinhb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpesfszf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3igunxvex.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxwfwbi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpvcmcji.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rppnqnmu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ydxpcfqz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3yzamtyfy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3moagnlas.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3naymfods.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jubkioqq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3trmmqyqn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gcoamxqh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xxkgkxcs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wxpspnao.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kqpltjpx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vevuiunc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vtwnazoc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jraubaac.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ifjhskkp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3owqdoolz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3akokjkwc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jshgakum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfphoomk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3dhnpumqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcpmprwq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xtutvixr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kbcqzocj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3twmwjeol.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jgxlenhc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kuyrippm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwseavxb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kwmjsbnq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dzocrvca.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3skjstypd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3kvgxmyml.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ushtobkp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycpgaizr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xgwhlbrh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gfapcofo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3awhihvfi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hisourmc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ugywnoum.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bquxbgcz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3lnblbudk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vsegsjpb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvhnxmsy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3imabuefs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3moetrbzh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxbgfmua.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fydilxbt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gtsshokw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ikvfyczq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3kneqrdji.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3yqnifxbf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3clwvdzrz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3akdswgop.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3kzvssxsv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ccfyjapm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hxawpjvx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhftfhgm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tsnmzljy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3yqbcrhwn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tiipajuk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3wydjguqf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qjfjpjnz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rpaqxltk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3kcsarmfd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cmrysddv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nufiwhwa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zhznkhdn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3uqorxxan.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qdbebyew.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wrgjiweo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3akozmvhh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tmqcddei.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ehlsoodb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rlrawhyn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mziopcxb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3iwuszjmd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vnkwdjsb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lfgtzlum.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lfnymrwh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qbirkycp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xuqhqdrs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3tvsszwji.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3esiiebuc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3nnokeste.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3goysktfd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3wjvgaicm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tnfdvhde.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rttgorie.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmtkbemo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ucxgnpwa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3qupkzhoo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xbggrdgl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mytetuqv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zscehvjc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pcpjhzzr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ricwuhjc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hedrlxkk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cvkspswk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jlyxxzvf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lujzkifa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wedzouyh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ckrckdgn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ooavfjeu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bhwwwgvn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cimrblyv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vcgvsztj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uvblmuqk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qjcwkktw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sglrhcau.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gzpgttkg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lfkypitl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qextyaov.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ihrzzitc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xjbmtabu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3idqxymfl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fyexceqn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hrtqojwk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ncsliqwq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wygovceg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3hvcxqaht.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3iabaqxqg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3eotyfaan.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3odtsimxj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mmkonfkv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cayrppdn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3awpvoofl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3smwqbsqh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zklbpcra.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3geuuefkp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qhpgwicr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dvazvcab.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gcypbnue.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhxtmyhi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3liywzdbs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wperoobh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jbkewbyn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cfimidyi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3nolcotkt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3kqreszti.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bfmxrthg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rjspvpnu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mmduviev.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lnvdxojj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gqvpdgqj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3koxiyjrg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3pwpyzcac.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ogdcetab.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fqtvpgff.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3wdtnevaq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3lkxshvoh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3kemvqnir.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uhrhkrjj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxbjmpbr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3djgdcuxu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3grpbykdc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cfpkcwng.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vnuczdfb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fqhfuefv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vgafvyyc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ocfdhdfa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wqycfebk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bnlytfdq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fbextyie.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nujjxzai.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3yidsrcne.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfjuzeug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqehrbxl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cqtdyjkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcpqnanm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3noactdur.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ppztsocn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uozcqkew.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ulbmwysm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3oisnjuug.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vyvudhbh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3aidipyrk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bsmdcvyd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3tqlecfyb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eznsqzdi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3pxzeoxaf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ukwowlbi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gdqchvij.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kcdwwuez.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3clnvosrp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kgnxadds.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxgzmgi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vdvstolj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dubvbdkj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qdqysgjo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3myfwapsn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vagwzjcw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jgyaftgg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vuktaqbn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nrctuyaa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hlllkmuo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dlxacqfe.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nqsnidbk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ljegqnoh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zwjcknjz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ldnlrmqy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3duzddbdn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3txscxwpo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3brsxdfld.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3sqzqzshf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ayzrwlay.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yyugjgek.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ahmtobgh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kohsgcqp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aaxkkmhy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3stirrbis.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3axtuvxvd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ijwmpybq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cfhjvopa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3czugvtpk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zurjvdrk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qiwshppv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bqdqkjzl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qilddzyk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lgfasanv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dilmtyum.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bizfwwgk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3keskvlsx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dhihfipt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jgpaeamk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vejdqvjd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kxmptjmv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ygthgbay.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3eyhnauma.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vfhrrriz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jciwlmmp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ebygjwly.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qqpotlld.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jmgeuknl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3saqoxskd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rdvscmfj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xudkddzj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ojyozbvy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3omtamxij.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zdapssrn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3khruhosm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wjozqjnv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ztwfevxz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3uyritksy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pmzvkpkt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ahedgenn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3yoddrgvo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3gddssicy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mzuaifja.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yjtldxzl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fdtkmdhb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3congdqnv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bvuylvaw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3szcdntve.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zksxvswi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3muteidvh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vpoajulw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wzxhjbee.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ediwdmgj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3izdkbhwg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mvbeutym.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3aoehozwk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vlcuberh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3djijvsut.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ixnhsbcw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hqggwkvw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jmrsuvox.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ryoypelw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ehbjfrcf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dzfjombh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3kspekpya.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iaqwwlfe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3txzujvnx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rsqsjzyj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pbaynups.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3magxjqeh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vhillbqi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3airrhlnu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3snuazhmv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bchrwyin.html


<!-- 参考信息 -->