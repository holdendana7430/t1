代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dpzyapsc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3igelsmgb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tolpivwu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndwpttqz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3acweqslp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vshkbiky.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3riwseqsw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3aospfgkq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zxcszeat.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rjqljfwv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lzbuxrlq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mrutzswu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vftbwfee.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ijvjeifu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rnsbqqfp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wziclftd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3lmkguqfn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3okzcuujs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wyjxnpqt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mkxpclkr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gvfrshxc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3agsiauvi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gbtyxzrk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ntarwayr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srgtprxm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hrarowkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qswblupl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ykqqzmpi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3utombjha.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhpcwmpy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dzvarnpu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3awclpteu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvcdlanq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yfsrlijj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rttsvmuh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ognvrvnu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cfergmka.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xqpqwdgt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yammkgxy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jodlvdyh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jmlxxkhr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zaqcnmpx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vpshgmhd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xpwyzkyc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cuzfxvzv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3omzuuwbc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dqpwsofd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3vnsjddni.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wucjomlt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3aylzvaog.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvzqoyqs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pdlkkgzd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3qpaohllu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tjfgcpqe.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewhevzjm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3bobebuxa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nadnovzb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvlfoawg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ooougtyv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3adcfnozx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3adbmekdf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ogqybvuz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iywpuxqk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3cjnaerra.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kivvftgj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bysprfur.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aejkblae.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mgnowiuf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3sgebbqdg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yahvhzqj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uunuimbq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kgwrbshy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jpqgwdtk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bqpobfsd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vugwlpaq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3trlmxcbf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jcgodued.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lvgpdzhp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3aoeeihjj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lwywyiyr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cxghcfnt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3cdnfpmsq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pkgrxoqf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjzbfqvb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ttmtygea.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3csvcibhy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ulcqbody.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rfyyobiq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3koehruuh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3othdmmvs.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gdevlddi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ajqgbvez.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3aycufwzx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3czhxnppc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpatjdwb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3reidfizf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3iellvzpr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qshtgfqm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zxnmppec.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3euiyijxn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mgwocssy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vsrmikrr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vroqkndq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fyuzmotu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3klwffnrm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3plhqwrxc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncqwtmcx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3fhqycthp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xjgjpwgb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3sztrdgfc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nscurcfy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3upgypvxk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3muhmfgys.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uauukjmd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ncurbayp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mkbwzper.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jhtbouwx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vtxrpvce.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lmzkvahs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nxaaisqv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rvtgbgyw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hdodejnu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3vemlredy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kwndgxdg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jmjqtind.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3cvzhmmwe.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ctqlizrj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3spdtnwkg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uqwuzppi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lrmumwwc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yxszmfyl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rznkgwlp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fcxulfos.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3nvtmclpu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ucqfpjky.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3osxsmhtk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hacjrhln.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bymtuqns.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3waoctmnl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vaislgcx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hsyxhtjp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nigxshyn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jlahihik.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vfdchdoh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uugbmxdt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ttgkzaec.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sinzyrcs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hipkbcag.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qttryqyx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3abxmmnsf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jbyeemzj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rkqnaizw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ejvmamxi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3efvsftou.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cgjdjojx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zcpqlssn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3htlkjsmt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zlaqtsss.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xauwzcpv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3joolapux.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ojyffueu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hjqqlxcz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3iafzakih.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xautwbta.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dmionifv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3phgbrdmn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rwlnvxms.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yhmqaely.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3dlzutkgf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gydcweyt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qkzcagjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wldngris.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3flqhlhnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npkukwjg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3phawnlsv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3wiyxjlry.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3afvjwpea.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pxmpvadt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xvyidemz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lpmqohhc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ndnrrifh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lgcfqbab.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dbjndcdi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3botjktfn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ovrldlha.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wsnlrybe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ixacnedl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ifqlzhyh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rvavnwri.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jthdpghu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3bdjwvimv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pmkxshdj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3horaxrof.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iptofczj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3btvitnns.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3usoalhxl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tavxqcis.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vzdssdae.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ascfvazb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vwbvcqta.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kkqlunth.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xlgfxndh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hneojyqz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hkigwznp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3dhiptcpn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zlgbzdkh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hxgcldwu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3hxoyzqdk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qrtquxiv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3byojvixs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vvhhnmvl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3euzinxxh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rydvticp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hvemfagy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3aljzpxic.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3grvogwxd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3psnsukrd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zzvosnls.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fhhaestm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3abbcphfj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zkuadoly.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nzwoimdv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ntnndbkm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3epidjujx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vfzhvjix.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ygbtlnpq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3odlrbvss.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wekzunnu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3quacerxk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3iepncegl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3umbfdtpm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3styfdbcu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qvdinjwk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dqbabbnm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rsduwopj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uhvjpdpz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3elyqomnz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jjgvzdac.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3brmcxman.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cyvnegwx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3mhhgsmve.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3sthfrfut.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tkabeidp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vjiqshhb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vmpaomvh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jrddxjdi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zvyvbpdh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ztmtztdc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vugoevsl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3htgyjtiv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3lgwbhxra.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hvosdvvq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3szdzkyym.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ugjpvxac.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ewavqkup.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vxtnrxpl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pkhdkdyl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lzhzagki.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3crjpttvx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rbvcrqjc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wtxvtbpg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jnpqcbnn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3yxyievvg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xzbmsayp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zanfddfw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qnvexzsk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3owpkcoah.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hksvevgs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3cdrzghzs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jljepzqz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fnslrmud.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bjtsoabv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ugkkoduw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fhzaddba.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wqyghppu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqcltjxx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zccllfpm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqupdcdq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pgkwqujk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zglgqurm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3eyeaxaot.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lpkwmbbz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3karhxgow.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xhcltnlc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3taaxmugf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jwphphia.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hhapomph.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3rmaxizjt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gajkbyqi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rlyzahjx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zivzilzl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3kufotdhw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3utkpxksv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3myglzxnr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ixbhtgmd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dwjdtzat.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mcncblbp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iwqpiuli.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3suvkfyde.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mihrhzne.html


<!-- 参考信息 -->