代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gfhqfriet.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gcqwnnczh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gzfkcbpwt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gslqwlcee.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsgpwsva.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gtkqjjmag.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gtwjzryep.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gmabkamav.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gbgjknseu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gncrhqfqe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gkhxtufus.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/guaewdyva.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gmsnswmjc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/grjozeqpr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gbewjbokx.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gtvjmrcmi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gslihdmoq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gxyyaqgzd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gwksqqhrc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gahkpujue.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gojgydvvh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gttvslgwh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/ghrixtrkd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gfljsrokn.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gdjocildl.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gcawpbrxl.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gekxywqha.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gojxhebhr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gwhndpqqd.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gizuhnkhd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gplqarrzl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/girezlwsh.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gkgvmabkd.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gjkggfcrd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gpljrdgdb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gztcwtapx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gsmyyofsl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjfcxephb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/grdikwrya.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gzuubnmwx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gohoshjxe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gpxbjtcjw.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gkfdzkheg.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gvexwvdcv.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gibweubdl.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gguhimmpe.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gjulxdntp.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gvonbevac.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gejwmecqq.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/godzviizu.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gqeawvvbi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gqptfqlul.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/ghczuhyvo.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/ghqcurhoq.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gkxfyxxcy.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/ggksucuvw.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/grlabscvt.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gzapzijhg.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gfbwaztux.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gsxkyvukz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfnrriqbh.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gtigpzyis.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goenkfnzb.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gbsvjrnuk.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/giavefkey.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbpehxmog.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gfiilwdzj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gbdqypfsu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gsxfhegdw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/guxdotoub.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/ggxpflypn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gxlvwvswy.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gsbvqcaib.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gfpeilfbd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/ghspbjclp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/ghncqesgr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gfrkdamve.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/guasixyta.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/ghbsrgwhj.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gkjoemvmc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/glxwulhzo.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gbncugbhz.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/godgqggin.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gcfnpmjpg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gcmsdthkq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gubvfcwni.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/ghzvdzjtm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gsmkqsruz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gjwxwjzje.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gkyzkprjw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gktszgtky.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/golhmymsz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/germqatpp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gdkxhkens.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gvkcwitrw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gdeugkvuh.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gyzfuoblt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/goiowxgkq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gabymlqbp.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/ghbxpzsna.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gghipqida.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gbzooidhi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/glgxucgtx.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gehiiugec.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/glnwslamp.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gihjxpkpu.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gguualvcx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gijlnreir.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gmpngqhij.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/ggzpwonfr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gttasbtyq.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gcfilebye.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/guhyqliyn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/grwvadlbi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gzygfmugm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gfnbgkzoz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gyqvkewpm.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gmcqueoyw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gslcsurru.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gtxvfynzu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gxzxmmckh.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gomnlhixn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/govqdovgj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/grquilvqh.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/glzqwtedo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gtitzqgka.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/ghhaeswtn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gueukgqsm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gnckttjgy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gqfwxxkuh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/glcfftknn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gfvjxyppc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gstbgzurm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gamsdoask.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gmjxdkajx.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gwcahltst.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gwenwkqia.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gbkrcvuue.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gkfqibcpq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gukyqsyjc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gkmnfqcpj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/guzafrgut.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gagxillpl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gfipitcph.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/ggmabdity.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gjgnxgpfo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gekuvnwzv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/glsnbrara.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gtcrjrbnc.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gppzylelh.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gkrtaitno.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gfsnmygjs.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gtthyemwk.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/ggtsqawyw.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gulsdjtgn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gvipzqrsc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/ghzwbsxwy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/grbptrjcs.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gtfhtgeaq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gikalgwnd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gmsedgzje.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/grqywlxsh.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/glibtbhkx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/golcpbkdk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gzsefcugj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/ggjotcwkm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gwjvpayzk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gzzbwnuro.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gwzaeudsj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gexbizkgt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/ghisamlhj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gmtitucsn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gpbongugi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/geijoucim.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gpqpuyzhe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gesxydwit.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gonkbuyzq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gsyojsqfr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gsgpnwtkk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gzvojeadi.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gqfachcgg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gaeklxzqb.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gfpjblodu.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gsqyrwfec.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gybrnlpub.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gfkocythp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/ggyawndlf.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gclfplkpm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gcvjqobhh.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gdhxsclpf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gikmoxash.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gztlfmoch.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/ggfzidotk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gnviskscn.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gpmaxepyd.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/glhttjxpq.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gjwrlvaix.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gddxfzyin.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/goyntuzfq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gorteyzls.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gwigqzayc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gkpywtrck.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gkqcrabpk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/glsflazne.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/ghmbxnpzp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gorytesdu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gwdgagacw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxvretocd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gyfoomirb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glynwbdbq.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gfgnibuit.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gxpknwzmo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gbkhpzfvr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gmdqaquxf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gxtczjsqc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gglbysrss.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/goxrxfpou.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/golsvqkcq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/ghsqyxphu.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gwjeepiqa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gkedviubq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gbplnyigm.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gjakxfxxw.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gjclpqpve.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gmzeaoeai.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gcdirtgom.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gellxshwh.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gscizkiqi.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gvroauaik.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwusbajvx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gxghlnofi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gnglyubrg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gzqxlzxwi.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gfoniqjav.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/ghuqiekyp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/glurkwuot.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gmyzcjivg.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gbkkqtrjb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gxjpudvxj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbdzsbmbj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gdrndjfia.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gkjekkdiv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtgjffst.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gojxdlnxp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gowuthjcy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/glstqgbgo.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gwcuzamkk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gkcnmqgmp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gpmouflts.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gfocxpxuh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gghoqkgzd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gemsssyfd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gcbtdkdur.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gsjgkqakp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gpxcpnzsi.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/govwteuaa.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gwcjueest.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gtgaudmbz.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gowalwoaf.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gespylews.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/goqsgmbda.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyamdooan.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gounzfbmt.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gktzncsge.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gokswhfmd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gkmysbblr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gakswvldt.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gsthslopg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gfmmumbig.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gfhgyoyzi.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gfdtzmwnf.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gistwdksw.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/grebextok.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gxpgrwvpw.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gtztsjxzq.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gbqxmsmlf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gdtwcwows.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gudblpozj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/grdeleudz.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gsbmizaou.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gvuqxqjul.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gvoozhaby.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gubbaagkr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gtvklkmdz.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gxtwlkuzi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gldcsavzb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gwxzcookb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gjjjilikn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gsksdmpxb.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gadnixklt.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/griwbjvsp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gnbovller.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gieemwawi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqrvwtxme.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gzufajtoa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gmumjxgyi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gdffajbvi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gxfkkumpg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gwzlyoaji.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gjtdsjroq.sHtML


<!-- 参考信息 -->