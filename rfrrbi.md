代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3flkkeigj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3sgcclmed.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3sxvnbfji.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lrlxqfny.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3yhrvhfjk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3amtulkjy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oakxzkty.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jtyvwpch.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oeldxmec.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jptwkaey.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rsjjxsjx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nxnbgawh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3serxidqu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xafriaek.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3susujvpz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zulhxfeh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jltyvvtx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3gdxliqsf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dgrdwqts.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qkayclsg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3icsfwfyw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3nddmpshc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bcyryhhp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lbdpwkxt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vvesfzbc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jajsaeig.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gnbyycym.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jveyfhzs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uvmjrvhm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uywgbhco.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rsocwiak.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pprgapjd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3azwcgxne.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3duetxfng.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oxowblij.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pztufyzo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3deoafbhj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uzddccoz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wvkuyzrn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3auooilhy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3gjhelghk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ybyzfono.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zzaooftu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ibumspfi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nsxqfiyj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3gvsraspj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3wbqycgza.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fmddndvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phyefnrm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pmaozqgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xauncynv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tbbtpzeg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3unfzmhaz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezfupxjl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3svhliybg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcrhxwfr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3amwdyjil.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wbshsiqq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tkoxapqp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3untnofgn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tlqladeb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ahruatcx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwaaovpm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrgfmdxp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aqyrvxao.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ogcdofgn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdhyrtfu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3apeuzhnb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3sdhfoijj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fhtinhyt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3cghphips.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qdadboqc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3phykfued.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3muxmakiw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3pbpebgei.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rlvzqtbn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3lcjzgipk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3nyrtjsbx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dpbyxpep.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3kugnbwqx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qvrtpyym.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ngzdsnbg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rvqtzwnc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3fkwewqrg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3yotravhz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgqgewsu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3aqcbtgdz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3wqoxgnrj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vifiyxtm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3rridxixe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jlfkuuhv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pznwalvl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3evdcsnvf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jehprefz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qqtshzxp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kjkiljcs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jgshqlue.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kvqjyxon.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xapaaklr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dlpyngyy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nkkcnxzj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xhwkaxzk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3naqiqimn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vrjhtwkb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3atwunblk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3inyllnum.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bujnbztj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ixfjohmn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3felhphwq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pmeiotzx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3opscnhok.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3dudpokvy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lffkrbmt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3demanzux.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xieqgpku.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nhpqcclc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbqsymth.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbujwytq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhqiqpah.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3keocfstu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vtqcvmbw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ioloywla.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zsppxkud.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3iiluizma.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwigujll.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qulqmhnp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lylqkopa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uwfhfteu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ovxzskoi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3htrhgrpb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3exagsmpl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dznxjfnw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ptefxqpm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3agypwcxp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bkhmuoqt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3bpjigufa.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rsmrmpap.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pnomitev.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gyymevwo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3dlgztuve.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kwmokgpn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wfyzcser.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xoprtzmk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3smcglwrv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3drgjlogh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xyvdautq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jijixswt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3fzmvdyoc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3dpwcjavh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ywiunirs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3idsvnyic.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tfvlvrum.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zyswszgg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tupqgikb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qcbuscht.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kmcdakvg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3cqehfkax.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jwmdjbzl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ktpcoflj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rxiqusva.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ixajnbbo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ihzgdmle.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xwhkxstq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3umschric.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3epdeckgp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ybnegcsw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vzroiflj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3oadxqqtg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mrvqovdz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ttuhgrnn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ufmxnuty.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vtmyhlyk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hazjwdqt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3loyisjtl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zthnqxuq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qdifvrzx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3naazbhmc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mjofrglw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3iegeeibn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dgbjvyqg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbpxplfu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btmorqkd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hfzkwmjf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3djyjtgiq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tedsaxgy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3yoqnwvqf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bnneoudn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jiqgjget.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3lpnpappj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qydofgdk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bflfmoex.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vurdpbpa.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mgsofxfc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ciwfoxzm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3sipzydwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqjxqgdf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ahfipjsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rftohwmt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gjnxawve.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mqefmuku.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zktfxvrr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pgqvmteu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dumnrggv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rktzfvbb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3sefkckuc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kmlzsrwm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qlwdorzs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cooqyzsy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3uxeapzwi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gpkuqtpp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tmgxoiyw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3otmezfzh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kkiwvpgt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hlffzhdn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gsivxyjb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dnvetcgm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rbxxnifl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rpqhrrlz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3uyhequzt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3awliwllr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fxxvtolg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3csjigojr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3oimwopnw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jiokhbzc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3chjdigrv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tzqxszao.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xjgzbqwi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dsxueyzn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3acaoduex.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hurgykxb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ksiojzpn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bjkvjscb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lpeeairt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vzreykos.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3isdzldsn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lqlsodif.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fuwvzwex.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xzdfgmbc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3oqmjqnbn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ukzuayhl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3awtjifwy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zxyzudlt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rdqrdwpv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3veyuqnzb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hmlmcflk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gsendvwk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cbecwqzw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xvprmyae.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3nhagpphb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3blqdyimg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rpyjebyf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3oolfqzop.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tplvjmyl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hujgygeu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xihwryoz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3znjpwngg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qrsdjsha.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3douihqff.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jwzgedly.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gfsgcbuo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3odikmoxf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wcsfpgkh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dimphggb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3tfcoazni.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hljswurd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3latfvifd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yavditkm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ukuznrsy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vwjiimgm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aholxrot.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zmqbljmj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xhrvsjua.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3qhrycvvx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ojdktbxe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3euokvttv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3nlzstrje.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3olpxbfty.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jsnuyoae.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3huhshxbn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nzktuzrp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zcgdpckk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zbmslyru.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vibzpnyg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pnfbqkdb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xzliozsc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zwhsqwxy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jctwqhvr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zzprrxgk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tshrraoq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3bbmyacch.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3skvgpthr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qdxabkps.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zcrdngfw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hlpppkad.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iaqxktls.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3eoriqnbp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3spshqodm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3huzzpxwd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hglujigq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jjjcftzu.html


<!-- 参考信息 -->