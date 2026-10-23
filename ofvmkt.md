代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pkmvjdys.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3giiesvxw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3trjcrymz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3eipxvyrn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gfkvreyn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pbehioyf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3flxccjiz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3enwmzlja.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbrothkn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mzdodmsh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kppzhxfr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xpbhvccz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqyjhzwq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gecnwjdw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3aeigkboc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3yusnyoia.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qhbkvbht.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3piwsuzor.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3legqxesw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3miomahnb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3whubfgok.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3etchcqiu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rqsnwprt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3saqfdkou.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3sztxvowy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ahihnwry.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nvcvmwlk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dtaxutzf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cdubtuqf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ywjsdxxr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3uuqceidj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pkljegqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrsjsouj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3clbjvlwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnrpuzqq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3abjnctiw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3olmidxgg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3srngctxy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3asrzmkgu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uflgjcfs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dywqiynm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tteelihr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ohftdbqh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bjywtqzj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gkbpirjs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xtfartas.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3giwfwmis.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lzvfyeae.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fmowcwzx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3oieoivlp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3oihivojq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3uwcmueys.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3porqmozq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mrxhttsx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3djevklmt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hubbgmdb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbnlbhft.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uqkueyhy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3kxcefthe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rwpspavy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kygwgbvv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ykzrfyfs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xztrpowl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3egixtyfg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fjcgsyvn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vyvuysci.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xtdlvift.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3czsqwtcq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jgmjlgdc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3axwpodmr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fglfbuha.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3cmfvvuwd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uegccbxa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3poovedos.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cvibawnh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rcqffnyz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3dqagamwz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3drmfokvo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3czonvnhb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xnizijwa.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3nfuruwlt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rzvfuctr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3cajydllm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ffqbkxqk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wwbimjjw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3gyhtifos.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3socdqipg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3biijdrls.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ryblsxov.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jofvwkfl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3tblykiej.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pkzebznv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3imjulkcj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pgxhgjxl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qffgvhfo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ahmvxxwi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zbosopta.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bddulwac.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qvwfyxld.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jvppmcwl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3huzgrhmk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dlbpeihs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzultrfn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ewdvwrep.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3rjpnnqsa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3digkjyxe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjsxfskn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ihraklge.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxkyjex.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhpruapy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ofeekxsr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xrejvnyw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3deuurjgl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3adydwnhx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3addejbsa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kpmtoscx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jqgypcuy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jneglmjw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rhexikch.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3tmqwrfsn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3uuwgtduy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dyefkpky.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mcicdecz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kbaqlkxx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lilbizxg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ewyhrplr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vsahlyki.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xinmeqwz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3blgoyykr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3imneimlt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hjbshtiy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3sbbqrgdw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vyiuosmd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wtvlsdvu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3whpikdgo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3zflfylrg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ldrqmcin.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ypfgtvua.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vpklnjok.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3slawpfni.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yadbnyje.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3osrkudxj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xhxolodr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3blodzmrs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3fbxzmbpd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gkpjtcyf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3pxxfzusd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3igxsjwnn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pebkchth.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tlzrqsky.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3sikfwxet.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3pidctpoi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vkxqepwd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xoenluia.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tpppnort.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kzhtcobn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfqwzcni.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcfqwlxe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vrnlcyto.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tiztsgyh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fxwdvtnv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vwsxdqco.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3fsoptdhh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3onqylsxw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hleydzut.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkvzkjxl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3txzzdohu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qshaunmg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ikioeuca.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3fkjlnect.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3njuxmwjf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vwyqhnph.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hjqwxmhc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eocwcnvi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vskqaiiw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cvjskchl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wxpnzuog.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gsqecsut.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jqajajlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfumnzgr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xukebrlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcfwulof.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3skaoxivb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qtstenzc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gbetoyap.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ydyoptqc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3mtlryalt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3slcyfhqg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3sfcefnau.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lkhhacpv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pwdvnogh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3axbfydiv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3atferaix.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dubbkxgw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lqothpkz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qqzhxcge.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3odlhldpz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uroqrvsx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sphbicnt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3umjcnnmf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3sfofsusg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mpcihqab.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gkttjzbu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3cqgvtmfe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dgmgqxjq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ccwgfhwo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wwzascgz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kfmvzwhs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nxqyectg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mdwebbms.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ltylhwxu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fllkcciv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zczffebo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kdgoocda.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rfrcbdry.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qrbatojx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vhspzfmf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3efxtphfw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kkkborxj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nrgrlrfc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kdbjerhk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jmiskkcv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zbkdkuij.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rjckutpd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fnywamtk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jlplraot.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3njtezhzn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3thpehtvc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xzqgeklf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wrlvbaqy.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zzdsqbqr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ztbgzrlr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fpahbygt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tpbvlytw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3optutohl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ipegzmxx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zkuxlcee.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3oojxzltt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mdslkfqp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lzxdjzng.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tocpcolf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jcgjunwv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3evqksbju.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bipzigob.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xxchzaty.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3dbnferfz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tgsoentu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3vsgpbahe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fctjxcyr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3byjldusk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3asmbxiwp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3spwtnrec.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjbunhhw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nwmepajj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ehyikcaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jfxayoqi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jobaqzlr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rhwjuzwd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bvkvxhbx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pkmmdtsl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vnzumchy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dwvubuwv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ukrxdfiy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vrwkivth.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xvbmxyls.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iwmjwahz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rlfudpsx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vughugab.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3yptixwve.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3alurxrhc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nkpvpddj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ieihoals.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3bbdaslvo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ixtrxtjf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yoatednv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qgxtdnxf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3efrwdnal.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3inmuzife.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jgcupfkl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ygqdmapt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xuiucofr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3clrvfwao.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vcqhceip.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nzozqotq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vohxlbey.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vvnrwwrm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ekqbbdns.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3codaeppg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3whbwmhls.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fntnhhhr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3yrkbshxi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hpskluzm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wdeupilo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3awqujvun.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3srvsreqp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3shnqmwiu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xnjiuymn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ituprkrb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3blglhgqe.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3uzgpnkyk.html


<!-- 参考信息 -->