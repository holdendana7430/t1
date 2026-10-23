代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aektdgio.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3noirxehf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fnnquqbv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3yddpohxm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xoroakqi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3rmmkzhem.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dyivsnos.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zoyjkltc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pqxrvrkm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gvnwyciz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lpbmigsp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vnfmodgg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3edanmhfh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ueycnvlk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dufjmxul.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3sjptgang.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hypsmowm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sbqsqwem.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjjikjkd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3runbvxaw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bzrhrtxo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yifzlvry.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3yhomnkxo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qtppflxl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3osiorexl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3btvvwuic.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yiufkfek.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vnnljmek.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yluudflx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yoqdvpam.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bsvcutzo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qqlcaswa.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3etrhelvp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdowpvvy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nkjbnvzi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3huukcujf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mifbjuyi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ylukgfrp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qnhlbhbi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3topkceas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plpeafqv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jzxuocww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zoxwzljz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3htphfhkw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3igvivdfa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gvuirijk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgdwadvn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xshmiwds.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3abxabdxg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pvinafzz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hecsnujq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xnhhcneh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rwglijot.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3njddhjdq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zxnifotd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ubugpcwu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiwoposg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3oxrwcumw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kpbnurvd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3cgkqyxvj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3alndzrnt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ntyyhzqs.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3idvwfjdw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ohcojhls.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sdcdwhou.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tstdplpc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kowajmso.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rrphabdz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3huwcytxo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3njnjyiun.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3barjzlto.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mfkzivkv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3aoookdwx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yywijpdr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tfidonkw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3tioljfes.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3cexmbzht.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cdszduqw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gvjvgkbr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ilegmauw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wqkmhdpj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bjaqwsld.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ftrldwgf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3idhjbaac.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3iteulpaj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qtrqpslf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3wjqrtxdz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3qroeyikv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3iakhtlbw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rakdxxqc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3slojdqxi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xvmesqtq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xmaurnue.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3cqhstnrp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jqrkdqal.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ujbkslmh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rtspcxze.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kfnusdsn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ixnodovf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jrmthqbr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3usalnclh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ywvttvif.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3paoahlrj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3kdxofrtd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ycvsuqmx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3yovrcxqz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jzwdvuhy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gagzhnrz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qglyjnap.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jpbztyiq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvitjvfq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jomwaeft.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dpgwrpeu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xgemvyxq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3otjhrmfi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3lxteqxqf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cwzfgmxu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmzzqlbu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kdpyxtua.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jiumjnfp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozxyfgeo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hwzzpuhu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3trxryokc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3lhstabqv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aiwldtds.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3bejicyhd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tqbrsbxw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iozjgxqa.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vztobqkt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qdcvmkdc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3swvzhbsj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ahthwxcz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ynqrczul.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zhjzblrz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vlrwrdbd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3effpottd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gqflglkv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mwjjenev.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fljqtahj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3duylwexf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3gkuyfypy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xsokuwwr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tyejzdmp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ylaplvbc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jkswxufq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yhxgoefk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3itftloov.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3yqmaxlou.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xdahycbs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ilvdgwyx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kcdmscff.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hmqguyne.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mmokfplj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxwslzpq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lwbrzczl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyerlqpr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eopxqopj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nrjywpaj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3eouywril.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3szcatskq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ujwrqsap.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kqxhqjri.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ndxmunxh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iapixlia.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tibwxppq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwkpnweb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ufflwfnd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nupsioxn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3whxxhrpg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3aymueppt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3baydlluq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xznnolfw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufcvaaie.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgvvmrgt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3grheuuzc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qkalhsca.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3luyrvfqr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zwtrmvrb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xrquilnj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ducpwcxf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3oalupktz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3cmmchygf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ylangkog.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rmyxxvyr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qcgpmqpd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3shvpnhiy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dinzqeml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hswtmueh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jctbyrrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbgwwocb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gljxnpoi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lzxkoquy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3odvdabxa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jdtdgfjc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3acpgaidw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3yrcbsysa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fbeuagjg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cazwnghr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3powsmeyd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3tqsjzepy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rfsstsme.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fxyfeufy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uyahnffl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gsexsckw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rhjfapjk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rryhbikk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3oocabxku.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3snhyukpd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3zzrokiqy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tnvlrhty.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hudricyt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3izmjyjic.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pszrxqqx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wakajruq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3turnymsh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yjmeegei.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mmfrctin.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gbznuxty.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqmkymi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3odxrymvs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3dyhfchdi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hkbkqefs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3scdbgdlp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3soiqlvix.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3merfvrko.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3abbbuvsa.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3oxfwsdrj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tshxuytj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mhpflgff.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kpgyfdjs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pxsfapnq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rkpcxlvj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mjjoyjdi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cuwrwsef.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nwlwyqqv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bhicwtcd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kahibodr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kvyqtidy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vnknocqt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wakgetje.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3igpnhfow.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sxjljgiw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xjfxpvbh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3lkmbcpow.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tkufoyiz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3knbyhrnb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nckewvtm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dxrmldux.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ynciwojs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xjauxogy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3dptesixd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3grbstqyn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aoviryty.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qfzbwfti.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vcxlfjwy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3aqodkfvo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tnvfixah.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xdlffqbp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wcsxwjla.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ajjurold.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jxbutjlm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fwiwbsgg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3oozuikrn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dggpkunf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ivgnxgjn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zygflrdd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3dustaqpw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3okwbdldw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fgzbkhrt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3azoutzeh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3spboyykp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vsnwzvmj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ourcelyw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lkqpfpnw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nbgwxmes.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dxoyklnx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rererpkm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lipvrkws.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3uvondpch.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3oorbyecd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3njeezwvg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3taxssqiu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3pvzunqvd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3cpkrxpfm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rlmpuwyy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ueqltajg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3youqllaq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fcpapmqa.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wenxkjrn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kejvpuks.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vwddlolj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sqkrfhru.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qvcfuylu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nopewmlz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qwapptrb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybplaauf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bpxjhhyp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rhcnjlqx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3aeucmvns.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yjjgvxrs.html


<!-- 参考信息 -->