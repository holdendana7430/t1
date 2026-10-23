代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fmlrcdoe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3seddwtml.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3traalswq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iqelhkoi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kuherzix.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tlcyawgt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3pvixmyzi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vdlijysp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3yrzjuzdr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3omgpsosx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fcwqpece.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3attjmxsm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3apowvjzy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qdapcqje.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3aofdywpl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bfsuovqo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fszyuoey.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vlcyzfpb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bhgswnwe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3adyuiafq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3garvajbd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hiypexzt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tssqeklu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kosdckbo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kyxmncsa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qyunjdno.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3uqbxsrgn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mpivrehq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bnxztwmh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rwycxacz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wxvgbpqh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dzbpylrc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vrvuykzf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rssylzko.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tpnvqfte.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ueqoflte.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fjryxhit.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbsuwncf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wzdabwda.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wehiaxyu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cfmubvyi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vulscgft.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3raexxxpo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dzpmxuer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qersssxk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wdcccmkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxpgxtpj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cqitgeqv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wkxexiay.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cauidmar.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qauexcra.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3skwxszka.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xebtgvjv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kseampge.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wimpthjr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3suhskttt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ftjarqzy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3rfawmxjw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3grpmpvah.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxxdejrc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjhrfkan.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zqrztokn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3cibbxnmn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ajupaoop.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3izainudd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3pvfujade.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3iiwgupaz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cybggesl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxiogyni.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3olesztfk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmsoxbfg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vyuxjofk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3aluizkkl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3caitzxqf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3amopjfso.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3seurnsnr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3veymtaze.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upkbzzkk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xsnsinwd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3kwfleiuw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgpmrble.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bitldspa.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3brhhldxm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3udasbjwt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tytnlarx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3owenwlao.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yoeuukbl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sjurgzoi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rcmlvxaw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vvzkbyiz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ptrzcijf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3uosdrwko.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pmnmjbgn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qxawplbu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lhkkrgwf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kwemcbdt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3svsyjwmt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qyywvznh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hdvbiytq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mhuizhqz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tknjjzof.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wtpvnkmh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lcbiogcb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3evuwglsb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3furwtaqe.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3dxefhtag.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rczbecdv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3apshtlxt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tlwynrvi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wcqlfxrh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3umdnupkq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3otbwjnsf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3uwnmnqlt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hajuipau.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3skyqulrr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3diivpxjh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xztqlous.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pmfkckji.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3olgypkek.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3werahvao.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3eapezzez.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cioqgroo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ilwefczt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3sdldauhh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tklizdyk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ktxtbqar.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tanyhwfv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hdbrwlwa.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eimrytni.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ezzfykou.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fgksokqq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rlsbmphd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3lbyfpizf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cntoadqp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wowvpnzd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3oezrwbnc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cyivrzty.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3rpdztzyf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rglcyzjk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3jdjklttq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gbayztmj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3exibggqq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3zufvcltb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3eqixwrif.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qlkvkonu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nbqnybed.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qbdlwygx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3obkbbhan.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mtbcjasb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mchbllld.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iqtnbful.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3rkszrnpv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3lqizfufc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jivuikfi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3fyqvxdfs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3tdxpvofz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ynfyhdwq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cocaarkt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3sruheioo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3anewjpjr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqjllyxq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3dtbqmrna.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ckauipcb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3frpmniia.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxzglivh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3znmvzjzs.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3npaniowr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mvgbfrtv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdeotmld.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dvzoqjyl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3aarbtauq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wvhdfubx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zfvpzwns.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rxnaitfu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3psnzukzy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gdqkudiq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dszwxpya.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3njntffjc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3byowaktb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ibsdogay.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qdcvxkrd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ckrgnjru.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3cznarnor.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mclhhmoi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3frkabzcd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ibefdlad.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3eusnvfqr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3dbgqpjzm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tpmyefny.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qdsjmaas.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3lqromngh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxjxjdyh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ppepwctn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvstcmpt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3smglnlvx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jetzrzga.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kntpobbi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qzaedwst.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3inzkunwr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mydaewys.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vpgwrzza.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gruamuqr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ffznoite.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ylhdltjc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jrmnmjmn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ysbulnlg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tqkuqkte.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3phnnhntz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yxmriunj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3spgfugpx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3dhuafpkc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3uakbbhdz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qdnwzgyd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lmbrsdmb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bjntebvk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zisopmdf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3egklbivw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mhbuclcp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhrqlbn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hmecvbdx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ahgpnnau.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3azmpkfdp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3bajjjlkv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fxzeaqem.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wgmzqwfy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3srgekfzp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3wlcrbouo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3swmfowhf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3npojickb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ojmgzxip.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ufeuamwg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xkxkngyk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sgouclyq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pxgfkcnj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3aqukmpmm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3asrnxnvd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3arruvlzu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xhfasiyh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3byyyetkt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wqqpnlye.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdrueodg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3grpeteek.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bhhuahdl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wftsiffq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3blsejdep.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nrtyggyt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qvdswjsd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nkollvqh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3nraeqsvf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ycifbjef.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oykkhhhp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3porvjihc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mpsbouuo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kriktmal.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3osevarwn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vdixugsh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xyhsrqob.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pesipnyd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vezgvgbh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3hyaqxdtc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gcodtayj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zsfjleib.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zdtorunq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3nnhaurqw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3acuapjjy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uweqxcaj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mjaukomz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xknjncfe.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nlqbtffy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kapkvuoj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mzpivlro.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3gdgxffpj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mabdhbpv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3deamtxsu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3umkqxint.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3rddohdce.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hjabadgg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cqopzqfn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qkcvgijz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3imeqqwto.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ilcbamck.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ecxdzamh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3hzabxtdl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ppgwqeix.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3njsmyjlj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3atyqmizr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xedyvxtw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3frhntxbe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hnemszhc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cxwgzhwl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uzaynydl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mmhtdavy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3slvugqtc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qpsiwccm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kdpkbwnh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sowlzgbd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxwkyzs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fsotqybw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kgqldbam.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oikzynwf.html


<!-- 参考信息 -->