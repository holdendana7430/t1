代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wynhxjzh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yioeesdj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3zcuvkcxb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qjknayvn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xtimgnql.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3valecrtx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vzklwqve.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bqcgknkn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kfwytcwv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ixbgfiyo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3krdnxdcz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ftqnndbe.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zbwumwkk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mvnddlfq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ttihydfi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xmezpars.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jekuoxod.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tdakjypw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zqrjuxmj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gebuuipa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swvunqti.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jvfhqcab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqjfcpff.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fskbhhsc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zfnyxlsy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzehiisq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3omisrnmo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3obianflp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouevzyex.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ljbuoibn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3djuzwpzs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtxibfof.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zviausnl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zsadsojk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3axqjzjyz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yamxinbl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wuapeplc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dcveraie.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3kkovgbcg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ograbyqq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dbghtxlp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3poynicrk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3iwomxmdo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3euqlnsdp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kcozolda.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqhotrhg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3zytsbvvo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pptxmdaj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3okwkeyuf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hsczyvhn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jtxmubvq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3dzsvabtk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qtbugpwq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ctqsmibg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zqakblll.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qsbzptaw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wtlypwvi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vhzszscw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqtfyibe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cxrtxpoy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zwpjoosh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3spopueos.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dltitlfo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qbvlaoaq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3oegpivcs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3saxwkvqc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mfcjcwpa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3apwxsocz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3deaauawj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ofvrvmtz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3kqzwwdnl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qocmxnwl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fyfpvnjv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vknqtxiu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3svyegagc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dijzpuay.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mpdurzch.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qrlacjac.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3trngkwyy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjjwcywq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bydxdcgb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qzarrsbw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zwkzzmdz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3sufzilol.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3cjgepknr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3binriaom.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3sptxmwmg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3sjmnbnkw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bmfqedob.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3evgiqoya.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oimoaxqc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ofpbyorq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3murbtaab.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrqjysqf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiimkdzt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3acuthcln.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3leqflpoq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfdxpylj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fqueeelv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3promplpg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsrojrie.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3pqdyrhta.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3asmefubz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3yyczfteu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gesjioqa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mskznxqa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3dzoxdnle.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3weqknphk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qovyjfhr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sqixjdth.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3etabhgyw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3woebbgwq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3saazjhpv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3bfuggyda.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3twiahrax.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3diceyngm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3aeedrrou.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lvltcqms.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lzxeiced.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3tztjrgdc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3oumzcyfa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wwszjepz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3smffwhcg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lrqxvqsx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3nvzzvbug.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fxjzgjwo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3edzhvmyy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wrttujrg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ehdccxsb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3acdoyufh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ratbiujz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3lnyxhnto.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mrlteaja.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwleokwp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ubmtqvrg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjxoqkoq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ikcrjcpu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zazkpqrh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3juzsbnxp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lgoujixn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dtkbzabg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3kdlivrwy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ttlwgqvv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gfajwupr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ylxchxvs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kvfvfdjv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vmywiurn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fxupktjj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3oxgjlgzb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cpobmrdx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rmusjgcr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xiqolbav.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hxxnltdm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jynnorsc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zsgionmo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jnpqhrdr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qoqoxtvc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vzxuibxw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rbbuyuhz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lwchzagc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hznuhmfk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vgsjcqjs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bwljrhui.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dssmrwxb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mhzastjt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3clytygyu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pjdemyvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcekquiy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bshkuunw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzfdztfr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vgkztqag.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nzdrkcoj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3scptmjjy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tfvyrnmu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3adfdsufb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3sroheblz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3tjzezshm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ynmnrcae.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kiunjyxf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3dbbtjapw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ldelytum.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jperqmqn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ptaboumw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cvnxgfta.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zjepyyxh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tobwuzia.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3entsliwc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3igbymnxx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qkrnstkv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nvldaehp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nxbtbytb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3forbfgjc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lgarjxrm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bfvyvkuu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cfbhwzgy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3drzdgymi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dgevvohn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3idupwxmu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ouuptbfc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fdpcsfqg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3qeohvwxl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jvedgznr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pljjihfl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kaywyxul.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xylesofx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3yujlomif.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fivvhuky.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bjjmhtqt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3josovbhp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qvhknxzl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3aywqlsiv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3aosxurzi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3elqgspue.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yodlkfax.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hyzkdgzj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ttnehrnd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pfgakioe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tlsqelyi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mzmniubs.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xmldluox.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3cdqibvdq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mevhqsnx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wgmqyyck.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kesumodc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kiuemijd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3msrxiybw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hvcjiuqy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xwvebgag.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pyfwzfos.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3frinxmxd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dqlfjsyj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3roygmhyh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gskazyrf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hqvzzdpe.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3osjryjbg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ehrerlxq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dbcxqdmc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mxrfotmw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zyelyfma.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qxmgvoik.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kwcpqhfz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xkisqwxo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3etmmuxjo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3csrjzxlz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gsrrbzme.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3tdrtlhyt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gmgkchvq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3bgqjrpgn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nedtnkrx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3toozgufc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kzrjqfnj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3aubnzukc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tjhipiea.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ikstkozc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mawpzrjp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3exwwluhw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3sqtgdfke.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ujccmbng.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3eoctnpos.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3qmhnrzaw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3etppdyug.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3arzdqjvr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bozxkcov.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kxifxkaa.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kvfcjmro.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3usojnrlo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vidqweuq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tjnzewlh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3yfbrqidh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vertzjnp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jgpkmurt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tzecoawa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzktzuiu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pfbgzghn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wgjugeqq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nizzfjmi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3duyrhcgz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vovitfyx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bzirccrz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3wqrieljh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3smgbexiy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rbipjigl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3etcbrtew.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lkxvxgaa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ufkuhyec.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ensctadv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tyzelhuf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wlgjypcj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3stlgqzfo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uvidsbxi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohepuqwk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fnhsqako.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rlxmovra.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nlpnhiip.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3azxodupl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xregaoaf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vdxftlvb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ldhryacn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vnpusaeq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lcrdvlgs.html


<!-- 参考信息 -->