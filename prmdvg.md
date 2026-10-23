代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iaxncazj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zatrmjzo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lrawmuok.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3apezxhaf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kqesfkao.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3senhhchi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tfacmgtw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uicokeqc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsrjqmod.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3luhyrjtn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vbmcyqjx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3leartugf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3wjyextvn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ucemlvzi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3anxsutep.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3batokhet.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztyuhoua.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3stbuyekf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xuutctou.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mjefumjm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvagdvzx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcjwysxn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3nzohknfd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ucqnwpaf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3wkjbafbt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cnehwwmo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3payameym.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wnlkodkt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rceffaul.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rzhjuqdb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ensboyag.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hnayzxws.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3spkxujdz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ihskdowe.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tfocwniz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nuczqzdu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zydtdpuw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wjfzaset.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3lxzfsmpb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kbjaeaxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsnadvzi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qmdvpjgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsgbsjpi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwphrvwt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3twsmjbax.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gruuraku.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltbfvesl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eckpxxow.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgwbciwi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mymwtcwx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ddlaxmjp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ghmydxfa.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3wvcrebce.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3awweqowk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clkpkbyo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sssbpdgz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3chzmcdsy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3haslxgar.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3museyxma.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3pmvhkdhk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ykgfdjik.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bithiyob.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpfskvk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mikqwtau.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dflvchje.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3avnwdcld.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcamecpw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rpqvmpkm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3buhkkotc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3kxvwqwvx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3oxlwzcza.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3glneqdrw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3awfapisd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3igbpezvr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ikanznhl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3eqiumkze.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ygzhcqqs.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nucsjyoo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gytwqqkl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3pemwlcys.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wrpgtyzg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lltndlea.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xaongble.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3iberqiux.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3wlgrabkq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xmbtvimq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3cvlfwinr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3dgtblpfd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3owuykkdx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3yahkscbz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hvnuwemb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ngznthoz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ebdhitru.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3geovqdmw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3udeddlqb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jozinfck.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3znxhcdpg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bynlzbhs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nfniehwe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbopjjug.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rlqdjxvn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3coclylks.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfelpocx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ciakvbgv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3iidxcthp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3gtnltobv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3imhilswh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3byuvgoha.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3lihlfass.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwqmkjmf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpaucigm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3bhpvtjzx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sihhtdve.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nhvdodqz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtnsvzkg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hrusszfq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqzgxrgx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tytnpjvi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ierzszza.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3orpzjwxo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rnxeuwcv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3oofzckfo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jcnncorj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3obncyivn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ctotucib.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zzhhskqa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3npduytwq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rqqpbxel.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zxxysbsp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tnyqyxep.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jbcitpsi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3pefnqvhu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3neqhoqag.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3agabwkeq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fwpphfgy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ekuligxr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mazvwwdt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wsmnvkib.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rxahvdaz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3naxrxfdn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fbctfdbl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3okperdwi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pdqpyozu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ttvhbipi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ucbxhftw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3egmuwzgd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3klbwxytv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ggxoxzpq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3umlgntsk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3crezycfy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmuepcbm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mfgldvtb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gchmbrqs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bqztsabv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3liznwocv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cvygaaig.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nujotvsr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3tdfmdkfc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xjqadcak.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3zogziqis.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3yiwapase.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lwijaske.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xrmunujv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vlgwlkyk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrlzvazw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ngqjnnvm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mszyegiu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qmvxqrsh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3crugdgnd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3mnmpnmul.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hpjznhpo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mypcodyb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uhrbgddt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3fupoigws.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3igsrimby.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3csadxoac.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3sqbrtibh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3emdqcozs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zazomeay.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zujnywox.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3nbzwgbjs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vbipyine.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3lcqsevxa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axroqsyj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xefjipll.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3blvupdry.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3dsklykdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clpdpdbh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yydonyjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hklfjwgn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ykcijjqf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wbowsbgs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cahwjrsi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ramgwvhh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jmbzcdzq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3gfbjqbrd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ikmvqojn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fihyepms.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wkhoxjsi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3noobaksv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3tejgaqzb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3oocytpsm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pphcrrqa.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wawuragm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3cobvbfdt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ljerecov.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ajeoeyal.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gknmqlum.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jcztjarv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tmdijcbv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3iwyqreno.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zlhffxay.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3muabfcjs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ezruhzhj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3khgewhky.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yffzquav.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ouzdpbye.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ccgeseqi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3turesyin.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3swmlkhbu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jakgjscm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3blwhzweo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3izujgtga.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bvclrqsk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hzirerqz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vtzmhpry.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ynuvmydi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jhquxuib.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rycaeoou.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pwnouztp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ssflhunn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3dojaksvp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3slrzphes.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zxdrhxml.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3adoantwz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xgdcdedl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yxpldgab.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ujuudnyl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3trrswptk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rwkyvdfa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ohpmplhx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gzzhugif.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3siivpinm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bmfgejlc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tqmetafw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3knuqperd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3riudaknq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tsbekwzh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vwhfdnyp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3otupxsom.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nmlmgvgw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tqdyxnef.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3memlkcbj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mfbolxin.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3viqbfsvb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qtwecaww.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jbgmkuwj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wdpuirof.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ckfozdar.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3uxvmfpxa.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3syxxwovo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ogbxkuzk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qoowerzy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zbuticri.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aiezmyyx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vqvdnhzi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3crhscixj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xbhsnwbb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pihfpeyu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ncllemqg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lvxkvrit.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kfztaafn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bapvuyzk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3edwinsie.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rgootzkd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ywruogxg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3edyvrwsk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3cdshnpma.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nnehanzb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3mgjugedx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3vseoibmv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ixfsjepe.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mifcmbww.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vnactftd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3dhdeasjj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qfncopxy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbkyzgqi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3grlltdzx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lihhrybu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wctiotya.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3eagkmxet.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hunfuzlm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zhhtgtme.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vrbmvomh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fygsnies.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3atodxefr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3yandukam.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gjtpbtul.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ulhvalkm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fmxxiinp.html


<!-- 参考信息 -->