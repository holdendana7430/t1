代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3alahuxdt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rxfhwmhr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3rfnhsppa.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dpmuxfjd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ttjhzwos.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3usaycdsr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3poflkvbu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pbufevpn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jphhtpvk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jcialkio.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kahrqjdt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3folkcmop.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mkawbuwo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vpouoowd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gyxxzbop.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qmbmituv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3sydacune.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3occeynml.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wgkdgaad.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zszqkuan.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3swttrdau.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bnlnillp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qvzobzsu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nnlwueok.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3vfoiatys.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ijflgatt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pbpahlst.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vxoepdsn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tsfvqxvd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hlnrjcui.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3enrccwqo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hmgcwlob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avqlxukm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3djvdcmod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oagensof.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sosqafmu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yeeajxda.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3moqzookv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3msdogyoq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkmlkxnz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pblppxyp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vduwvahn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3uqcmirmk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltqlthdu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ahpvylrw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dclsdsjq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3geisjqpe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnogweqe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oomsewsv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fwjoeocc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3opgxcajj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3axwubfvb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zctvcmvy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cdrnyqcr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gbgqojvt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kmmklxzw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jkytikzm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdjacxtd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfxdbhkv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fovwdhue.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xktwsdcn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lslcxduw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rizoflwc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3yauapxxg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3roafyrkf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgbobzfl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ivqqbpnw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3yguqwpar.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rldmgshs.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vsftcysg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3luouzdnf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xmzereqt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3exqthckf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3aeltlayx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ccoxajun.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rivdwazc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wfabooix.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bnjuqamb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cqgmvgbz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vwndgeqx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3oiwivunl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vrrxddug.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fnhrlgti.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rfzmuwxu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hyvvyiri.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3bapvovlc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3bguybpol.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hdggaeqq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3avpqvrpd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ixanrtjq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dfyfvosn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3blatzyfy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vugyddgy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3lfzwqhnw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3snzqxtvx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ivsbowrh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3sxytwert.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xliefyni.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gbheyjne.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gdvfvkof.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfvgjwas.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kipnqyji.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lpqzegmh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ntxahnpq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3actcfpyt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xrgitdgv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgovtktm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3quzjnfxt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zikencrc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ngbhgskj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ibqqlezr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wycokjad.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vsgkizee.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3atejdvtf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hichajwu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iptmgpve.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3juykkjwq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3oxyqwubz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3afdnirlw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wofiazhr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xbavetcz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lntyxdtm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ggflydqh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zjsjadef.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wacvnbbc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3cmmygcho.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3anprssdo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ijciiemw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wpyeabcx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3dtkggpou.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3worriyvk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mtqpucnb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3begsrorv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3dwkjpplp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zlextkob.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xoukhipf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wjzlwepy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jalqqnej.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kwngeigv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3flvuxpuj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3yjfbxqrk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jmfmpezw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qfoxarfz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bjpbhhpc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3djhuxtkz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lsjyjvcx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3kqogsxkc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayfrkbmk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3owpgnwgf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3adtpupuy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ayqzijel.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fbuullzb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3artauaes.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pxlomnhp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lizuvwrp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ygrxcgnu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3grgfbpaf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3otusfwvg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3rztboazl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qqzxxbea.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bjlhomhp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ivmwpgga.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wnffcuyr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sfgmydep.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tkisvwaw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rhxmcsti.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vaarsbgg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yxgyxesg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tvbpgnel.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ocqoncuz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ixjrqofw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wbefqmrc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3asnncilt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ertoenzl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3aygtmhrj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ulrzoxvc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wqtvviwt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xzmxuzgv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3uvefkplh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enoijslz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3znkjtomr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcshtgsx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wenbelwz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fndcxoxc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uyjazwtv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tzeyreuk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kjlqdknw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dsydwyre.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ulyqdcbh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3apxclbmd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nowewfox.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mbptqauy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dmhvqggr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3velyhrmb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dnfyoprb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uejinuay.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yznjedtw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ntbehnib.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3evujnutt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qfuuzgft.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fxapurnq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cjkpwtqd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bjuedtjq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yueauzmm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dttqyqfo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jwcvmsnu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3lenocqww.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nqazjtgr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cgaymgcr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3aqcdtcle.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ggoylzca.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3iysgsikc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3cgagsffa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3aqpmtjyv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vpqilnwc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zogiphbj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rvotttgi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3krdxqqoc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ldlevjrf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dlfziuws.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mjcmwyza.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jvqlftuv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3tftxbwnx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mhsymsfo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jiolebxs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kwmvlyvb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3afjuijcy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nyxyewzq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aiojldld.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rmvdupvu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ucutsxwd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zjdcdaty.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wrsmrhys.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3smnsavku.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jagcyzua.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mzklybvz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3fqwfdwgo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3oluabpjt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vmxfmrcq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bxtnehfl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jyvgyduc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ctflggnw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mmqkerly.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cxgxzpox.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tkactajj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3khodmmli.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wcvyfiws.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ztxsxnva.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vcnomobq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3eyqmiyyo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wmcsbjab.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyfzqns.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wymsrvrq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uhrhfugp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3iaccdbef.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3emioqajq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hlkghyml.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lxvjfmjh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wllvfoqf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fmncjdwf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ayrqzdva.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ipkzejrz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3azidagtr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vmidhhja.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3wnrfqppt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hxhyikez.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3epmwdtqq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3quirptzl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3bwhwmipm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qboenwci.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3leiyfjjw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3soacchlq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vjqwwxgp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3aeljrmtk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3awxpwflk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rplwunfk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pdpxxljf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rndrcgfl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kjccbdia.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rchqrepm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mvdettio.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qxsuvflr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nynlveer.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oryzafid.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tlrbnwmu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3waamcory.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kzwpeyri.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mmifiepq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3irtopzhm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3akcptrfn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pmodwwmc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jmaoexua.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mkoeexgo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jpmkwonz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3arqibcre.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvmpnidp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qnbqxrnu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3jrrrxnzb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nxxltewf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3bdxftoos.html


<!-- 参考信息 -->