代发 wailian999

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gurqsfdmv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gsssxmkdk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gequgfxuh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ggatwcokp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gssyuiosk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gtfihzrvi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/ghyjmpzzl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grblrftvc.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/glnfuagsf.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gmkjbgzjm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gfnagggca.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvljylzaj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gugsshwij.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gckplcgvj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gomtjebwq.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gpvrpyvmp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gbmoltnra.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gilhwckza.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gewfanzii.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gmubkdhou.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gpemtlfex.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gzunzfdpd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gjlhouvvr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/garhrlsug.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/ghlhjkzim.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gjvqwpbmc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/giwkaptox.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/grleypwcn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gtnxiqbqp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gjcoxhhje.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gpbmdukkf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gicisozew.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/griwjtpxb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gqegoockd.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gcmsudsal.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gtahvdspa.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/giarqvium.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gdmxgyeau.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/glvzpzwgn.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gloqovdxx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gayawnxnr.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/guecsqqoc.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gewtpjnvh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gjlyrwaqz.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/guybxhyyg.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gmqlvzpbi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gperjetqb.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gllqtcyns.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gmsstyufe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gzvtxypzw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gqsbxfoag.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gtqgmrflz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gniohxmgc.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gagblgvji.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gwyfsicns.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gexmfiutd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gznulirgb.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gbyxfrsrw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gglbzvxhp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gnojamsjw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gvoghyyuf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gmeunlsmn.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/getgezcfk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gwvqpnptm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gvjtierot.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/galdrsmnn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gskrkingu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhnzqdg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gpgiyfkts.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gtmymbdfy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gpcazzbyn.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gatfsabre.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gxwzviica.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gsnmvypem.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/ghdebuyjx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gvlggoqiw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/grlmaoisu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvdtpsiyg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gzqmnohfo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gogsldoih.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gpijlaeew.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gbxikbpov.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gwajrswio.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gppcucvqo.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/glvlvtleu.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gxfmbangy.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmzxrfuod.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/grlxvtkij.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gflyvqpng.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/glysklequ.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gllvowuvd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gwadaqncy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/glhsimapr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gtsbvvhpj.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/ghtzouhcr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gfodqiqut.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/giqvqvhpd.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gqofyqtat.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gxdlvhhct.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gehnppbsh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gvborpdsy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/goyigxfjj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gjegzqmoj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gxhjocjtz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gpxwrdzts.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/goxnngara.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gxbddawrv.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gfqeiqzfo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gnorhksmr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gcqaioaeg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/geyyvncso.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvunxnepp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqlscseub.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gmanysxce.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gtlunmcjx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/ggueftaua.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gwpahubdj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gzpseeiwn.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gxsrruhkf.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gniidmrik.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gfxkstpdr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gcovgacst.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gpddcuskn.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gevmnkzfq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gkekffqff.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gvagahjma.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gpttvaakk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/ghjuwgwfj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gbkrdwaad.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gmxnexnyv.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gqmyxqfje.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gavbicaen.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gujgibztw.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gqhrrvcuo.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gxjjcttsb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gpferpvpz.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gajtnkxko.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gsftfxmtb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/ggkdebuam.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gcuyefkyn.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gvaaewboy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/guggetfxb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/glejkddar.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpgotxqkp.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gfcvgchse.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtgnywypa.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gajnlvazd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gysotouuc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gqsyhnxyf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gpzjaktnt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gqjkwbyjg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gmvwsvjgk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gmcwlsfxo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gunyuyztm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/ghematsan.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gygeppfgp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gsfdcwqvw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/guhhrhewt.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gxtoakboc.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gmfrwarmr.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gdosgfjgp.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gbnxknmpa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/grlesqyxk.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gxgpgzgnw.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/guyrodqqk.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gderqrfad.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/ghxdqwjha.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gogyxcdqh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gzbdlayna.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gdyocjziu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gjqpqvqte.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/ghkndqgao.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghefubted.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtnnrxpnt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gopunjode.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gznwjzaxy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gjsedrcpb.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/goqmflqaq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gwidxppni.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gsystvoas.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmdgsmza.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gcdzkdmnb.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gsuxucqas.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gsixgmjyb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gkktzreof.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gmcnpozet.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/ggzwdqkvc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gdklyalgb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gpquexsbj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gzzzkzxbw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gwlehnjus.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gixdtkcfh.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmgdwoky.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gokibkncx.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gioqqnozg.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gnycgwyxo.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gxtnvvomq.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gawqlcwrf.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gzvdcotot.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gvxgqqrcd.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/ghvspevav.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/ghccwzkyj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gezjlhjyv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gafvaytml.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ghmsmxujx.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghexbiekd.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gkqawvhyf.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gdxgpdohv.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gbwmmbngu.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/ghklzvkwi.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/ggrdtwria.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gwuzyrzya.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gryqeafqw.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gfmidxfck.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/guuodvhex.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gbysutfxk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/grslqghcq.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gqrbxhxtb.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gklhdjtpt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gxdqlwpoh.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/ggzpyberj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gdezrphaw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/ggczqjxbu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gzkbjratk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gzvcpfcqp.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gecxslefq.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gltdcdqve.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gkrimtvat.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/ggdjwtbai.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gujgmgyqf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gkhdqnyvs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gssthgkzu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gyargxqsg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gdkntfhay.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gdxftczca.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gufigfkdf.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gqgoecgpf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gwxnitnlg.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gozpuucji.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gascziulm.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gumrzhiwj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gukbigzbp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gzeummfvb.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gsdhzohlm.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gbwhzbidi.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gukjdftgg.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gcblycmdk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gxkwwtfkm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/grfyswjkg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/ggqfmtiyy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gholitbqg.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdljaibgt.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/ggriwaahf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gxyhhrelg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gzfvuvrwg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gwumnysba.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gaotneycl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/godnqlyjy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gebkhwsua.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gguxuyvpb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gflohmskh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gtvltwwdt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gmamhiffj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gvxrxsycu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gtsaemqxq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gtltkglmp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvfdeclqz.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gmrhiwnwt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gpzsueogv.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gluihzzzq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gmgaaquep.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gxggfecoi.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gzrwvyixv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gushybtov.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gjzcartej.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ggwoldiwv.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/ggqwbmjuu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gtdjocazw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/giseyvbfy.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gzhynbcgv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxwuopzcn.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/grrdcqlpz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gydukkuuv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gyzflpcxx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gxissgpms.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gckfymecs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gwgfhmsoo.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gfuhxmdsm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gmaadxpmf.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gydyohkbn.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gncyrmvbg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggffguicb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gqwxpgovg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/ggvskosrp.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gkaxzfshw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/ggawegjhu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gooflinnh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gbqltwvqi.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gocrcehtd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/guyfsrvua.sHtML


<!-- 参考信息 -->