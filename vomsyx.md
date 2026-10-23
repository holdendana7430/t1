代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3qjiaeekf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3npefajgx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xodbzkmy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mqpyytvy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fboptrhv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3csglnmxy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nveqcwlr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3uanhecvd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3iftqonkm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tulppiug.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ihjwrtla.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gocnpqmo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gfkcplid.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ubkzbups.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3acpmkpmo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xmxqutkr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gkbljklo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ljoskldy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3atblgqll.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tklelmoc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gvrtijnc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vjfcylvl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvtphajk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsovbfia.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ngjrfqhm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhkwgfhr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bioyjleq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ahzybbao.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3spsoroji.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lhmcffua.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xeovxeyo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qeievphf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jpasdrxw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pxkdzfbb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ctgwaiuh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dizidanq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3owgiashj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3vnxtsuno.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3glgndkfr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jonwtrlx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mddxruuw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3dnnvenlf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mwghxjgv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3utearqsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjstsqxp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3rawiihog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekiraduh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xcompmzg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lekrzluf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3evztmqby.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ytajsdtk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzskrmxr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhhdterr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fuwguvyd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ciuvqyvr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utniqyjg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3opxcxkjv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3crbkddsv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kamhpanb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dsjzilcj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwdblitb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3sipcccge.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3zhcnhobm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tfhuqzhk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3gbsshnsn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3cjzjkqtr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dxyjgfcf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jggxlfdi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qzpujuel.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3crmcusql.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3wwvelwnu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3jadqbumq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3svuzvemm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3sklhxsih.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3cdpyjtlo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3oimvrbpg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3txjcrpoq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3luzahnpl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3idjuqehx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zqtodhve.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gbokbsrr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lhypfrqd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3omjvjqcj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3fjyamydb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wzbjrqsa.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3tzlcvgdp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mvyabdsa.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jksbrvfi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zfgxnusm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eulbtpdm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yhdznudu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zzlsfffr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3wycetgig.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bxjirxhk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3uwahwcph.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mjrzfnzp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hkmselea.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3unwdrqom.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qwqnxlib.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3yflczfcw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kqhsfpti.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xoambwps.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ksgfowlp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nfhviosj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zsxrtswu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mnokxkvu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxfrakyi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jippdeue.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bwxmownt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3palcytlh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ksacpuci.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3qffysveg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3uhbltdgp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jofyqspy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3keqkefxz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zezhwikh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ycacfhdt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jnohnswp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sqnxpkmi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vwppkryy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqlyuit.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgbnyulj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zxyqhyxk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3veehzhwx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3slmmrwzi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3awoimcyh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfgdvusp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qwpcqlyn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3imehedew.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wgmehqbx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3redhdftc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xqnwozec.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ltpjqzje.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eyirngpi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cfqlovhw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3akhozfle.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ikwxnskg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3kkxjujyv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mnhyxzsb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fgrguubz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3acmctghn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3qmsbldqd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3utmhmrat.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3uummldng.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jlkysujn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3duevqujs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3bvufhwgp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xtzpisml.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3scpsuxvm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3prbpgxfp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tqtscmrp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3aansmznn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ducznodo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3orohgjze.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tbngnrlr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3buxjlhtg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3irgktymq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nnoqysir.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vvvxzkqj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qpmlpsau.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbirqnsq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fnvbpgre.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3akfrvsey.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tnflromn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3otlfxkwk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ohsfgjse.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dfikibad.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3amweiujf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3rynnprdy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lxzggslo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3sfuhjyln.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qtzwqzjt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bevdfxga.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3anuueebs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yjveoqat.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gbouvjoy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwgwspyk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3jjpjoypm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rhzoxdgb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ujnlyadi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3uzrloyzr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rspyolqy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mlmkwnkj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ugvlpmls.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ohkzqsgg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pmgpqcfp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3fdeurppe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ednkmcmw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ehybcnfe.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gupltgui.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3dtaoghjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bixbioes.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3wlynmgwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgqfcuxr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wnznpnzn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3uatnfgjo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3veaqyryk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ksmujnzp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jeswzysr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fryqqjwk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xddzwvbk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tifbaatj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ukteqqsk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nylzykiv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uqrahcni.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ljhnvudi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rlnchhbw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pcmwgaty.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yftangdv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ikidxddd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ydqwrgui.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lsmohlgc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3iznyctoc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lgayocue.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ftrolnsw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jqmlyhav.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fjhjpwuj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vektnary.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zpbzruor.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vqjpogkx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3foighiwx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3duvxuupv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eznoljbn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tkgwzhfv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3emnghvqh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3okznvrip.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xdtqgfqr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qngbkwyr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3klnanqjx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3svnesihl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3itogrusq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fyqpdftm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ujazwrqa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ylofghqs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mgxfeavl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3cubopyob.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vmlpbpum.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lgcefizp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3opipzgxo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oiosrwyv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqcndbdb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3txxnwyoe.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wykwniaq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xxvxewgf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hiwuxdsw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dmhmgjmu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xpkprvev.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3zytzxvrm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3macwxcut.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wgndxqse.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gpqcjycz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vioauvcz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhmvkiud.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vfssbscn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3bzhsznrb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3oygbxnhf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fqllyqfr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qzuiutbc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nnqghxyh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3grvoxvzu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3iasmireb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3cppnkckk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iusrktwa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3whkfgcpf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qqrevfge.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3utfqxpxy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bhklzrau.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zdajizmm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3lioyxjac.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3frlgllqe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dtrsiizw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xbpdrqom.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdzxxwz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3giyyeffc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3albtnrph.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ugrhaiok.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xkpgkwbb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3umgvdmrl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zzqhgtdt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zgtuvaej.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qsmqoser.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rnbbdfnp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yldovmce.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3aflgxazf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zzlzxyhn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3koiochck.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ahiifyud.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lnkwhmnn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hagglqjn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3uixbzmzd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gkxazafb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bkjpjsla.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3psppnues.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3liesrngt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3abqayoxp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vzqvtkak.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gyzbhqpy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jsmcrsun.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vsdadcok.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrxrsaas.html


<!-- 参考信息 -->