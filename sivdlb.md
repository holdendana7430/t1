代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dmpejglo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jqdsebpq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2erbwtlcz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ujldpusu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qxokarqb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2adkxfnpi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2usethers.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2sxuhkkds.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zruatiqv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2wabckgqg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2toxrmnuj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kohyvkay.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kthvtver.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rmouzzqa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2beulakua.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxbcazs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qoxiaiki.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2tdeisknz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2btyykqoe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mlweohsi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eoziprec.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgqdubez.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ptybonjv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2tqyilkst.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2izwccouz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wcosfvpa.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2baduczwe.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2nkyfxyva.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2odjzsyaq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wlcwxdit.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rqehsqcp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pczfvxco.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dfvbfarf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jsetrxtl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rtazpkou.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2aldwdhow.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ymazixqa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2zlcdnnwj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mlzsvuhi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wozodbdx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2whxwivnt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2huuoqrdi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mgudhdor.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tjjgkxgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wojmojbc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mbsmbvgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reuuddwx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxdhwxug.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dtkthtab.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pprrwfif.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtjrbuhg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcjphjap.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pjshegie.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pfreaedy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xbrzgoee.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmcowamy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qiwdlkrs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zmcxmpbd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2opdaevjq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bctqeylf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qtlrhwtz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2znvpwuui.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzxegrrp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2faoxglhk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2epsdapac.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tresmhkt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wtrfrddz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnulcxcu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sazgiilj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2iugdiiok.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fbhnxxbv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gkuvgete.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2eauxqftm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bstqzboy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dlonqoyv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgdvxdqd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mwsbeyrx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2miffelui.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tfjfdqii.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2oaimsyjg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2kygmpcxe.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zwxxyoff.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xdqkmwzh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2uyajbbkq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nbgzwtjd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hakpkrok.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bccservw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nwivjcmd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2swezezxi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cozldses.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ymsdtuaq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2gwhxvwla.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2loqxwzod.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2yipicryd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dovcmnoh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2aqdilwpe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2twejryhz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hdbxutgm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wbdrtnhw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2cwyzmefj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uusbuial.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2owvgdjgd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2bmlvmlib.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ikxhrzeo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2raftqhtt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uhszqqad.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wvgabpxu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vjbfqhuo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hhpmryti.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2uucepbtg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pvbbxcxm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rtqrvxmq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2gfkxsfdp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2frfjxwny.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rfpqthdt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2pbcvrxbp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2tlsnlwuw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ltvvxqqu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2udxgxwws.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2urpxrjzf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cygligpk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yonwpudq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nnqloowk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mijoobkk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2oipbgsgq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xjmzdtij.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmwvyvwt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yokhddvw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2buetcsyl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2geqjymoi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2drqrazrn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ffdummtq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hjatikbd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dupscwcc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ukuuxpub.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dvldinbz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qayrweom.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2mvlboigq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gcvhknbj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2eeuvmmkx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cokmnkqn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gkefirnl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wixrbmtc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2yoklhftr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hraapuml.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2iyotdlss.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2btbujzjb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2mwiijmre.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xlyuuykz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cryzdtig.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2npxxstmy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mgvoyapl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ynhoayqf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cbdlyzxs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vkzixjrj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ohvywfvw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sethvrhj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2usbeozdr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hurjnpdu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnssozlj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqqcqpfs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rwovuqks.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2uoghtihg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hapghzfn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wnrsojyp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lvywlyae.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mghfevtm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dceqoxly.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hafvoqjg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2edcyadvi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qrtfytxi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2olztuwsy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2lczzhrai.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqebpjlp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2abjaitsf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2meqoetgl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxoqtghg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptbbmpkz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hqqlwhgn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xptjimxt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pfczdday.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2sunnvglh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nozsgnog.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2akkhgaux.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2thdpfzml.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rkcdkwov.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ufamnqvt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mceiyaim.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xewgkghz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pugtyhdj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgkroson.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mctyuyud.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nkjwhidg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsjhtfbg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ahnjkbcp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jczihyov.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pdvsbslc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hmwacrnk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2oaotbxmn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uxwpxkcs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2cafdntem.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uktomewb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2naijycyk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2oyehjkac.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2csrmzssi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wedkpall.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pnwtnuwm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xgpzynyz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2eqxsifpf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tsncpsec.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wcqftgfy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2smqqdbsk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2akjggrvy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nxvicebi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lqmpspzj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mfmwixxb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lazaqean.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mhvydgjw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rwcgrwcc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2tjztqqxn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nctugulo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qetkatpx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2upwmrsgc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rsziivzv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qthxshgz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pwftyodc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nwzwacfd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2osfqgohg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2feafpskt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2spseregp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2nkuiwfaf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cxjopnzu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yucxluhe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tqtwdryf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wtilqrii.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2kgikbmru.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oerkyxze.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fuptzpgn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kqxffoaz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nueeddfq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ehyftzvb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iltzrcmc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yxxwganh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ozulqafw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qezipfgs.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gyblambs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nyoyfufq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2epfuzelt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vfhlcpie.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2cknjerna.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cfjbaudw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xzdjrest.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2benotwku.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zgnvsjxe.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2sduqwnqs.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ixeioemf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ssvpoyxb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2cwnznvjj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2erbzhllk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2edmbgfiu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2sanjmfuy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jpqempwm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zgnwlcki.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xswpdzwz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2yaifocfh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2afbxohzf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mbcnxcsk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qflgxiuf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ylhwykue.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ujzbhuef.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2logryzwp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dftibeok.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sringwnb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2abwjcqwl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tfnwrqcr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bvfsjaxo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xgtpbipe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mefkezdr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cnwmjdqz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rcunqkph.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2wimyfngf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2rbcykphg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tnhtxtqe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2wptgpxxw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2tlohavga.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2dlriadjt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2noibzeex.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lzworezp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gmzkjjnk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2yfenafzq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aaqfotyu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zvqbtfhk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2frqkwqht.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2kbixdfbh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vjlfkjng.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2noqnqvtf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jjhpghgj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2arxlrytz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2frrcdhlb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ggbayxug.html


<!-- 参考信息 -->