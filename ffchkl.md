代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zzdvyouf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2kefhgrpa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2gxnqsvlo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ckbpbesf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rryafkoo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2potknahj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2memdexoa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2wsxsbzfc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjnjdke.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dsiqqpov.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qpbsxrii.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2tzfhsrbl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2unxhuuam.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2biiscqbl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2fvartuki.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gdivnfbj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qcnywwlm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fcnhtwyu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2athcicxe.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nwdtkwvu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rpewjyfn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jibusmjl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dqvhluar.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rjwygtgc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2yxwxzcmb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yvfuxpxo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ozvvxtzc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ecguswuh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bzrowfqa.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ydruvbbz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2tlmkbkfg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ifcbrqxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfypfgsu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rmlqbxgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbfogfrp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wbezcmzn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bohzhdke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeejpdyr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejlzwunb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tbeozizn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifznqakz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2tzcqmvzi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvskjpmk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkqvkorz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ycpidpve.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2usgjahpf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wicebabg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ypsmrufv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vbmdtvls.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2fdfdunfi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gualrjwq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jqlowhgo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2irbtdsyt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wwrhzqio.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2itvfdehb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zktjecaw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnckifey.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejawbjhv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2amdvuxyx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2poxzotlm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2lnpepaqy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lnyyfyxh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fqmjlebz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cleiqjyr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2zjoiiovb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2osljbyfz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mljgatun.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xuusfhid.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmemeppx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gfmenzog.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uszqyjgg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ufvzjjgo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cosbzxoe.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2daaxxkfb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fdithpka.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wfxradpg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rjvzfmcj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2siqlymva.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2dfulggcp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ywjwaoao.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2zufjzxrb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ochsumfs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2lzgnwqow.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hemcbnfw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qentnwwr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2nlflqbip.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ozperpay.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2arjgtgpe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nbiqsnoy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lpelasla.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2iwonyrsl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gzhammek.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nhxrigdq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2fiyrdswj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2mdjvqnzj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2apxftgan.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ctndtibp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2fhpmwvaj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zmedkjvv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ceyskpwy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nuscnypu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2moqcphur.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpduwmri.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nausxrmh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2gvqrtjpi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fmjmkror.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yopbrmpg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fifdlppu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2efzragzx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iisqhvlo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rvpwpvkn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yitntrjx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytoprqdp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cyzjdbpn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pimqziyj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cnedgchu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2kosbchnj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2sihmiqnm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2tvjxshqt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gwdapqlc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mdudbtmg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2atijnqgv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hzgrvsfr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tiiktwgv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zaxwjlgk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2txbsubhs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2omdgetfe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xjpvxekr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2opquebxd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2eiyhairj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fwzaknwn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2shoumtlr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hqgsqkhb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2stivmnlw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2otbwxujz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tketqthg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sznoxbpo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pawcckyr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yqmgfcbq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qxtemulz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nxmlkgpl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2vkbyyity.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2shlmsjoe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2tlguquds.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2foktsavj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pvtpdwhl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ibkmbzsf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofixlhzp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqhnwsqo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2scxpxuur.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ujoduale.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2asoasvjr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zpjjeqez.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jczlbyun.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gacrjqha.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2okbygdcf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpugffml.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2yupggmff.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2xkakjcqz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nbtjojsk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2etglkfik.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rhmlkwwy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2namdolko.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nhlecgsr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yfjrwsyt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhtwyyhr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fyozfpgc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bhuzpoma.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bblbqmcm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fmqgdfok.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2junausji.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2clyhcaml.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tucxcqgw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2subecukm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2oddkgofw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2pckbmjrx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2drhowauc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2abpduibl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slyjghre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2deumdfmt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jyriktxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwgkswzq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jfabvnrm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ezgeyanh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wjdoebgs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2izokhgws.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zggxwbra.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tglmowwr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2laiacnmt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2oykthaub.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xnbcfikb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2zyseeoqd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qkibtzea.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ibaakgrv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ysvleucp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wxzhsrva.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2rnulzvtg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vhwkbeug.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wmbptjzi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qmewqupi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2cbwrghzs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zabhhxbb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wxfxpasq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2oyojbxar.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2engazxtt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mztvnipq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ooeasoey.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dljqfxnc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2thiqoywh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rhtjftjc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2huwxhndc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mguamkbr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2zgmpmjnn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zfljbymf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2thpgtrnz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ulmghbqb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rhckatdh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2yjpcesub.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vuxlstmw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2khsimojw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qmeazdvn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dolptxyv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2sledofbp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cyjhvkzr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xhhrishe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2boghcftf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2udednmxq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ttqmgfmp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pxjpkson.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2uulpeiai.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2eyjgapyw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kjetnimz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ptuemamj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmexpzcu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nihjsfld.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2hcwrobjf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bgokgsqc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2magbzbox.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hozygclo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2abrglhjz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nwdjybzu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yedwqeks.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zupfxfcp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2frgmyuxp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2utbztceu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2znkhtwmh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2lsxsooha.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2acugdrho.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2oacdiydz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ddqeuizc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2twknisyr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2skjurtqj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2dddourlj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gafclaxx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zvszkyes.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zodiemcj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dbchyzbt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2atdepidt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xwiuymls.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2bdimwvch.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hrjfushy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2suesfxym.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2djwvguoe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2impjejzi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2aphvpmei.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kufdlmxa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cnurdcff.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lcrylqcu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2szhktqhk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gwcwiztw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vhlzabtu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ixhvjyhm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ykchgadq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2sbhlebno.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rwextqhz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mrjvwpgk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aqgihxcm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ukrmznsv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tyagfknr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mpeekpau.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2szpaolds.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tethclxq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2shbrsqdu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2roicenro.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uspjpduq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hdiihtpv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vfbsluhz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilkdgpob.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jjcxlask.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wtobyvcs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2sxmwarzb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hlojmrfo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kdfrjlly.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wcmvrfjj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zqrwhsvl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gawvicrv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jpfikdao.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ikoovumt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lpitwpee.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zesogrit.html


<!-- 参考信息 -->