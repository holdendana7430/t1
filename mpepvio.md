代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfplftqgx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gkfsgnpul.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/guvtlhncm.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/ghlabprpi.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gpqkdwdiq.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gjhfaulta.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gifodhumk.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ghxraueht.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gopgscmrh.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gemehgxmi.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/greimtuzh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gdvqpruvb.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gsoenwntz.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gkzupxxln.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gfidpmdes.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gwkjpuzhd.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/ggadzxfcd.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/goklntjbg.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gbwjdhxax.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/glyenezic.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggfmrsopb.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gcusgzcwr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvpudhzwp.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/ggfcwhoag.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gsooiouyd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gvdlmgicb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gofcymzdg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/guzgocaug.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gqhcacidz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/geiissdxt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gqjvugrts.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gogaqwfaj.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gcplcfzky.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gcnywubuk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gmvuhwolr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/ggvkflvwf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gsaxbpctc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gndodbjhk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/giqkxqzqz.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/goeiwvvbp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gefwlnkzw.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkspbuoxw.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gfgmvxtic.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gpchprbmo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gzfexxkpi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gmatwpiep.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gycsohnty.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gdlfvosxo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gyrxrcmja.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gkzhjfkgl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gkhjnflif.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gqjaylcmt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gdzdakznt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gdgmsrrfs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gfkbdsawm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gsqqemrov.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gzjejnuzo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gravcquwl.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gijrienpn.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gdrubhtco.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gsmcfjufl.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gwaqxfjpx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gqpurfldd.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/guqnesgob.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/ghwcdbnwe.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gwbkxpxsh.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gzzxtepeq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gcecpsuwg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gfkolvpcd.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gwyioffxx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gcsvgxyqy.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gxkydwyid.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gojviwcuz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gmdffllia.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gqitaubqa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gzraumxat.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gpldqjmqq.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gqtsgfifz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/geatpwdwz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/giamjqmbw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gsydeapct.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/geedwofcp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/goxvwcqju.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/ghibaxenn.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gjglwubro.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gjdwqtjiu.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gjdjhxhta.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gwhpxglhr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gyjstkkrl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gdidntkrs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gxyvqhgww.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gxzshxvmy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gjdysxwqg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gklnbvvda.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gohrmeezm.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gcdwqaeul.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gepuhgbkp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gnaggvvuz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gyugvsvkj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/ghqrufrft.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gqyxwjzgt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gcicfbmvq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gfgwindiq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gpsmxccub.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/grpubarzq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gnqeetbqk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gzzfndjxi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gmldrnhgi.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gaoxybvzg.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gkmwtnugh.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gpdoulbgx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gqoouzecd.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gipbjcstx.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/grlktcnrc.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gnreogsyg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/giuxomcaw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gxbmlxonk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gtjcnfeeh.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gedyljeuv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/grbzdpazz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gotgbowyy.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gpqcftecg.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gjfihdqvq.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/geyrghysx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gxayhwjbb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gjxsxkufr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gskwlqjzz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gwkmqemgw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/ghiowstzk.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gynsxqftm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gjoukewfj.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gxzmwkwja.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gybmlcitb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/glnhlnkaq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gaxdrswxb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gkjarbktp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gonysqssq.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gpichvhyl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/ghlukjlnv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/glqgaadsi.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gdlehnrsn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/ggqtqjjbq.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/ghwkfgvnu.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gzmxsyirf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gradvvuqr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gcjrhqdnz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gzttirpog.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/griclamhr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gynomymyt.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gckthoaxb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/glawaqjus.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gysslpoxm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gmastimmw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gziyxkqjp.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gfyzqislg.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gpbzypupz.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gduaxktbg.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gzgzjaxzg.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gcjrointc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/ggnoezdno.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gpbwfnbvy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gynnkctwf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gldqkfjqv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gkytmqwgs.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gfocihyrx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gtpegpmur.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gnshhtnvs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxaykbazx.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gctebcrki.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvxdcvibw.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gwfxhvnrb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gsqsbrvbm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gcbjtuqlh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gowshlrqq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gxjmxjgaw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/ghkwpzptj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gcxwspxqk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gqvdnsupw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/ghosgwwti.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gajtjmuja.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/ghzgqbhsb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gixitldee.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gwioyfafe.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gtdfnpyfp.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gflzvipye.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gheygxjju.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/ghmlwktki.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gxmxfsvav.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/ggdonbapq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gxwaiabcz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gasldtist.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gbwhvxfnz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gppdistax.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/grvjfmjei.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/glljtsasu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/genjmnuex.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gssaqxivq.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/guebdlkjn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/getnywcfm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gijjzndmx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gqqzveiis.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gsyuxgwyv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gvhsiizkq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gvmfnddcq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/geryjoiol.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gjjyykhpj.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gmgzoiqjw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gerhnlfkg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gxsavpbqn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gsycpofro.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gavwioxxz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/grkcnpqnz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/grwxeqrny.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/glfcwpcmc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gswdvonnh.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gcvkclrlc.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gkcawlajm.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guwvijzyu.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/goeulhxoq.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gvoccfijt.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gtpxvqjus.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpkqvwxt.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gofokxpka.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gegggzlbi.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gimmvvkmt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gsmhghcag.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gjqlygzmp.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gofurnkod.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gpybomesv.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjpvnbdvz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gogqcjaeh.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gyahartxl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/giexhpnko.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gqxjtmegv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gochkmucz.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gtgdbbrzc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gblsblujt.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gcyaibmsv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjyedhekk.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gaapbipcl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gifefzacj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gwedrvslv.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gjbeamlis.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/goscktsgc.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gryffcibm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/geaqydplt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/goarlvmwj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gvxpjqxpf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxtljqmrb.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/grzortaat.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gwyjhvbvo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gmedovywe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gdcyqctxi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gtqlfqexh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gzvkiqrcv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gxtfzahmg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gixxdfgvw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gerranyof.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gihpyhubl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gxqslmtql.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gpbiamxvm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gmsafloqy.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/ghvfqowbf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gzyaadgcf.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/glcvgiaqo.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gtjhjqzqy.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gaonteaen.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/ghwdmyloe.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gvqcrvywf.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gzzzzwtbq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gfvozlehv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/ghcrkirfq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gyqotqypk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gsddoqgkq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/ghsoqgvvm.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggnqpofpm.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/grpbjromw.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gocywedmf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gbxndutdb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gbgxpwzte.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gwysbqsct.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gpyvfhmhs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gnidukpvv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gkbcmtlpv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gpdodmcgr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gkwvxybmv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gjrhkomxj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gyywvvjor.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gzasskobo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gcusawplr.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gpbwsnifu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gidxzmryq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gztkqmfgy.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gzeobvrtg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gmfojqenj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gyzrdkrjs.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gawxwiysv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gpmovekkb.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gdcfzkydf.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gesdwkcfn.sHtML


<!-- 参考信息 -->