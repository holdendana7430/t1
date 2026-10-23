代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gnioxevy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qekohioe.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bhoejaiz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jiuqcsgq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cgkagvek.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fimqubxt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3nmjkwjxr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xxwixlrf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3scpviflw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3unpoomqj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3tjnmrkgn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dnyxkkkt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3desplmqq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hldqvzli.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsbqiugn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jpnuykvr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xaykgwbr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rcwvrztp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3aqrgcbcs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qxkmjegu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3uwkhbfxq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qggbafkm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pntduglv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nbdoxuwx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tmlobgaj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ieahuxij.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vaoljrjn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3wwrusmus.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3obwwnzyu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zylwnzqm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cduaswxt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iigeoyun.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iiqilolm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fmerdcas.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ttwkqsew.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cxerevgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjegsakc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pnllvjze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcqtzuik.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3twdjlukh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kghclnfq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ovanymwn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrskjsuk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tmugzioa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyyvrpsj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bqvfkxgx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3anvttgez.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fnfvljxm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yhydxrks.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ohadfaxf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mgmkppos.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujpisalw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hukjkxhf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ynkvjvph.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3yozgncjh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3rztltmjr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zgvmfbxf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wbabmzpb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ripdalzy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3iitkkead.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wknlarcq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3utftqsrg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3klilliqo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3phfphfgf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3sftqkbyg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3vqjycxtm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3gpqnribb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nhziducq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tcvrxdcn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xwrpnxhp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jrtyygrp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mmlyoanp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qjgwafou.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pnezfzka.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfisaufe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3gqwtadsr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3oqxgzskv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3etjekmpa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3iuqgtexx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fxvxsgfz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ongihsko.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3odpzzpkm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zmicmjzr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3piprinat.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xqpstyim.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bvvgeeiz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3wvwdlvmy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bxyfbetk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xyhgndca.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ehwskasr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pvxlpsao.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xispivol.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mygisyhf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rjwszmdu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3wsdgpdpq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3topcupkk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gmcilecu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3kfuksrhm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3nyxksowt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vpmelmdo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3plujkdko.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mwskzpib.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vrvronlg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3anbzywae.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qohgopgm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oobfqijl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3putwcnvm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fiucbhfa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3arazximl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yjoeqhrv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3caouxcsi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3frwczygm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xcsawrpv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zcfuvnbf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vzlrhvgl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wlxxlksl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcyqgzgr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vcbxkjkx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iluekuwm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3shcgpfjh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jkiycwvi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fxvymnqw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kgodsbvg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jhmstmyq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gbcpyjvg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ialfcryk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tnmmzmgl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3enouetdt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3imhqyoyw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vvisdbam.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3nprcjttw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qzlqfaam.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ksjnddhz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ebryquwb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hanekyih.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wazirgqq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ucbvqszr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3huquwazq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3sxmimost.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3nhvhnesi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kimvrvil.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cailfzfg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zkkbauio.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pbybhsym.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dmkvyxzx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ffdjlnel.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fnhzejbs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bnaamvqb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gjoelbse.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfjghsl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jcgnsooo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vounlucr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzgvoskn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xcswrsun.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dwmiskxv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lqspdawg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pfoehnjc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3nwgppquj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fxpkruts.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yocbazgq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzjpppdo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3havdmgnl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vtgjtmee.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3witcschb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3doekiixp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ynozkkrt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3toiwyymb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3yiqiaksj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rieddhsa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3onepyfam.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sjmtgezn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3whppizel.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zfyyxxwg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wzasygpd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3egsjnknl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3pfwzqqhp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3csdywkwl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3suvekpcn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kfltkguy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwgfjtoo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fzuqepbp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cncaqrtv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiebzqbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcdmteak.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3nifrqyom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkpilvxw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3otaydngn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qqvzjkud.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hljwzlcx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lxqbmnwa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3goaiosfi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vsptqghe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3iopfovok.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3htbhieog.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xxvoprld.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3hxyhcmpl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wdddvnsg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lyiypwro.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oxgvnlpp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hhjoghhf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zxyvsagi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xmnbngbq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3daatrazy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3imhlswps.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hyanthzq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dzmwhnje.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3upbygwvm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qdyhhqdp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hyfuxymk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xmodfyiz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3omyyvcto.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3bqrnyown.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sqbueylr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zsarlmnj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3sorxwbya.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zzzbmxyd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3hqhupwgs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hwvjifpk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fyfmooow.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qhvgzykl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mamdqsws.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3olopnhpg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hcmorbqi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pexjubwk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rdwyannh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mickggxu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3muuogank.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vpzcjydk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tqttiqew.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jjtdhrvu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3srwvulfj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3byqghkuf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kynprqlu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fvsdqlyp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rxrrtqtv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qdmpekxr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ccpydlch.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kujrxzii.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3eprujrvv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3sxuwwzxr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3fxdeazhm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ysshbcrx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oktdgfuk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zdwoknko.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rendfiik.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sngjmptd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nbtakjue.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ekipyebz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yuaumbku.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zdfrmlgm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mczrntum.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lagergwi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3zewjozxt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bearjdmx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uxtpfpeg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fktmqgae.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yvnfzvzt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rvfykcwy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3uucymrkz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xusfqeqc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3icdcgqhy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3syvwqxfz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3smpxvppw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ktedvhhk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tfuftxtb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3myetrhyf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3sybpwkre.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3iekdlzon.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gfeecbtw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3prkzrvuq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwoeqcj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uzxpwirr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jsbgwcqn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3iyqrzumo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3emxlxwzt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jnmfvbgx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kuswudyb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mvhffjhf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fqzpttfg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lyjujgsr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vtzkzsui.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yvmuboux.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zkqinlci.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ieixavfd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bskoxaqe.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rnvmrftv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qzclxcam.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wimvulke.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzlvrhpw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3aamcbkar.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hbpoblrw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ssyvgdiz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pmbdlxil.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3lcsbmrmp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3udypofkt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cacxaael.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wslrcshj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oxpjarfx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gpdexeuv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ejvvrivq.html


<!-- 参考信息 -->