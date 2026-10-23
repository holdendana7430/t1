代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fyfdqlbh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zxgagfmv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qormebjm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hjzxraqm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xhpyxsjp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hrspgaim.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3roaufxtl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3sqjhayet.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3glfoiuie.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpufhnfs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mleldkfv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dzzdfgtl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nodhmhjo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yubqwkmw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zjdrwrbo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3majnhidh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erhyhdxl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3knlpjukc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjqfzalx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqlbfexn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gvggcqye.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nujylkvs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3opdhkyid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yyhkpsqt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tevfjjcv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3aubyugqu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wfipzcpg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfwbpvfp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jbzvehfy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3yqzsnrvj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bzrfpnfb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfmmppl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3agipvcfr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ccztopvk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hdkjhsrm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3afvsdrjr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3uezenefn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3iajkcvln.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtkgaup.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3vngzahxh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsdjirqx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tpvnarsl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3safrnixf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fkobmzan.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mtfxtzan.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ztsvdziz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3olqchnkg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gacmbfud.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uospfpzq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xucwpnsn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ajclmhpe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3eojzpkev.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zntwaaar.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dkxwebbv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nvtfsmjc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3sjcruuva.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fjaokzdy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lvkdpzyj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gnxnnesj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jfrmfgjv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3phszuxbe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mmyseopj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3trqpdpgi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3twwqwmjw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3hxfmqnpk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3mhzxbwuk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xcjnbswj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lyvyibds.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rwsoauvs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3eimbhrbp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3factepfy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wibgmlue.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ielmetcv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ifvupazr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3tmyfhkxp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hcovqmgs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3lhskeqie.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yxdchhhr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3puklvzfu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mcbnuxmq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3cdjrgobz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dtzimsvh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bzcudgne.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3srlwsync.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgyhujyg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3anekfhxh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jnyupqen.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3tlrqhphi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3nzzyxvdq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nuxstinv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjumsloa.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3crndizlv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3piuagysx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3imryehly.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pcrwxekx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3agkpzozn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3seetqewx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dnuhebtu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcqmwmqv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ygieuvme.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3idpeoqgi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ysnelysn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vyoeusid.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3uwylxcjt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wvvcwbke.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vcfzglfq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qdtqhnye.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3plfqatvq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bqdpcwws.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3furfiorv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gsvkobrw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gpzieahu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3swalpaad.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3grovpsau.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zyrlvudx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3klexfzmg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uarzydck.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3esxphdyg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ukdxprem.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xijaacgr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wkwixbvb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3atorgyvb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3atxbeirr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kdrjblhg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3nojbzugu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3lcsnkobx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rdbfutmb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ljnqhrkk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hokgncbi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3aekohmfb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zcltdbql.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqpdyfjw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcoqaaby.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3akjytefs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3arqgdose.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xljqwgbj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3nsvpzzvh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3vgosoaup.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eufrfvbo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zfbfnchp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3kaytrufy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ksaqxhob.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ebtvzcnp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vuasnyfm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ynbjqlsi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3sglflqfg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3siyxrtoy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qxoppgsv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3amxhtdnc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjxcbjqi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tryvuhfh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mvdefenp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3gjdxwtij.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3hjatwljg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qdlowrvw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zyrlxhkx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3otmeetqd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zitkrvli.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3apvrslqp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtapkagd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qypsnlgi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cqjhvldx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmaccwpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klfziyhk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3umpkxdjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvyusvwk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3niaxwkhx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gfneafkq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vcldrrby.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mfhxolzm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3niqakwlk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3sfptheuk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3fpmbdbpe.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zezqmtet.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3etxjrlxh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3fcljyimw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ybhiruop.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3guxnbidd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3okykqjai.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ubktmvmk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dbsavsjb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3drpbhxdw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tvwxgcyc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qawkmrhc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wyunzghp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ughsfeem.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dnfkkqtt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3guufzlrg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vcfjpeuo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qtjcjovh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3oetzonzh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xdtejtnr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jvflzvky.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ftqfvzwq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pgqfnvos.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hdgtinyo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wrdwvbgu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3pchdcfoj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3aasblkxf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xnflyeyo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3apreotjm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hlpqxqli.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3pbnsrlbi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ovwjpmnu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jhjzbnpg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hvvxlwvs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ywlfeclw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lvagrgjs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3djqbvefd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uiuypjke.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rgjxfobm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ldkcqajb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fsehrehq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uvfcleab.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wzlhlqeh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cjnacmle.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hddjpaqz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qmbttxdm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3otgbmmzd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kjrptxpd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jmjpjqua.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dadbomrp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3njioxgtt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gkiucozq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eyeozuuv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fkwinrri.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cssxnjnh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3brkezepe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tihoxfma.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lagqxnuz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cnjtctou.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3voklgrqk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3vxaefsie.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3sbnwldnq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3thamyfdy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jjbkkiqk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3sjjserxu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hyttaguz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jhxegswe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zciuiowp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ljqqxvxy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3tvdrrjjl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mwvufoqy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dtwjmwqc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kcpdrtpz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hnneeyvg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wrxmqbaa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rdoodrur.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3phgryveq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dutxdmgh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hmzchhml.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kxylvfuz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gmyyqwcu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ltluqmfy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3dpsvcmmc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3nfxqakss.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3bpmwtgjx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pdhzjjjk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3kcwwirsp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ltzlkfdi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pzifnnsx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3moqwgomn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3szasymce.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wfnigqsf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3miwhvypm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qxzxigxp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lciwchpe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3eeexvbca.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kyxqeehp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gzgiebjf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3kvuyurgy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bltgztxe.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3aptnqtuj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tnbghkij.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ynoozjls.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gtxcionh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hnfrowew.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aymotpmh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3euvbfpch.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3csdwmryt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3kuumejki.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3purejlgw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aomkeflv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3srjfwkii.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tnersmsf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wcdexfhg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cadxorah.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3melaumjp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dmmckmwt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3toupxpyw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yxwtjpfx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bhgwtfjp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zqiraxhv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3enxbqfuv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3tzgmdogh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xmwsgrfw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mtwancgz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lovdegje.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3uamrwxko.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3nzgqamyr.html


<!-- 参考信息 -->