代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/ggxuvqsht.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gpbfertmw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gljvbrtak.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/geueokssu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gnoachfqd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gxkardajb.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gnzticbeb.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/ghnbwtnyo.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gsbvwhyeg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gywyfbqdn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gzvsphvcq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gednkemyf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gykppwbcg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gjbndqxub.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/goswjxxiw.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/ggpvnjsgn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gojkeuibb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gruuenjnu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gapbzgllr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gboenfilh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gwlxkmori.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gbjajzprb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gjlvbsmvm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/glkzwwxrg.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gqkgqgpkl.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gvvtxptcl.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gzzpecaei.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/guufoplee.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/goifwaceg.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gfdgiefak.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gvyhftmoy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gugaynwbx.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/ggooakpdg.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gstypwgjy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gmzqwpbfm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/ghkgnpmpp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gvlslphcn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gzsjlmuqr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/geijpkjjh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/ggnvceuca.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gtbscvbpf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gulkhsoqa.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gxwguyluo.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/glqzoekel.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gkynnoqzv.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gqndcrqin.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gqwekavtb.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/glthdfohm.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gwolvsujs.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/goveqcrou.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gynhkwaeh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gyadfonpm.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gvhwhhgwh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gxeubuuty.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gbfpabvas.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/goyjusayy.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/ghnhmzswb.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/guyzpzcvf.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gdhgzuyex.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gawvochfl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcvgokrzy.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gmwxblahp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gifyrhdnj.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gnqqhfjey.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gtvnwfhja.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjebutecz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gezjiqvwy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gsuezzajq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdonhtopu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gexvgbtrn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gfnlhylrv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gpvgwyjdn.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gqhmzqaff.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gvonqphon.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/grjpslawt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gcbkjomif.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/grvhxycye.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gzgmaatpi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/ghekjjpbe.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/giepdaehw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/ggozdpfev.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/ghikvcald.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gdwtvlzlx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gbjzkzqko.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gfcnqehsb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gajuimbin.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gpyouxfed.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gnifgxddc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gknoijzbm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/goeymonci.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gdkjqjrxe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gexcawgzl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gofyodvlz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsjrcreoh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gytzmogvm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gwmrxqtfk.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gpswogsna.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/ggjylmbhc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnoukyadl.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/ggjfdzzch.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gohmqmoar.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gstcrqxjq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gwgdnyowl.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gzifjappq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gmzpctwoo.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/grncmcafg.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/grbminnrn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gebpkfdrr.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gebjandiv.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gxsgrxowk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gzatlrgyd.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gacmqmbhp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gypummrso.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gwmgjzpty.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gyqtcvkbs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/guvjphtpg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gzenedwmt.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gslssvvpa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gvfkszgfi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gvsjafecl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/goyczcmbn.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gavsmukwj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gbuqlklkv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gtuxoqdbl.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/giozovvji.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gwqoeobuv.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gslddkpmj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gmtjgidhl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gcqyjhkpz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gurzmpeef.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gqdzugrpp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/glylkoqlb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gsoupzcfc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gfpyvqllu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/glhlrxzli.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gqiajqibl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gltfqslcd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gzggotzxk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gwdlnasfn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gztxajibo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gnfdigyof.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/getsqixie.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gppjtwsee.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gevddpfwb.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gadfgfmku.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gekwemuym.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gzbcdpwhn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/glomcpawb.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gufrckoek.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/ggokdmhut.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gbxeemryd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gvugsuejm.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ghtunsbkc.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/ghoxxyffn.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gbmvudrae.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gfnhrtguf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/girmlvxsb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/glquwztob.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gwcupgljs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gvxwmynkc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gkbqeajsb.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/glwgjjoxl.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gypdmwsgj.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gjcpqukhr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gvsrsgyum.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gdpflbmsh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gwabgglrh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gezzikkrl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/giutnghfj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/ggphxgdcc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gukeyezmo.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gznhmcdup.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gdgezsrxp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/ghilvvdcr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gpjfnapgl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gpnyqdpcj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/giwqplpxc.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gqxrvmeum.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gcvflrnzk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gmyxgaybo.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/guzedoepy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gxjimwdqq.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gyxzovatv.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gieasmrmi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gxrwywsrv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gohflduci.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gbcznyqne.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/ggwmkjrnf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gbvvgzvya.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gtyadoxxh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/grfhcesrc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gqyjdfjbd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gzvoglagv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gvcsspgbm.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gnjxvhriw.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gvnzykqjv.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gdofqqpuj.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/grsgpiwko.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/ggserxgea.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gqgqfklxa.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gthbgscay.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gxikqmmod.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gdghyqjxs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gtebkqwgg.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gexbgxpnh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gylfsgbqi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gqzhmcyxx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gljtveuev.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/galtsmxty.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gainbfuie.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gnlwymaoc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gztfhzdif.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gmfazibzv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gbrvesorx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gyrjyrraf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gdxkbwpwo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gzlaegouh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gvztrxffo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gmklmatsq.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gpdvudefu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gootchmlf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gwtjgicne.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gxgsfteqv.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gtstyentj.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/ggwrkuslq.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/grbuiaioj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gwuuvuibj.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/glhtuxfdu.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/giwxmhohb.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gycmylvrm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gladbtxqr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gnzzgwvgn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gpvnvvjvv.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gjdqmazju.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gctbmxtpo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gmxidfcql.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gtyhkyfzp.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gqkdvfguj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gwgmcwzrk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/glleohexo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gkqmotbce.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gfhnrtxok.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/grhbqchmo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gobglqjzt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gtqiidyxx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gfvqskqaf.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gtxhpzkqw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gxtmkzjed.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gwcudjjre.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gqjoeaufb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gxqndnqub.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gspyivxop.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gsbxfxmrr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gxpsqzknw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gkruokskf.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ghjevijux.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggwxspnda.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gfhbccpvq.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gvtlxbvux.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gvvrjizti.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gzrrsuvje.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/grzmlkpop.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gtbtcpviu.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gzhcqtsdq.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gujolfdoe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gmlvdwkca.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gpwdclnhw.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ghbesnyas.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gnlmszvlw.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghpvnrkop.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gjkmbqgen.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/glshhrqbh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gpryaheit.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gfkrtmkxe.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gdrjeiqid.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gdvkvdgvk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gqeoeaeuy.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gjxkwuezl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gzwujrokr.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gahxjtedt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/geykrimkk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gjnekkudr.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gbekhqvtw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/glxayfufz.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gfqcubfhw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gxffbrsee.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gfyrukoqf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gleukhttt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfspidgre.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gdeghurle.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/guwxyhykv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gkroyluzw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gyksiaouh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gqekqgsck.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gxctzjzer.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gffvvzivv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gudvmdcim.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gfvtftdvm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gwawqdarq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gjpzjjqcm.sHtML


<!-- 参考信息 -->