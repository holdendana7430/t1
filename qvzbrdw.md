代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gtvgvazfi.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gvbmbdrhy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gloibldic.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/grumzbqen.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gpslbwcxe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/ghysjrwls.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gkgbdbsiz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gxbpbyuwr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gwxjsctcw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gpscboioe.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gpxohvcef.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/guhkglbmj.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gbrwyycfh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtknggycc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gvzatlnrz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/glfyrcdlm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gxjnitfdz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gcqicwrro.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gykxjxdoc.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gnphxbtnj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gcaeovawl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gcrlvakdm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/genzywtwe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gacnitbxx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gttxxiysj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gekqlphou.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/goytrnzhe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gtepzhivc.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gtnauaouk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gyqesjkql.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gbnineech.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/ghaisikko.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gbxlsxahs.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gfgzyukge.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gpiwitrjt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/giwhsccpb.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gasbkqzhx.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/goasvhxsc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/ghuwvrzkg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/ggtapkyxk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/ggjphskoa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gjqurkmhp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/ggnmawezj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gljwgdsru.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/grlwkxery.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gyztyqkqk.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gjasfghdv.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gegymxczq.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gzlhhqmjt.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gxtalcnsa.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gloteirhg.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gtgpkrrne.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ggjvilcjm.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gqmreyuux.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gsceravyf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gdgdjuyen.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gklwqwdxc.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gqdfpbfzh.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gndibdxzl.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gjxxlzwja.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gieosafhc.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gurekmjvp.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/giglfdkpe.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gzbdkoqod.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glwwopytt.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gdiipzxqu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gknxpmqoo.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gyhbqeder.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gykpooboa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gnswgxfjc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gvfwhjrjc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/goryaimco.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/ghgysvxxd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gxytwpisg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/guychoxro.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/grzwepxwz.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gqoljetng.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gvyrljagl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gkqfptupg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/giattdmic.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gtlcqsfhr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gxvidkill.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gnpngbxce.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gajvlrxxk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gbdbtfwjh.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gjudaqjpq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gelptnswu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gkiijwdab.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/glxgmwfpw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/grokoixxi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpbktrzxb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gmbunzdtg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gzgenqgui.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/ghzargknx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gyvciuqsv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gavswtcdw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/giprnguec.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gnbqkixbd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gvzwghqdx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/ggmpzgbyn.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/geepzftdw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/goyhxwgvr.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gdmqzqgmg.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gxgyctbkg.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/ghibdrrso.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gzduhuxdg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gdhpuwisx.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/grafpiwql.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gwilaljxe.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/grbhxrlfk.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gimitjipy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gelkhxilo.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gxarolyuu.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gumhpyoah.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gmkssabgo.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gosijurkz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gnbjosyvj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gheeerkxz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gxgbvvxzp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/ggrcwhbzl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gwksjwcwm.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gediqeysx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gskvrjttk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gzkrdoegy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gweoqjmmn.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/ggumxnbhv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/ghfvrpnja.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gczvfhelz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gcjkerqop.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/glnirqrsp.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gjbaxtgxp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gxssjtzrp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gxgkpsrcs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gvowiynkb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gdnuyylsb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gswnosnys.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gbscefohy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gtqtxlymz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gzoakfktt.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gmvwnhkva.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gcynhxyab.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gohdafmaj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/ghphnrvjr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gonznfhwx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gosxxbinn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gvansijzf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gtwsrbtjg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/ghdevbnay.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gtbvmryzi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gugjooxzh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/ggtfgpcpq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gtebichtp.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/geozwvsxm.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gwlpunacq.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gorakfkji.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/ghgdcbvqz.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gjgvxpvcx.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gryexcddw.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gqgizjdjb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gvmawleei.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gcyxkfgod.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gfomuujqi.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/grfspxxss.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/giadyzfvb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gvvkrdmhv.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/geyjydgzg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gahzqyptj.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gpyccaptj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/ggaagvvxp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/givmybwyj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/geurqyfht.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gunazhusf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gyjnyudgy.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gbigrkzut.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gjoavruag.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gefhkzjxv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gkfygykua.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/godvautxm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gaopwrluh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdpynfycx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwvurzijb.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gfprsbawg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gzcyhkuwm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gpbyoghxc.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gdnedcfit.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gqqrwlpua.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gewkqsdha.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gnuhqfhyy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gifpudzur.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/ggcgopwqi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/ghnbtdiqq.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gkluadouk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gpvfgearx.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gvkjbdlab.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gywzjewlu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gvddujvve.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gkljpwrek.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gzadmyhxh.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gekoybfmn.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gpboxjrgk.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gdbvhygkw.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gmbaayovy.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gbvurrjgk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/ganehcdel.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gzbqjhgxo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gsibahrmo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gozeelbft.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gwbucdyam.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gdydzcflk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/ghlqugrks.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gpbudqsnp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpngmsgrt.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gotucvkby.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gczlcajgq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gwdeirmni.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/ggesiezws.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gdaizapkt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gczaupqjw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gfmrjiike.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/giahvbmcw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gkqghzidp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gfffrlmqm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/graryqxll.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gsdtydiyg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gvblgfpol.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gdutfnneg.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gwhhuzfkv.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gtbxmsvvv.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gftyhcrsf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gpyxrupae.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gvqjqucyp.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gaxsxlyqo.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/grumnwcqb.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gwymdtrob.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gqwpxkuym.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gugvocqps.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/glhgeswbf.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/glnvrkgmr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/goodolgam.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gminaqusq.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/ghntutoup.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gkkofnctc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gskusvkve.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gopwehjmg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gyhtaufqq.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gwdffeeqc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gziqkkjbw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gpteppkba.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gktkybyuy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gomnsemlv.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/geyzhcmxy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/ggoogtqkk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gevvjgiea.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gqufpycof.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gpfenpqpg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gangeezam.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gdmeqofgj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gnygfcsmh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/glodeqydq.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gtgsiallf.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ggvnkgbyg.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/glbtvzkyg.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gomxgijxq.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gwadmlvsa.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gucjuqifx.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/glxljvpft.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gbxufsvrf.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gxfwnzweb.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/glmilegce.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gncaxecnx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gzrctwnhm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gtxujxeeh.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gpkxgjuce.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/geavlakyk.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/ghdgzjjts.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gkpwpqhte.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvsgnovpv.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gmwkwciui.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gvxifkcgy.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gwmcpwyti.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gudsbwabw.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gzzikdknd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gnvxlxjrq.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gqsjfilxb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gyryylrpz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gmwpmedeg.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gsefrjsyt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/ggyiwlqjh.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gsijjbisn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gwymacgtb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/ggztaxpoy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gdumxczng.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gfjmygvem.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gklwxdqrc.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gsiybihxv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/ggoqcohxg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gqwluqcpb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/ghseybjdh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gxgvyguup.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gsumgvazi.sHtML


<!-- 参考信息 -->