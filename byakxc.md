代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qojkbwdy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2svsomvjc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zaqzpcys.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2expguded.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ovzfispq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uaqskhlu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ouzefuri.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xobgcbkv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2kfwauqzl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2nzrqccdh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ydrewdrb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kavgilwd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dvjqhwdc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nzwztcwg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2nyombtup.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gzxtbwkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pelndvpw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yyymmynk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlohgwkv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yaekkmgm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2owiccoqe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dsqmxzds.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jfvwtosv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2asfncgza.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zwecqctq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vqpqchbp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2gstivnhs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ajnmptvt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zuehroxt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2utzdxrli.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2exroarae.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2boyaiyjn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kkkujwkn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2leooguju.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ggbcwtzt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2aamxfjsz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jmtulqnw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yjqjvhgl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2dccbcgmf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhsltvqy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxwjvird.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qfglavty.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wuzerqho.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ryowplgl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2gmbxrswr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lfmqapir.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fjavbufd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsmlxluh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jpshwqph.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zdurnhjw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yhsowjqz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2eqwwjwjq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jfoltmrc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wdrqyqaq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cytibbir.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dvtlomwv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bzqvgwjl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2shvlfdcw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zbmvoueu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vlaodupn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kksdqcll.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uepvdald.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mvfczpqx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jxthrbrp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2aukuwkzi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wfavlout.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lcqxbmdx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gmiazfnm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bjwkcxry.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jdkyeoqs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2pdsngawu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2aimcrpew.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jnmvjttf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2aoehqvrn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2famtoqhi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tnlkkmpe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2wxraxzwv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wgaiyleu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2copychti.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hlqzfmrq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2sbhhkwbi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wfqegfer.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vkpperze.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rtbiezfl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fiitpvtv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ltmarkit.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bxwmtbbu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gsldtpal.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2maoooicm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijljctuy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vbwufeek.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wjbpqbrp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tvwnynqh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pxhmtxwe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2phxhmtxk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2utdtvioh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fdnycwfj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lfolvooy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wlkltiey.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xewmseyw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2evmyoxmw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2yvtrpblo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hpgzoark.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2odhclsoh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wwppdbbs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jfuzsbyh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2icxuidry.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2iuxwumkx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kylhworp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2wcqptcoj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2yyhzuybf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2espgqvjc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ocwvtpmw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nixjmqbf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2dglilryy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pxgjcapc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2aaldqpur.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zpkadzpg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2csblmdjo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2mkcmlapi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ombydkor.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2imquumut.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kiqxsntl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bhwjartx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2krjvfhax.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rcjfanio.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2swicvveo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2usmfjtre.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2cnugvwzh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2taauqtcd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2odvdwjoo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztaxgfce.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ywgbkokb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2aviuwdaa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fwcudcha.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vdxfocxm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvzdctsl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jhermnsq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hzlppevt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nfkoyysd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dsjgbtqj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2djinnbfx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gkgwmqyd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vxckuzpw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2upjfvxyz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rtbcwizs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xviqtqzy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zoourbno.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opogbjrh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkjmcnqm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2spvwwxca.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yfoagyov.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2apmlkchg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ealzkhea.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2uyedevwo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ywzehtzv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2jprbvbru.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rblzriym.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hesomciu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yyxqcpmm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kddqxnvq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mpakpmim.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pptssgoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sejctpys.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2skorgowf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gozlijpo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gafpawoq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2gukkunrm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xuhhumkf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pcteravi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2omdhtkcp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2phtwozcl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hekafcmn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bkilyjur.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ipahljxe.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2umdzmxxp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gwujotpq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2eldqeofa.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2altrhytd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rsolpuxx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iofujxsl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2krzerhsa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zsobkcjs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2usfbvcxc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ngeutuux.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2iqegkesm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hazmasrv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ckglljif.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hzmvhsbv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ereoqhxm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ubjcvutp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gmjqzhpf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zxsmrkre.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lcjzwrub.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ozfaasqn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2crdxbhiw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2prpcufts.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2enyrnuqy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sxtlnrjy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wnphauye.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bkxnntbf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ldnmjtag.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lxmbujnl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pddbnydx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2givkugmu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qhkeriku.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kxxgdluj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ftypydcg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pimgnrop.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nvhbsgat.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jbhdulro.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yffliulq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hfshtufa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gdxgerjt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2grdjrqaj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vwfgxgff.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2obchgurm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obihnsuw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lfrdyhxd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ewfjiqzu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qtpldawk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pctokrsm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xkyiblww.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vornwbnw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2glzjuwat.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ewnwsmkw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wiphrgml.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ojkkppsf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2btbzvxbz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2eqmvljdf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zhdwwyjw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jocldonh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ltujytba.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xjivkjlz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2esvrejdl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cfujpwzr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2pyxeofpx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xtznjtio.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hqknxioy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xbpbjfgs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yplslxaa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2yoicdyms.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ihssqsfm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2gsmfuwlt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2utfhrlkd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ohlxkeud.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xpoufsqk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bydyacmj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ufsrzsve.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zinjzvao.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbmawgr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jxmjwdvz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2sktoqyib.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2hktknqao.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rlvfoghw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ghxzfdbw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2obbkofel.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vflgagfg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2evptbtan.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pusuxsoi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lgxyrbpj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kqvkgpfs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bozyysyj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gkstzhgk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2cbbpfewp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rajrfaru.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cgypnvym.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ozfnbmnx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zxekpwbu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ywuwirto.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2nupuzmpq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sssamwoa.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kosmelkg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pfttzvgf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wzmliwjg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2knwcdgio.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jdrcfeet.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ftcyjoyf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lcxxtzbj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jdsmssnd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2btchejsp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wbgchiiv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nbfurfna.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jdbqgkcg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wnzftgjf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ewrfqmbi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kmodhqoa.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zeychbqj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vbdweiat.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mnoexcxv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lynvswkh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tnysozaa.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hoqdjgej.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bkfrfumg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlhnvepl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ynsrbtur.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2amokfigl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mqceuscy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2lxpbohfm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zqnvpyfb.html


<!-- 参考信息 -->