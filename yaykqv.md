代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3clvekgmo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lqgfvieu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gxbdlbqh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3fnnytvch.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3pdagdptl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3dfqwasbj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qahqjutu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mjlfuwru.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pqvhuxtu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtyuhbyh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oigzhobb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3juocstlb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eevusjwd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3foanufag.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3msjwibel.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3yqoedgsa.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3swkmlscv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uvabmmar.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tkjbrqhj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zxblovdc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dthrwpwa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3quqebppa.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uaqukfis.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gbbvozmd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3nwrdcnou.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tlgakgqy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lfpnavfp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ubnltcrr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3worazwgs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3imtbauxa.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3gkmebaxq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kkwdxsja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3riwujptt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kfchfhmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unhwjsic.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bfdyxbna.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3czarkiks.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrbzyunc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcbljmhz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ougxfozp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nctxwgks.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3izmftbun.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tywducbz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwyncazv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dtzvffzn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lvrhviuu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btbyiyml.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cbqzqgpo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3stmplhgm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kgvhebzx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3thodveew.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kgzgypeb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3llattdqv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fzzcbqlz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3oaivmgon.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tylgqlxh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lwvdefxq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lrdoaqym.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3aykfgxoa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xdxkclrp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3krzzdawn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ejztfsiw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3lzvwsjtb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3sozyglyd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xwkdjqdf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfbxxkho.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rundyhas.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3aajadosu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pgwcucuo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cgaayxnd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yidkevbg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vjhriqvj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wwndslaw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bccitcdr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nkvgarhc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hchvkojm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3pmhlpbix.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lkjpgzbv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mjmryemx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3xpwcelqf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lmallzmr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rzphkltr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vaidockn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jrzstyma.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3txhwquak.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gbqackzq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3lxigkkpn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rdfleuoa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uzwszume.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3zbmgvlzn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3sbfzjxcg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eucursks.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3evhmtgrf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gefrhkxt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3niwrslzx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3fcecnqnu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ufrgtncc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mrqytwxy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ysdcylsi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tieedeod.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xctxasrt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fktmjcgy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3phbxxnro.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3scynqkte.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3cgrsseok.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ivmjqpkq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3luqxjuct.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kkldhpjg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbnndpgx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aybccdqr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iroydhsn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dybjuhei.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gaoyjdee.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wyaqgnoy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3myycybuj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3pokerqhi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mpyodzta.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vobglrat.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nhbbikax.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3yqojdmqb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sbdbujfa.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bdatirjz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gxszluay.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3llxijrzy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ikkgliau.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3upxqtrye.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3jjuyrprc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fkjaewfm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3arqyujfn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3yxwdhbeo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3pncdehpf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wjiditef.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3tjstyiij.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wqtfrzku.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bczltayv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3pcwtupkd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kwaovvoo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wpjzbjqk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3acyrpyha.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tosatrhx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3krgdvmbr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kfkvuqur.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3axoshzxg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3vklhzkai.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3fntlocae.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rigajidc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mfcgqcpi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bxrtsyfh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwutpxju.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3espkhjzb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3hresyrkp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3powmtohf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pyaklgxd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3psexyumz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3roodwvdk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dsxnabnv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcciboeb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdbvcrgy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3chafrvli.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pmgjxcim.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uzyzlnun.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3bkxkfszp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tiavfzvq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lvmrygqw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zrklftxn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnngpqrr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hbgtqcjh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3aqfiowqb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lqsgdsal.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ddlreuyr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jqjobypx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gonunrdm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ocbxecsr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wdsrqfhy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ezkjrlze.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kmosbasg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qyctqjci.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bkapuelx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fatncfze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfdunvvo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yrrkrwdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kimumyta.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3khqnftsl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jdhbggpv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3avkmjbwn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3byguugzo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3eacbdmiv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3eebexaoa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yiwflvng.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tacnfvba.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zchbijhy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tngxuqnm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fxedrzfj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qsyjaeus.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zzkixadx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zvxvrugg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3irwcjylf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rxulnhsg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ocqxhqzc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ytuxffiy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3khoiyonj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oolpuvwa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gilhxfwz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zuvhlqtj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ezoljmzp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bzaiwhjk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fdgqxawl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ndcqfykc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bkmecynb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xjnuukmu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3bfpuifmx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fgqtrrjf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3qiifwerj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hjoroees.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tqeeulmq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dytdmwkv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xhleztkg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3giyipjzs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gpmaxuij.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ivuacwki.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xexdsnbm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ykhkuour.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jenspbph.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3cqzpgkvu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cxmcpnqm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qtgfkhjk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xgspuvqi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xoifqxch.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ytfjjoqr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3edlprbdz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3oztqvrvj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vnmplzam.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3afukdcix.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zliixgko.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xusqsjop.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3sewhilfk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ocszojnz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wapqurlh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cefqugac.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dhfdeovg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nglloxjj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hdfiriyu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ttfrqgey.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jgcninzg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yflvwcmx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bdwowqek.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oodzdbfa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3glusavtz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3mypwkwbr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3leendqiz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vimpozjm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gtnyzveu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3svcxhbrv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3etscvzuk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wcwtsydf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mjrmoowq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3eiyxvfev.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ddxrqkay.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3athalafx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3voiadfsn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctizvytj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nphpubjc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jwpdsesq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tiwudqme.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jmelfaxs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fgunlfzi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zlycnblm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mvkuzrtk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3umbyyjsk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wxlirrqm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3vflctwnr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qiahtqna.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3poptqwga.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3kmagyodx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kyqjbxpf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wcbqdiej.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3swcuuqwd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zuywjoaa.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3mixoabrk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3isernniy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3etwdptic.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nmrhgxjh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3runllzjq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tlunsmob.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kxkjmieo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wxqdljnr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gaeqkmog.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dvhwyqka.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgokrllh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3comvyheg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kfzfnydk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qaiasdsy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cmlykqwy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uceenzww.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzwwzps.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gjqyjdbl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3cbltmhhe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3pcllzihe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mvmtqcxp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zwdgtakc.html


<!-- 参考信息 -->