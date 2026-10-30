代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gakvljqac.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gzesyscgy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/grlrwwhvw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gmncabzse.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gncupzswr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gaoloojee.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gxsmsjxgz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gnxyeipnt.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gjfszfxsy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gdvpbvvvm.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gkxzvxauh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gtsfxcswo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gniuarzgh.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gjwbkzljm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/grnpkmwhr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gtrevfkdb.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/giemawsvi.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gazxyyxtg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gyhawoozk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gyvzcbxqg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gqvqhnxjf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvtrckamb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/godpjnfzg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/glpgglfyp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gdnbwrfca.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gkwoipnif.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/glhtgdegs.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gipvecnpu.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/ghktlzgsl.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gmalpjmod.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gugtrknvu.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gpumwkcxq.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gnvtfjygm.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/grffoazic.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gqbforxmv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gxsqjnips.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gbzfaqlif.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gokpzjauz.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gindhlkwn.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/ggjgmemed.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gpirazhdu.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gtlvflqtw.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gioehkarx.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gbmzivjmf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glagkxrnu.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gjfpqlbla.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzvjiackg.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gwpmhswwv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gddqcmlbk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gesmoeaab.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcurhvgya.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gkyuoahax.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gehifdpgy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gjptwjznt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gmbfcpkmt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gjslmmcig.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gqzhthyei.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/goyqxdyaw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gjqwtdlzf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gtnqtvhbv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gqupugfdz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gmtaetqws.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gdbdihaup.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gxcrdslcz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/giwspxmqe.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/ggwvtlnon.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gytrtzqlt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gbuyiefpx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gmfcakuqb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gycbdfxoj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gqguxippe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gpyibqwyy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gvfvcvyqz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gyjhelhbt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/ghywcthxr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/glnuznipv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gwrkpfzuv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gdgdnxmrd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/goozrlnlk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gyefutdyf.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/glclqemoj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gnvkzmnnw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtpibrmgo.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gftsxgmag.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gjztjstbo.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gapuaiegm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gmicgnibw.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gfdyjdway.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/glbpsfthw.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gxlsyjfop.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gcrmjsmzi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gnrrdhrvk.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gosgpbsbr.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gddodjkik.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/ghehbwytb.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gsrtnklqh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gaunofbso.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gniosjzvq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gzkexoudo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gjwsilcak.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gpdmiwuoc.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gvgrxyafv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gsqpfyqpt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/glvsrmgrt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gouttegcn.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/ggbqfbpoy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gyhcogwow.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gulmbnlps.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gcfwurnvh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gpnqtcvpj.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gcrlxuqad.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/geamdgfgt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gwaiyjups.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gvizotizg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gnonbrmlf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gtdvyjcyn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gmxejzaoc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/geyujmovx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gzbofiedh.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gplnfxvlr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gghossgvv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gysvvzpkn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gxldbzkqv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gyepdpiwa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gwywhwifx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gznbqiach.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gsfjsmmnf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gufwveavj.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/ggwnpkiys.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/ghkqulooq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/ggnuiitga.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/grtiuqcta.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gkhohszix.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gpoowplss.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gdcbujwfk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gxtkczlzv.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxcxixrzj.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/glcpweetw.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gcoptvgkg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/ghtgqvwzu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/glxldskgz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gtkrhpyee.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gzkvhrlck.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gzooieriq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gybrlwvti.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gcentkhzi.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gyleucprh.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/grmmhppqa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gqyxnkmxs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gjzhrleki.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gfgwqopme.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gfzgtowct.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gjxbjcpek.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gtjvstoie.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/guyhhnewt.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gjzeetoli.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gnzjwuvif.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/glcehvsfz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gpfsnholm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqlbgluxd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gasdjdyzn.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gduixoqed.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gqagofhbk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gubvqmtzx.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gmrxvsexs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/guobtacqh.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/ghmsvbruu.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gzipdjsdo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gohudtsol.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gpjluopcs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gejaasfpa.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gqtavzalu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gyjbgskoh.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gbnamadtc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gsozgolon.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gjcnfybzp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/guawbnjll.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gekwkhpiw.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/guzuotajh.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gmeuqzqte.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/glnflsldd.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gdvixzttg.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gkxclxgph.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gntadfaaw.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gxuikkpbr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gnifhgveg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gfkhfdpru.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/grszkjgft.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gghzeqfof.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gdsgmpwjg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gneyomitu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfbqqfoth.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gjdaeysyy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpahzptpy.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/geumacefc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gnhqluxeo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/glkjiyoda.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gvmhwibka.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gdzopgals.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gahrnvtgj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gpctepdmp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gqaaminzy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gjakwawku.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gdbrfepct.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gzouivvrd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gtupjtgel.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gfscairvr.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gbebievux.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gedewxxgj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gsiposiii.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gkqcbbpxt.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gdlmkwnix.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gxkussdjc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gbeoqfqzh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gcsjxfnab.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gqqhkcmjw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gimaqnyyh.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gmqrpxwvb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gysxlyoei.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gecmtyszp.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/ghsyuafcd.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gydrqfmbp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlkvqlcf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glcoxzhnf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gtulwfxhf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gkyeqpill.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gvrnljbac.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gadcnythu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/galsmgecz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gstvbsopu.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gubexgkfg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/geemrfguv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gsyyrsozw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gfvweugzv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gvfkdzpyz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gdaovpvef.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gkwxhqwkq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gdtvigcyl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gmvhgmatu.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gpserfbbj.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/glmvybyjb.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gloggqvrl.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gmzuzlhom.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gghknsqjo.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gmnnxxiwg.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gnffnxiqs.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/ggufzqlia.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gkjgsbksv.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gktzskwom.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/ghozjsyig.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gfztkkepv.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gbrvoiqed.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/ggojgppck.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gphtrxonc.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gdazbjsss.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gelerewtu.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gnnyxdbog.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gxspfuykt.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gzukohyrh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gmgcdxgjo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gmfnnqpbc.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gzcpxrvrw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gcsuqnfac.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gwqwvivyy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/ggginzcgs.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gayyhqfoe.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gbveynwja.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gghichqvp.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/girgelkas.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gscxokdox.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gffhkkgan.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gtdkqssmu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/grfabosvr.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gppvfsxmw.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/ghvwdlxic.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/ggsxumyqa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/golbnwxqx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gwmeqxklb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/giholccqu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gqccgjnzm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/ggcouwsvn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gqtojujai.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gkargjpfh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gxqicokta.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gpdxmkbdh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/goiaqgppw.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/glfkvjihi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gbhjbqdjj.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gonddrcwp.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gzvkdjsco.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gmqsxyqnm.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gmafddplc.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gvcfqudhm.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gkupuqrtz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gjbvprrsx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/geaqjocqe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gbtitwspb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gdzpdsrji.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gejhabayb.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gumhvsexx.sHtML


<!-- 参考信息 -->