代发 wailian999

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rukujhgx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tmnafttz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3akqrrrkx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zteeqjke.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wolzihfo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3nuxzanxe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3cqkkuhcf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lbtlvgat.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jiwcqdut.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ogxbvgam.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gtavqydn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3utfalgsl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ijkgexiw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzdatheg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3krqvciuz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynodvaio.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gkiromyw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kwlhqtoy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3nyjvfzhc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mebmyhtq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ctsjzfhy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ltlmalsn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ovupulxx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kaauueqb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yqauxhug.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3amtjkijp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rfrlxopg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wxvvnkiv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pmubzhkr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3oufrmsrv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jpowdkgb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wjumvmuy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3brpwwnwr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tciipppk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3plnvdhpo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wvgsucho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkncdpbb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jonndnit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfgqqude.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vmiadrxp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kqaizgxm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jyhuuqep.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mggdfcuw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhuixbce.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ampalbkv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ezdixixb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zuoyaajb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bnkgyxvw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fefrwrwt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3opizapbn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxserxcx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dpcpjtwh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3prhahfum.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3effhurxg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3cisxhxcw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kbwpopbz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3iahmkuay.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tmchhwyg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3lnlqmqga.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cpxgcqgw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pnggeddj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrubumvv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqopjawv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3nheyvcfv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3rlnfcnnh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3iilppiui.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3xuniwvha.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wvjgxgov.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3kpjlghob.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hjeleewz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jcqdgzmb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pzrlafuq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3isyoifkn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eppqqcaa.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vhygewze.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dykrnneb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ydpwslti.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uknzehhm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nztjqdlw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xeckqvqx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wpwrcihv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xbwbvonx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rxcuakcs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3sexwagja.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ufxlawnk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3eybhmzkp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3iffutqds.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3viyegswl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xkaworwl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uktqnsti.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bbuzgnkt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3emkjzhzx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iaeshied.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wzqwiccy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3cplgdtia.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kpflpghg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3awufcyoe.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fnpliwsl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3atbwuvxi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pzaioqdh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xlqjddqm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3idehdvxz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cqotcylj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mrnrffio.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlfbmnbo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqwgovxs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxmnhibh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dtemkckj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qcebppcj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3shorbbdd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3frjhovco.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pfhsnndd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fnvkxrwr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wybysweu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3arjsapjl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jjavyqce.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3iqegmhqe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3gyadmjoj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3typthxhp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3napxwhlt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fvegkqqt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3oksbkurf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3dyxtiavx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3onoeuchh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ucwgaqfu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mbwwwjbe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cvwzacwy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mjsbeoaw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3usankzvt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3menwvtyk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3dvxmodth.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3fxczngea.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qcofhgvc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cwhaairz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3onwsxunl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3lluhdfxa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3edugoybr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3flhjsdul.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3oaqcqwly.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xmbeeegs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3yupypqir.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lhnkzncd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cqpwggry.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jusumwqp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wfrfenve.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ptzouzml.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3enszeafj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mrndttld.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nsxkxibj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pshnimla.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xcrphwca.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xyxirkow.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hdwbtqyx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wmgtdukp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mjgraolw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zsofkakq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3jxvtqooz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3yudigdkz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zscamebc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gvaqxmnq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnsuwhqe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3inoqhusg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rcchsnpr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ebkbzwnd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gxnavmsb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ucpzjxwa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wugkqsij.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vewalync.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xomryjmb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqxufhvq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kzbgbunn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3edhepxxn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3csppmzvh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nyjkwcmt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ywtjbsra.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zdwfhqum.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3tnfzuexu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3yfcnedmx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qqdmcoil.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rtlccexp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3znfbmqma.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3psodckmn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3haabhbry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcmnerwl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3erpvznki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3coxremra.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ygwnmrrp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qhnhkpyg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ejygyrwy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dxihgvho.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uxiepsyb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jjmlputu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3tddpadut.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vylwgqyz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3uizzblww.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zhnzlkax.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mhssizrr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wsrapkaz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3otgjhgjc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hufadmvt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3axhhmpfz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ebzsmiyc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nsginusj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kouyayct.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jyqhmpud.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ixcpmygr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3rzfmqlbz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3loeegofx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jmmnoxdt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3oqvwdfwd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dmfbxxdc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ndgtruah.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hferwxbq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3gdfurngs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nfpdudsv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mvtcvhdp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fpylpqns.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3onipmelw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3drjnbiue.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mloeorpf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ttnvxngj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jseazuzx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3skwyalba.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ahtbslji.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aqfgjvyf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pnzsvqan.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3etbiodsf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ixiqckcn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uzpoqjqe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mpobeson.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oagimwmo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3auwvvzhc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xkvvzcie.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hzftsfit.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nfgnoprk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3itywqtuv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ogejhdsa.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3froxrzkz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hnbqzwjf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hkqlyhjn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3klxdxtqx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vlekxavw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mdsnyftq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dirknczn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xiewcgps.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sqybvrzg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fehdysqx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xfhrxxwf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ellbwenh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zdhbddvb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cfctlbye.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hwdlygzz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tfasfdvb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3yzpafler.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3erzwxdfd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yizjtqmd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yzuapbxq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kyfpzgox.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ldrvdcbh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3shyveugq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nvvclejp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3byftqlgt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3napuwiym.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ezkaflss.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxyvtxgo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pjjjnhid.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xtxegkmo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tllyrxge.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dgaoduuw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3thzkhzvn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fkjhjmom.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ufjnotgt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3fabtojns.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3mvvppock.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cblokquo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3uqkmkhkr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3odkekhtx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3zlcthzqi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eikjhtqu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3efdydtwn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xbcjcfuz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3cfjtyhpc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ugiyfwkl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fdjrahqn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ijlwnxse.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gykffjub.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3tebxopdi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wzyuvcpw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3drtgvrhn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxfvebx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kuszlwvt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjhsotdw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahzeftcq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jiiqsdcj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wlyoxmob.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iyejplsb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kmzmlhdd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3aaidletk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qulwriqg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3psodsqng.html


<!-- 参考信息 -->