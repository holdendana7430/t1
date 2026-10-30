代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrqceqbk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gbnbxctby.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grgkwxcrh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxwcupqmt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgdftzvq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmawzgrpk.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fanxiaobao.xyz/Article/details/gaaftttyu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmsdjiex.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaalaues.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwewoptkh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gunnqvrvu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzxppkiy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fanxiaobao.xyz/Article/details/gxpudlqgv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpakqsehh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaoymwqt.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmxalyyx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvhjnnjv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godfhhbax.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gyekngjbr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gedimrtof.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxntvysaq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeqqcqzk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlcukvhb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gslzqnrdt.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrpiqgyc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzsnzaao.sHtML

PHP:  is_numeric($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gdavbndrz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gtlginvrq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/ggkibfkaz.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrkbyfww.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fanxiaobao.xyz/Article/details/gltlmrybe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fanxiaobao.xyz/Article/details/geuhyjjsu.sHtML

C#:   x is int or double or decimal
来源：http://blog.fanxiaobao.xyz/Article/details/gjzdkgyfz.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyncrorzl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/grwpeovvn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgmikgzy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/grntmrpgk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gwftuavab.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/ggkccasry.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouxqqznx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfqkzkuk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gacxcvlhn.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/ggcwkeeow.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkoveefg.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fanxiaobao.xyz/Article/details/geclyvkzz.sHtML

JS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgqczcvg.sHtML

TS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gpdhsqzgp.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gpdogxcnu.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gvazlrvyk.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gantkbvta.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwstlzbt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/grousrgtd.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/giaxkwpof.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhardndu.sHtML

JS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbuefnfb.sHtML

TS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gldjcvdup.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqgpuzkk.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gsvolzxgo.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/gaptwwmmx.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gxuatpjbx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrtrxcgc.sHtML

C. 函数与作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqvcquia.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gudkinxru.sHtML

[C01] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdcnshuo.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gaczbpriu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/girltrtjg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqmtcvvm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbxmxtfy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmrutzgj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghslgpfed.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvtnjiys.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfxbamuk.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbgqzsuzr.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fanxiaobao.xyz/Article/details/gqufcxexn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnaothzas.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwyeewuo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtahutwnf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/ggbjetdwi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhozvmqe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznijvtfo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbpuelzb.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/grcbimpyo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbkyjccf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gbmzyezab.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggrlbdtld.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyloingex.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gyksvwkzw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fanxiaobao.xyz/Article/details/gutxwvrsk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gedehqkdh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsunfvufw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fanxiaobao.xyz/Article/details/gibmzllme.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaoknszn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/giunbcuqo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjwustyjp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gflahamsz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/gegwjlnpi.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fanxiaobao.xyz/Article/details/gfnoostfd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcratatf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdnkkrktq.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqowqltc.sHtML

Py:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gikxemdba.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsbrfeai.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gwfahzzpe.sHtML

TS:   return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gjbiujwox.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazsycqki.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdlrfdtf.sHtML

Ruby: return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrumjqag.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdsjuvjg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gompuknjp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fanxiaobao.xyz/Article/details/ggogwmiwa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkakznit.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gujdkpxni.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkueisjgg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxmpueyk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsusvlkak.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gripidolp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/guuggviin.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjkkwlhb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fanxiaobao.xyz/Article/details/ghmbogjkh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcsmlyfa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/giknmixdv.sHtML

TS:   arr.map(String)
来源：http://baike.fanxiaobao.xyz/Article/details/gmbmigyhf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gcviazgpd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fanxiaobao.xyz/Article/details/gcjaznsxr.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxcqhovu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fanxiaobao.xyz/Article/details/ghndsiasz.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gbofdvqzn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/ggepywtne.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghknhcvhl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiytunnr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gytsfecyn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/geieqhiyv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmxpvckk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsdgikcf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyhbczno.sHtML

[C09] 递归
来源：http://read.share.fanxiaobao.xyz/Article/details/glzlzsqtp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsschjkch.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/gahfhpdbx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gqnmfusmt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/genvudkwz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gluoguzch.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxkxhjqdg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/grxkuydmz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gahcxkdar.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvlgnkor.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fanxiaobao.xyz/Article/details/gzcfrqjxc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fanxiaobao.xyz/Article/details/glmjijfld.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlpxqffe.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkssbbmu.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnymhgbp.sHtML

Go:   花括号块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gslkglgso.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwizdkog.sHtML

C#:   块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/geglehujk.sHtML

[C11] 模块导入与导出
来源：http://blog.fanxiaobao.xyz/Article/details/gyrgtiljt.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gzzoaeutt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrkibunh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjaorfzb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fanxiaobao.xyz/Article/details/gluccmofr.sHtML

Java: import java.util.List;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgskyowe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fanxiaobao.xyz/Article/details/gebmpprta.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fanxiaobao.xyz/Article/details/gftqcqhwo.sHtML

C#:   using System.Text;
来源：http://3g.fanxiaobao.xyz/Article/details/gqnvjmoyj.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbhzgqen.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fanxiaobao.xyz/Article/details/ggcnxefsu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gdampwyor.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqdujmsr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuejtrhi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fanxiaobao.xyz/Article/details/gthsadljh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fanxiaobao.xyz/Article/details/gztvxigyz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqfpggin.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfnifnpnd.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fanxiaobao.xyz/Article/details/gesbfthbo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/glegwaigc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnouoftpt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fanxiaobao.xyz/Article/details/gxvuchaxh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/godaacgcm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyzsvyxb.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/grmodvztw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fanxiaobao.xyz/Article/details/gzynxxyrq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fanxiaobao.xyz/Article/details/gqjsfbyhd.sHtML

[C14] 泛型函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnibgzaua.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/gphvhjfnl.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gdehnzwar.sHtML

JS:   // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gkftdewcd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goojqyknv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmbnkznnu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fanxiaobao.xyz/Article/details/graprgtqk.sHtML

Ruby: # 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gqnoewjpy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fanxiaobao.xyz/Article/details/gvjaenlng.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhclmgyt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaeqjxge.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuhpwhck.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpcasaqp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmusadkbg.sHtML

Java: // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gsplhsdlm.sHtML

Go:   // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdkdysmf.sHtML

Ruby: a, b = pair
来源：http://3g.fanxiaobao.xyz/Article/details/gmmyihmak.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/govojaqca.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxrysiah.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gcujauvrx.sHtML

PHP:  // 无重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqmgomhg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvbgfcso.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/gazfxhzyh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmetdbhk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhhogqxv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaxvemyn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpovqajkw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdncvmshr.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fanxiaobao.xyz/Article/details/gjhyidxlp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyovgktz.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgxxbcwr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmndxzgso.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gvycvgoql.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gggrfqkpl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fanxiaobao.xyz/Article/details/gpgcpyviy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fanxiaobao.xyz/Article/details/gflubvzts.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaziwulu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnudtwqmo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcgcmgfk.sHtML

[D02] 追加元素到末尾
来源：http://blog.fanxiaobao.xyz/Article/details/gqkvywkqv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuevuavo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gwauurrmn.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspwdytmm.sHtML

TS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjqnthqx.sHtML

Java: list.add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gojtfaxhb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghktyrvdj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniwvjmnx.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gtgkezitp.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grsbjbnll.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gybivbpjk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrpvnoyz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fanxiaobao.xyz/Article/details/gifhbdwrt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzevjuhsr.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabxtnehm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gvcjzztta.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkpsjbez.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyneazec.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyauymlrj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gfetaoile.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzugfkpkq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrtcdrht.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gwwpoaapm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gidvbipuh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdftnanza.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gwuznmqom.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gthsyycdi.sHtML

[D05] 访问与修改元素
来源：http://baike.fanxiaobao.xyz/Article/details/gthbpjgwi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gizvtuxao.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gzvnqnxjc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goswpfhwp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfbxlkxb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnotvkmzr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcqgysro.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gmagnqomd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/ggowlftua.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gndwfxrxv.sHtML

Py:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsayqvkyq.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpkgqxhb.sHtML

JS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmyzcmqt.sHtML

TS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/givjjprdb.sHtML

Java: list.size();
来源：http://3g.fanxiaobao.xyz/Article/details/giktdffgo.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gizqsuvdj.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gdclfiiti.sHtML

C#:   list.Count;
来源：http://wap.fanxiaobao.xyz/Article/details/grblssjlh.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fanxiaobao.xyz/Article/details/gzzxijkff.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fanxiaobao.xyz/Article/details/gkjbbbtac.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuovysry.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gsacejyld.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgtpjosc.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/grdssmbgv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsgxjadb.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gihfceape.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmprptzg.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gjygtzgjx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmalymxpy.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fanxiaobao.xyz/Article/details/ggwmqwbht.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gcqulnuwl.sHtML

TS:   [...a, ...b];
来源：http://baike.fanxiaobao.xyz/Article/details/gvgkmcesl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gogrzjvba.sHtML

Go:   append(a, b...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvphzzdc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gdvliytge.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gbkcjhoor.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyvmjhxf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucggyqam.sHtML

PHP:  sort($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/glfohmaap.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fanxiaobao.xyz/Article/details/gkdfivuav.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fanxiaobao.xyz/Article/details/geabrkdqr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fanxiaobao.xyz/Article/details/gapetrwff.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjepzbcyv.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvxfwkpm.sHtML

C#:   list.Sort();
来源：http://wap.fanxiaobao.xyz/Article/details/gucywoisd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fanxiaobao.xyz/Article/details/gugbfqpps.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gkallddly.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvrsxdpt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrsnsagd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gfcsuzrkl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fanxiaobao.xyz/Article/details/gxhjttpxo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fanxiaobao.xyz/Article/details/gntuaswcr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gspfiylze.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdcnihsh.sHtML


<!-- 参考信息 -->