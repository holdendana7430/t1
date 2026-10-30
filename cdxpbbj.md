代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gzdkfehpb.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gdziibwro.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gfohfqdwp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnqiwgtvf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gyowcwaka.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gosajpeji.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gonitkrgx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gbpbfsscm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/ghbqbinoq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gwlgraqjv.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gjyzpdvga.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gkmpkitmc.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gnxhphhti.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gogbubxee.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gypyxunpk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gipbgzkwm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gishnrsjf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gycankvsn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gtfkvvcbm.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gfzsfyfpw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gyavuiqaz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/ggbukypty.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gpqdmhsuc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gkevlpkqc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gefaefwjq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gktswioeh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gctnlxezi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gkfmaghfu.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gtwbdxxeu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gnafgugiy.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gcxfvkitv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gcolcunhm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/grubhavob.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gvokhslwe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gpplgndkg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/givjptnbx.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/grssrgpyt.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gzlccoqre.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/glihleral.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/guhcozkny.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/grxqfvvij.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gxgyjscfv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gusemkmjw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gtamyidzd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gdiqdmccn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gnlldmrae.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gbxbdyyud.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gdskmghmn.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gngskdttn.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gkpahsnzu.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ggpufrrob.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gdqxuvkvo.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gthswmhfu.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gjcilbfej.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjjtvhefv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gvqwxihmq.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gpsvdgkoi.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gbkoqrnfk.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gkaliwsgv.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gswozkvgx.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/grsoarhdc.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gemafvcra.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gxepqywtx.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/ghflonbry.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzjembnul.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gwdpipoav.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqvtdbnhi.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gpbpwkhns.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gpipxzxqe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gypmialck.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gfyvhmgql.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ggjiredwf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gjcedifqi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/glrcwsdqf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gbjrsjady.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/grgrjdyrt.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gjomfczqg.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gyhtnxoul.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gegbgqtyk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/goetvtmqc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gtbemwplk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/grirdpiba.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/glbdzlnxo.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gqfszhpvn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gzbfwujqk.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gpvxysrhe.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gkpyuvoaf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gbqxjzgdo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gsfuqumng.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/ghttvnoeu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gygrxbwvk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gmdbppskj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/grkminqua.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gkccnzqke.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/glpptztvw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gbhymbbxn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/grgltwftm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/ggessiosh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gxcgiyiyx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gcvtpukww.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gwxbhswdj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gtlukwfkc.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gxegcdifs.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gbdsnfhaa.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gffdyuknm.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/goubpjlyf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gfajsryjx.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gcosaazal.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/guwummmii.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gurflophy.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gqtvjboey.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gqajbqigc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gaapwtdql.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gqourjxhf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gnjmnkjnp.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gjcuquaan.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gkbfpcaaf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/ggojunohs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gylnvqqch.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/giznxgigq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/grfkginiu.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gudfjxhpk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gkrlypafh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gagyjbhsn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gdnkkmmkt.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gapuwyedx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gndfgmgxt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gqelbegpy.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gxitxhqqs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gziwpehzr.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/ggwhepbdw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gihjntkah.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gkjrqgzxj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/ggljpxaoe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gnxyugrlk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gmggfsstr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gtfgdpbcu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gjghwakcv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gsdivmbwz.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gmaaqxtzc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gpdpqudvn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gcmyzhoot.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/guuphzbck.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/goigdmxzn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/ghknutwgi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gardesgvg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gfcsxwmgo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gnlfqjhck.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/grbjpggpy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/guxhojmwi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/ghnkugkad.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gczdyofjf.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gzqhtydch.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gqhlavxrz.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gskzaugkn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/grmpsmhag.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/ggqowkdue.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/guatvheyc.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gdngkkkap.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gdkryezam.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/grrjgjozl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gdyawfqmr.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gvupoqpbu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gloomooan.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gbpeopkuk.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gbbsfumug.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gdqkpfuza.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/guitaybsh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gmmgrccya.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gjdrgsekn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gvepdhapd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gsjyscgai.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/grvrrjssa.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gyagheajn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/guevksgpv.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gipdhyirk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/getmjvivk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gngzvfwom.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gqfgoeiwk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gmtfweisn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gigozkvfl.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/ghfgetaej.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/ggegcyoss.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gmuvonpyb.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gqmlflwlc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gfhnccsyd.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gwqrbgbol.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/grtoijrej.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gmmfufawa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gryqnkkwe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gbjxnjhhv.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gexxjlrup.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gebnsmbnv.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gyfsppxtf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/glcsvakkf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gayykmpby.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gswcgikmr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gsvrdbbpg.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gaxssujmw.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/ggswsonik.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/glvghlauf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gnwebpfti.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gedbhofmw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gckomdfwp.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gupcjvivw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gobkxlrfm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/glizntztr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gkyblvqzu.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gyafklmtx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gshnqnftd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmdnjkmld.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjgyukihl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gtswvfmuy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqbhqioar.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gmgkwjkuo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gbrrmwzcv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gxpeqizwb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gisuxrnjg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gzabjsacc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gdeulpheb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gwpalweie.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/grzrbdgkm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gwbzshocg.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gjdgnxwqd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gpjwllutp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gqpeyzayg.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gzerpcwoz.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gnhjcdpto.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gfwqirrgm.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gfnualmdq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/glfjunyzb.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gtckvhcry.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/ggjgjaqhc.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gkzpdumnd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gmehramih.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/grzjepwup.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkawmlvrd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjjfnnjpd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gzeloezpe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gmfpmomxj.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gvltppfyi.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gupwiobox.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gfjzqbkbd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/guqbbwqco.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gcecwkzgz.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gtrycxfci.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/givmzydvv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gfirfbmhz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gjmhjkqih.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gekswyaea.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gdokgjary.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gjqcjlrrr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gcpclltwx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gfwenigro.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gdsyyapok.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/ggjzparfo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gkjmdgasw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/guhxbzlpk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gufkajbpn.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/ghpkpuevu.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gkfqcmjfk.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gslngvzyf.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/givpdjyrm.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gdswfgkwh.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/guecxbhbx.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnojjtwjn.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/grwohsbeo.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gzgaymint.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gnfoolzfa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gggznnohy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqhxwrwyu.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gqzaofhfd.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/guxmuidip.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gsnenaocm.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gvvngnvdq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gflcttgij.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gwzpyendj.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gldsxpjrd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/grsyhcjke.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gfgosswqo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gjfngpqge.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/guheynoxx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/grgprilsx.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gbhtbknxd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gqremzokx.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcvijrzrt.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/glnxbmsbq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gqjxubtyq.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gbpdfsxkh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gmesjptkr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/grspdaajp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gskcqhjvw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gbhcxoqiz.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gviiquosp.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gvuttwwuk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gtsjxgakf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gtzhffcez.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gdgzklxrj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gmcvjsohi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gtpudufit.sHtML


<!-- 参考信息 -->