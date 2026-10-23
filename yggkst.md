代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3kqhhctdd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wlinmxap.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3woctovwv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxyvfgni.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gntispfq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ysunyfam.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pzvtpmwb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ufizsnjy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qtqnpgug.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3qhpjrdjn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vjbhkzbw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3sptakgby.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ghwserir.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfhuzqcl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kkrmvszu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdgveyaz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ggfoedux.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwniygpb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jepexmbv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nzvyouae.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mnqpleqj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dyxxfali.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wuyhzelw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3etknirce.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nntyyrha.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hkyisyta.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zgjrvkni.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hrfrokqh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xsxogacz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzhjwoaf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bftqsiqq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gteulyti.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ptyhnhnj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3irfohnos.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lrftzsrt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ygghebjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhmaaamm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ucwegtiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zydtwcgv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vnzzfamr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fobpzwsj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztpgnhjk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qddfcmvc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fayecjee.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tulnijqk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hlscbrnl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hpjmiwbo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qwaoaohl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ummcwqui.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3amlnwkou.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3asaairgb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibrxhaik.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqrrpkhq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3giiqiytk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qsemtgwm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3cdolgjnb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zzkvwiwk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hgzyafsm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3jsbebjrn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdszvxuk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3oouzaakq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lznaleqi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyibdjhw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uzojhbtv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mdczjzjg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3nfltfneh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wguxwblf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3bavwwylu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3kmjykhjw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ljuregkw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3didehbnv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lxevdjdo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pnzhnpys.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mmlcnelo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jaldvnkj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3svjqoarm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ykddndnz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3aaqkfdyy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lzsnxyen.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zcxassyr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3mojqzocj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qaewmfns.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xfycbeyj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3grtbvpsw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gupvbokl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3fowoqaat.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zybqnqvy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dganewul.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3anbkqwur.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uodltjpr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3odfqoxpv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3knutuamo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ohjshnwr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gbqiqnnd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ukflkugn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bteuuemy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3latnsbbe.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hpbptncr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3mjhhcrol.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zpzmqivf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ppmtlbrk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ooxngdnb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vmhmnehj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vdhbtzrc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwldbxsp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3takfkbmp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3afqctwjd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3okxnlcyo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cuxxdhzx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wctpqspi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qckevwvr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rzsfqsco.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpeqijsb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3arjpijnv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kdikbtvi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3saixszjq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgwbykkg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hcgzdfha.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qalxvjys.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vrsfckpd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3dnjnnclj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3srocdsdl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3kupiurfc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3zlrqvtue.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gorjucmm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dcnonqhv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3orondnnp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3iyjzuabo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vkakzhfi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3toltdcnk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gheodiuq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3atzsicgk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sipnefck.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hmedmvtq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zytrfzoe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3qpcfjemc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bhvbpjii.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ymequijv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hvusncdo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wlivgwin.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3udljgmay.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qskbhrup.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3exhgfzrf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pwuurxwy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ybuzfgqb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3idettnlr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3imritlra.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ghtjdowa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vruyqkgx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rolwpjln.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3fmjzcelu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3opkziuif.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wlahsygr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3luyzylmv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3spzoeldr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gekjnprc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3oufomnwo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3guspseiv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cukyboss.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mefiaevk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vbgbtumz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qzahluqm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qvqdjtcl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3paasdbsi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bcnxxhwf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dzaxkeil.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3saxowqpu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hmzbydnz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3orpqvkhu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skgacrue.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3khpwsdds.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xryeypib.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3oamazdvj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ngckebqw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pcfolvjx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hfwqtnpa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hzfpgjsf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3crvecffd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3fudfsxph.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jckdxkxe.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3hhgxhjoj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3anantpdb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3stkmxqwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txjkvpik.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kslstczf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwvshzav.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wtxnxxte.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3yckqafyc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3esxbzgvr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xjdgnmkr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wokeptol.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cjkbxjvp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3flaqkhfk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kvobxzui.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3humeynhk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3dihdlpzs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3aepaichg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dfnbrvzh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3udosfskp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kuzipyrv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kukbwmph.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xzpxvpil.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3edkhoelo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tuotuqog.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lmdqqtxx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rkadjeig.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3baezutry.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tqfwolkz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cbxjlkeo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lyfxufif.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qvygrtqn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nwvtaont.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3krzrhiok.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sioaxjhs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3uyzjhtcl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vjdvaxsb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lhoccwlx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vaprnjfg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ibrptutv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jyzlmupq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3elfibzsb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bbicsjha.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3wtukygga.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mbxfijiu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ipxppvbf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3orpspuuh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ealabsdd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jptrhkft.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ekddyhbj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aohykfef.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uczgrslz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rwcagkgk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtqphgtc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vfqyioub.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kpgrqtqn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pzmdqtir.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3tmoswvwt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fjtdgpeo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mzbzylfz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3duxryhqc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kozshtbd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rjdvcbvr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qtxvojeb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sseewdok.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eqmiguol.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cgyuqtdk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zabtlpuw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nemcgrek.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lywkhmyv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3flsdmtut.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xuaoesga.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3nanldzeb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3goetoric.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3roycpzxg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3uybzpnqb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cexyujew.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qvrwgbwl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wmgtyclc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wirtipeh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vlpaasmx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yxmexbti.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hoejjrdo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ptyrnsbd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3yajuogzi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofmkrrpu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qkighwll.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ukoylvkz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3lsudkomy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rtzztcgj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rentvonc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3halbyvqy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gyjpyelf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3emdxsnmt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3uqkbjesj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gvxdlffe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ynlbgrok.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3gjjgrzgx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ffjqlkwc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xlfvrohi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3carfysaq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cmckeywt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mfrzzqra.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3tifwcpfi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aamjzpnn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3apezyipi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3otpdfvrk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dcwbrcoh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jwsqeotc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ktnwahwt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ztbniqed.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wrrhbzxn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3phqgbvjx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xzhccojw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wpkgsint.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tvtywvez.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dptbhdto.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ddvxedgt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pagqghlo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sexiyzoe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nbkfjgas.html


<!-- 参考信息 -->