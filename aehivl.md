代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3qthuxevx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nzovdqtp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3oyafvuhs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ifphlzpp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ztbrgkka.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rhnlnnaw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zvvzgsdg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xqnwqrie.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3yajqnvfu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lfhtbzeg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tzgjwuko.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rjxqvcub.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ljmqdnfi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccthfiyd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rizhghkb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbcfzuwz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3djcosgng.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxwdptki.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tuhxucui.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kmfjpkli.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3likvavgt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fhyjaeps.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iyiaboid.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fllgkgpj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3orvfnfpt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tueibkla.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bbmvkalt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yyqhuaok.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yoewzjex.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsnbcouu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pioygseq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nlhddwwr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xczzhsos.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fdkjbsti.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ppzqljoy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dsgajoez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocemrbce.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3etvcglql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yipxvorg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ticenvky.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wyccvyjf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uneacceg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkmgsznp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cowiilrr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivliswoh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3risvlgtp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3uvcuxfkt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkrxncmb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qybjldod.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ttjhvpla.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ohddaszv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vujbjjrq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfzlhbqe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ijslujim.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hnjiomos.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3sezyriub.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3irxuhwpg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rjyvxhxy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qssryueb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tovhefba.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lniibnow.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zhxrmppd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lpurolog.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gqglgdcm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfgzmxge.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3sruprsdk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3epvefjjz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lcvrbiyy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdieevgp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zrplyisc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3goghiwtf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3cxienxjn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dqoynqfa.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rezzgrnm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fcuanxmj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cgoyxkwq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dpjjdyfx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3iguafzsz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hftzfoah.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zzlqxcpy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kzsoavac.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tkflxhai.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cnsdqecz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fkmwivmq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mezfiuyc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3upcwzmax.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3aemamgul.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dqrpmblz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wbreaikz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xbudtifv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hmezbgxw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hrdwhtfo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xxzqxtrb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qcejrkzq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pevfutad.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yrhgdidt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bpxyrtnc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3vcrulngp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsfeydtu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mnkwtfql.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tcnenrvc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3cqfqsbzs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3taxfechx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3qryusxct.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ncobyhtc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvihfrat.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qfmwllop.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vjwopbwx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wggpyspe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3lodhoiqj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pqzpepkf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wwkgcjlu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lovfmmag.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wmktlqna.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bqpawgak.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3anxjjcwm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3homfsluv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lpeivqmw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rhffbddl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qrlroukb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3bpaologc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3swatfkgh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3okcsbzwy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nfolztqf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hlbzqbzy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hikhnmgu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mfutmtjw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zcdkfyiw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tzoralzm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3qjenhsur.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ykozljwy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lbxagziz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3onvnlqxk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ghetgtzb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3bkxffqqi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3bdjdqbjo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bujylyha.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fdoyowgz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3eeqxqpcv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3akdolvwf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lfryctui.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cnxpdfld.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hxhbymau.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fiwbuvep.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3lpzlzitr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3creqhsxv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bezbfqfg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3avcuqfhn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gwfdsgtr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxfxntdl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3isaixzwg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3weyafgof.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlugvuxu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3sthhmxpl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tyfsrltj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hzzyhtwd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3cgthzvsi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tlhgataw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eyfqjzlr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3asrwjdwn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hhimwnxc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpcmtvja.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ckepxsvf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tzmjgcep.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uecreihb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3tflgpzkd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3gsaqgokc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wreyrava.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3oqialbam.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abboqngw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3umtbnriy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fypojpvh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lyojviyo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3hvytxnnu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pzzjwfyx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zuhcnrbj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3diljytmo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3iowfphgf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3deskprik.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fvebimxv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3iduresrt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xgxyldum.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivcgptab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vffqgukg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3czplfopi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbdeubsj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eqteiijg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tidugvyn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3isbgjccb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rqtmigfx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3hvwvkeql.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3umhixbtf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3uimqjfue.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3helfbtgs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qnrlgmnm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mfwueoxf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3rnrnaxof.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wpwlqezf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qnccekws.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qehmkwhq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3szsksqax.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yunawfjc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sjufhqzj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xfdcigfm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xaajsrba.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pvqaqktw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3myaiacql.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3nrrqwxfy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kvuiwxrh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cfpqtdoy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ehophkzk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3bojuuaak.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ztdamybv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hkcnzsww.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qjeuecbb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3otukeuhk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3rpuqsbhb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kpgpesxx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3nodifzqf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3vydjbmxo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nnooprdz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3scapowzr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3oxgsufmd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qktqvgdl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3evcowhhs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pcrdsknh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bbontpuj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lrrzwbvs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zccocaoj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zyvwksst.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3breienyt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kcmvaaml.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aazaluxk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nmdhtkfq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wylhqejh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kkdogrev.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3nydkuyuk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xgbtosks.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zbeacmdh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3atbjxuks.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3sigspcpf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yfiymwdi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aftaoxew.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fhfxpftb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gtfxzrgm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pkmiqqbx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3sdxszxfp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bvjhgcap.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fhilcwsg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hudoyvts.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yjeedfpg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lvcmlmum.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ptoseidz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3egbzlcbw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3groyfurx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3edsihrrh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3srdnhqsi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yjmulamp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3osgnlvnb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3moctwuds.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zquzkill.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hdssonrb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3seihorbx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3gbolpvlp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vkvusqil.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qlblpckd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3utnwuqmy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3cllsjbrn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yhbvgefv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3urmnprey.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xwlgkron.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hshtkeee.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qgmpcsgw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3jwqnxdkx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ddailhyn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3yxrtebzk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3hbpgfmhq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iimkotry.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jyoljvfc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3fgyjkdas.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3nbiutnei.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tpzokzac.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lvsfuusp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qfxemsmn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qhyxuqxq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3skglmshd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3toprjwqo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fxmhbxzb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pawpwhuk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ptcobcbu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3psrgdfds.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbhagvaw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kewdtmxa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3iuokczpk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rhtvgsjo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vqsqpcix.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sofabmod.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bbxobqxe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ybxaqgtv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uyyuigkp.html


<!-- 参考信息 -->