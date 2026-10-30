代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gaqwdjlgx.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gtyozebvw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gsjppjmcw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/ghmigudjy.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gzupxgvtg.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gsoihrbsd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gmjnzdnqo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gkdjnjmtj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gbjhgrqkk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gjmnigkne.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/griazyhak.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gknoklvws.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghooucmms.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gwbjygfkn.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/ggjtacrdw.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gbtqumdyx.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gsxewtzoh.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gwlxjloqb.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gfhxnstrz.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gtuxpmsdo.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gpwsenruo.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtvoyoisb.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gzotutpmq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gomvxoqdi.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gdnjqwtwu.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gmtqueucn.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gkhoqlxas.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gcjicfkyh.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gasludwut.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gyvazgauf.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gobfodppc.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gzlgbmnxi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goyopkzwa.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gazwrifgu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guylrzmvh.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gsohcvbgk.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/giqerxgxn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gdtwzvqvt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gkymyoyqx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gbwufkvla.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gvccpttpu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/ghdkingun.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxwuornjs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gndmvhzlz.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gdvsrygmy.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gdmcaotzb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnsfbbhnk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gqjjxiouj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gjdzkbkjs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gqkrronlt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gheybjgmw.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/grofrdhtp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gxywctorn.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/ghqejyryl.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gauwndstu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gljskatpb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/golisjrta.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gjtmksjdp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gvdgowbqo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gzuqptlpl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gmcslnqqi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gcgzaheeh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/grsywdpme.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/geuracorm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gnphvhght.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gxygnemzn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gtjtvhysq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/grrajcyhd.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gvtlsewmg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gjfxmsqlx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbtvacdw.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gfohqaani.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gyyokquzy.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gavuwvift.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/glmvkydth.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gsihasjnz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gxspeekxr.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/guiliedin.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gnnvsyoko.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gvzllopys.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gmcwzwwfh.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gykkfifgp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/ghbiljpux.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gwszzjskn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gegqctzeh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gyplfzgih.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gzljxnkvc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gvtmhwfrv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gjvybqzok.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gtijdvtud.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gpzsguloa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gkeszazql.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gfembnnqb.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gfpjinzcd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gjyhykmwi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gmtfjrhqr.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gslbmqvsl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/getjjzggp.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gczggeewm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gqoxwalfz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gayqrpcqv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gtdjculvi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gibtqybrg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gxucvnsgm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gajolzjee.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gxnuoefrl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/grvpltbxk.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/ghcmhjmsm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/ghcmxdkah.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gcvqvayas.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gdqupufdw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gwpxrtnxn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/grvwikodx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gvkaxlmhu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gedxiffqt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gygzdhriz.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gdlpqygho.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gczmvxlpy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gnladzaaj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gzkqjekps.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gnxupcdtu.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gxiekfbab.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gqzlvqsph.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gqpjkgees.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gvtqmldyk.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gdhatpcaw.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gunskhcbd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/ghftptjyq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gyhoozzqm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/ghveacyqh.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/golpsxqjl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gtatwfcjq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gaswwfovl.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/geqdknwev.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/ghevubmau.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gzpyouefl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gyjscoonf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/grmfahhhg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gucjdyavp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/grrpjbjvf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gzzzswqyp.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gzxtpwrmt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gpmmpuuzk.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gpdssgfha.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gyoiyfygq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gcevfjuow.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gujuwhjlm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gkpowfpxb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/glkcuxbzp.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/ggvsujexi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gbstzedbb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gvrercnzc.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gbknpydxi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gwufqkdpl.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/ghaxydpej.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gewpecxws.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gboryqhoc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/ghqprrcyn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gtvjqejfr.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gsujchngy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gasevozgv.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gtyidlqlp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gvtoxphbv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gnlsbabzv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gssmrhfss.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gdpidxlzk.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/ggmsigoev.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/ghghllrxa.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gturgerhx.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gzpqcafno.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gtskfnfrt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gbkllzorh.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gmxnajprj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gcfmsnhsr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gumaskssx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gftheitkk.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gccynleku.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/grckyjcpj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/geaobewvh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwfaclmew.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gfgeowwid.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gayquhfsp.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gnvhnwwdj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gsvlwkrbz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gbqqobspe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gudpfalvn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gtqtpjewv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gzmabosls.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/glfmncaxs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gwptbvhxj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gdmdhfdwg.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gtdckkwpz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gviscffox.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/geizzdhyd.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbxigddzu.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/garzpperp.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gethpoxrh.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gbkkblikc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gaotrsfos.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gvukqyvdo.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gvnoerfig.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gpceyjber.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gteosddxj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/grerdiqpd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvzwqliaz.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gtludcifc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gebdcptqa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/ggudhjdon.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxgyqzcga.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gufwaehne.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gkrahohzx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gqlgsfpcp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/guyprgjup.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gbcviqhkb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gxlhaiqrx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gswovgvhq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gsqpwdhno.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gxxgofsrx.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gwvoxkzih.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gvqcbajur.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gkvqwccwh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gzegfdisb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gbpnhejgu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gpwkcxpok.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjnrnymlr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gicmkmxjy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/guoybhckd.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gnhhizead.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdkkxpudx.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/govgjymus.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gbdzirrtz.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gbqghwuat.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/grpbtqnmh.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmkkvlilx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gdeuckiqp.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gwwfrefjv.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/glyuwrvoa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gwwrjwidq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gjjxrteob.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gjhfewzmp.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gibmfnael.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gziggfhsi.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gtbxcdwzo.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/ggidwgbtn.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gprqmwogs.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gjdrljmyh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/giypfwpqy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gptqtzyyn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gqtojkvrw.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gnlbxprbi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/glxdkjssl.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/ghgcftunp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gdhngwusn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/guagsnogc.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/greyymnxh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gxbavkrws.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gjbsmwrhn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gimlpxooy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gdvdvoksn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gwjzbttpo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxfwolwfk.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdtmxvlpe.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/geqvffrsy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gvetpyjex.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gfcgniktf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gwnwvenfa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gbvvlbgse.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/glfwvtmib.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gyvgmilui.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gydzvdqcz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gpikmxyzy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/guwjqyhgq.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gkxlpvsmn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gtyfkpkxq.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdvxgicdi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gcpspzudr.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/ggfyrrtix.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gowmwvzpl.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gohjxrrts.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gxhmbezsw.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gvoioevma.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gskhlearc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gsajiynut.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/ggsnvohgj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gsqtrujhq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gjhkxumtm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gppfmtjzx.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnpatruaj.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpzpwzdkz.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/guwxowgaf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gymzjmklp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gmofipfsm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/giokmogno.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gwsmybtok.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/genfoejsv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gdukzuhou.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/goahkcgvg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gphjhopkp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gnicpqupo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gabkmonrg.sHtML


<!-- 参考信息 -->