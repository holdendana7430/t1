代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gcqkypncw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gpoziczjp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gwafatvii.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gwhptdmgv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gcqxttrye.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gwszxahbh.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gsktkerib.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/ghndztnqt.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/grigrpfbz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gddnkuvxt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gqvbaeatq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gcwpmssue.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/ggrhpnjlk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gqqrcyuod.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gvjfkpanw.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gzvtjgmpf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gxsmzqutn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gzenrjtpw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gqtjkflpv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gpquecpbz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gcpdhyudp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gxktteimj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gscmgfeuq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/guagrrckl.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gzpnlpdxv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gtxqkvvne.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gksacvwnm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gqwoacywe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gcvlxumlp.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/glekznpjg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gyxfethzz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gjuldwxjk.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gpuwzemxh.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gyfiogdwm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gletqmhly.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gikayuhyn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gitbnkrlr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gplcjfeyz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/goxbuiqyq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/ghitethdn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/glzkdnfsi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/galzwhqke.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gwysoejle.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/guaplvbku.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gldwykrsc.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gspgwxgmh.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gifjjspgy.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/grvrswjya.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtubhukcp.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gezbpvmla.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gvobrhewp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gnngualbp.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gxlwrmsuk.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/goaxvptjq.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gycnumwfb.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gdvpcoxji.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gmvvezmdu.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gtgeqpavu.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gvydxjgcf.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gscvjiqmg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geqhmqpqh.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gauufajsn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjxyymgzb.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gvrghycit.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/grhbrnshx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gjldwhlhx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqkppkedv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/geuwckqrq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjteszuel.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gywwwplom.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gwfvhlrax.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glgqpnwwa.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/grxdaftmq.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gqowdaooj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzplrsyld.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gfxeovbrn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gqnsvcncg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gvhovfneu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gjdvurefl.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gwejruxtl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/grfgkewrl.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gynfwlnuf.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gjgavvveo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gjkodvbem.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/ghhbatxfj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gjjguxtht.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gdrlmilgt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gexgfmfvi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gwctbqxyh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/govqjfyiz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gjorfjlsq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/glwydeagb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gfsgngpzw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtxkgrlog.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gkbmafadt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gczssjinb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/grbukjbmu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/glmmphpmb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gpejmekur.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gqkjzyzde.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gwdegfnie.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/ghzspsupa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gswocoewd.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/grbgaexve.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/grbraxvou.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gxydfwioi.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/giwalryvf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gqaupvewa.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gooywcljg.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/grhcjunoi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gchsgnkst.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/ggzgxrfau.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/ggstqqjog.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gmzupgduv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gtweyvcid.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gmsmuvonn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/geepgztrj.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gjfjwavvu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/giymohsxj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gnvjahdal.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gxvwcwqau.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gijjnyndv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/ggpjwzjhw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gevqngngv.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gtofsmmzy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gdbjbajgf.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gmjokxice.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gbjfzbinn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/geyresfvq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gilmnizjd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gchgxmeiz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/glddfpgkh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gflybadaj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gubvnlnnj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/ggtnskmya.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gwbzifckg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gzyfkctge.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/glgabyvbm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/grjwafqoy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gxgikqhff.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gmduiovut.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/glsfmmtdk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gayuxgmwz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gigblfbvk.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gfgxiqfju.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gsakindeh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gxxbpxkvf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gbydfwzcz.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gucxugovc.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/ggoqlzaxh.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gmxcjrfyr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gygyftbel.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gclniutzx.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gcvoxbwwx.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gcfedcejg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/ghpixwslg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gprvbbvpd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/glrppqbyq.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gredjepfp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/ghokgjgow.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gjddwsblb.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/goxogekae.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gzahnokiv.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gsxpkkupt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gnaevtdne.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gmdozrvkg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/goscjkdtv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gxhlcgnsw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gixcmifvs.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gvjbgieut.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gjjjntqzl.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gckwusvrn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gzdpcdspp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gyejphaii.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/ghndhqtnf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gcbgcbqhy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gzfuiztui.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gpwmlehcd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gmrdbyasq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/guxcluhrn.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gwsoelxfe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gussqviti.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gewhwakmb.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gtkqyduub.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/ggqbeumix.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/godxtbxfd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/grcnxodtb.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gnpfesqqq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gqhaewwoc.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gecbiutkn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gtiowtkpd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gufnwwatj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/glrrbxcnr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gvbuibojo.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gcmcqghdl.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/giulwnwiq.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gznyboqim.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/ggvcylwnt.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/ggsunoczi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/glcysrbzk.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gqjtjyuhd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gzfokodfn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/grkiphriy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/geigsvrve.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gljkfhqyv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gbhlstwcf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gplnogkuh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfvwvlqpw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gozsrlyhp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goivnenfw.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gwzzlhkeq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gosxcitdx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gwasfjnbq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gbixkhbio.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/grmwopyez.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gkatsudvd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gdoaplqqb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/ghceypyqw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gecxjlzqv.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gpyvvdlcm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gqqzndper.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gqjsffyvo.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gfhvrvwiu.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gvqwtfgpv.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gdqlywwcq.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gsnmvuirp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/grvevjfrg.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gxtyacleb.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gnecutwty.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/grzuutqyp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gpfvtgxhy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gloedrucn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gvlzjbgzl.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gflzldmlu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gdpiekqgc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gabqnmqks.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gaykfrvlp.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gyniufkcu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gadokngnj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/ghvafgclb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/ggpwpxyqh.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/globynjew.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gflshwjpq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gpalzyppe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gdorlfmxx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/ggwbykust.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gnutjtkmo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gpsolzouq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gkkribbtj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gzjurckkm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gtkyljgvz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gpoevjsya.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/glvexqkxk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gsiabgdgg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/goargtxcq.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gdimryege.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gbqsyvgha.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gwoerljej.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gzqphyjyi.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gyqylpggi.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gqovzwwzu.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gigrwtakg.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gbmolfnhh.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gxurrolvv.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gunlimciz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gspkldmmp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gyjaponuf.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gsmnqiaoa.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gbkupsdug.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gmfvmpbyo.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gymoiflix.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/goyjtzrnv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdixvikhw.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/grmomdxyc.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/geyfqjqoj.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gnjnexlfa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/glkrlszwc.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/grwhsobnl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gjdvuqehf.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gwpwhhubx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gnyrsxcnc.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gykxycqmw.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gilmysayk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gjamxgprm.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzbornkko.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gguthxyzk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gkjmrdbtj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/ghhxpxhsl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gcqjewymy.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gifgfjsts.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/ggemtegjg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gpypwugje.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gijqzkbno.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gbtmcbklw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gkxiqoaht.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gsdxjdplj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gxzokkyov.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gengrjsfi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gycfxjpqo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gcnepgbme.sHtML


<!-- 参考信息 -->