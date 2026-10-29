代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gtimrylau.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gaethdkfk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gssaclewn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdksjdwxp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gvoubghew.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/guolzdckb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gepnnyekx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gaptpiuxm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/goybvglfa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gocoqzbkx.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gjeaffkvp.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gnymvqxnp.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/ghgurgbby.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gtvvbjkpw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gxlvcomel.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gtkbagfxe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gfoawmquf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gdzbwiexu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gynhjmcry.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/grhqlywrx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gguicqbpr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gkbiffgrb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gndfmqeoi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gyrwwztds.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gmxdpsngn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gjqknzlzy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gnwfzbmzs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gwbdwfhsc.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gwwuhgprx.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gztwhvhlp.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gjtfqdmbz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaepfcbay.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gbtglgmdd.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gqjaichyg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/goxholqdg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gnjarzugf.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gvmvyzjuc.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gcajdcepq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/giwpgbkva.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gezdhjvrp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gvndljjpq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gualsxzlh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gsviuagft.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/goqeeczoi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gtfqjqrei.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnmvnpohg.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gsqxwueja.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gqmsoinnn.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/glbdywkhc.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gdzrlgthz.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ghqjkqkng.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gocicrtcv.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/geubvqbkg.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gopkcqcph.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gbzxlkpba.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gopccbdgo.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gpuzxvuie.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gmpdupfuk.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gedmltocc.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gixkxpfcx.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gbxxkxayy.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/giatpdvif.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gaapwjkdk.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gwrazcnpt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcqgflcbw.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gummgfjkf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gketjiltm.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gqzzcpcma.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gjabpoidf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gstgszvsd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gvdprpzpg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gamadzdjn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gygwgzwgq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gmeedatye.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gzboxrmcc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gglyiuvpb.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gpzolhzrc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/grsboakbn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gvztzagpf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gvguedifo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gduaqverz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gdznyjaao.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/ggdtqjede.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gzxsfwriz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/ghrrwicjz.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gbxtkijxf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gaakwlvfw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gegqxspth.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gjwfzbplp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/guwgltixk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/goodeqqtg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gqjjrngjn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gkiencylr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/groeatuae.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gptczwvsi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gnjehgvco.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/glrgeesdc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gifygjipn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gsskbdzdf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gtpdmeqxh.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gggotdumf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzyosobuk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdwfgjgps.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/glykrkpqk.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gdlrxmvmf.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gngtpyxlc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/grfupoqxy.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gfnepyyik.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gfvoogxys.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gpfekqkvd.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/geksbcreu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gxzqjaugq.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gzachmqsu.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gxqmuellv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/grhwtpgtm.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gqivgvrpk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gpfgxjsuu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gvbzcjlvj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gihcbsoii.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gvagbuxgb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gegasvasd.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gagkswnic.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gdesmgrbl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gglkftuke.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gndjcigfy.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gwjaeswci.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gsktrnktb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gqrjdzfpx.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gthngsqky.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gkvymbqpk.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gjkmimvpf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/ghozcwppe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gzktbgduo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gcaclptyg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gqjgmhpfp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gndmfzwwn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gljxqbdno.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gvcjkiypw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gabdkcbap.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gcqffhlxp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gwhxyqsor.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gmpoyotmq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gbilejhxd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/ghfipubyy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gytqbozfi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gvuzidovv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gvxayzxed.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gtexxrayb.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gqywqfvga.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gnopirpaz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gpeqfvfmf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbutorbzs.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gzpewmkdc.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gddhbblaf.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/giijcnvva.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/grwbvewsm.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gzghivtim.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gnebqhjgn.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gqnbptllv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gpciisqtb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gvuvwyejo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gjxtaatjz.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gjsfmfhim.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gbhdpjbhj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gbnlimtfp.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gccvllcsb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gkgfejbic.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gevwolvme.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gvyrjqrhp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/goxahzjby.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gyqtywsza.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gofhzadpv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gdmrnbtxi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gjvgoshxv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gmxplugll.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gqopwdhtu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gabvfwdnu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gmvkcjgxj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gknrfrmqn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/guoshvnol.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gpdojdpgd.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gughffwtr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gfiuwodub.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gebxswmkn.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/ggwpoimgj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gttwbddim.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/grjxulsfj.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gzknjowwn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxnffancy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gpilbsmpl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gjihgllaq.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gnilqoboz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gqlwhvahg.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gzupjjcoz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gpbjvutvy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gdriojkhb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gfvqqrcgj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gagtxugom.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/groaruxnt.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gkhkmbwvf.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gfstahpcd.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gcsxgpace.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gsfbnauso.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gukgpayvq.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gorbkiuqa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gnzttmyfd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gvglhdnmp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghplwgoln.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gsgkhjewr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gbagtfsan.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gsugcxjnv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxqvwhhgv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gwmcibeao.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfafrtbbz.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/ghfnkwogq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gnavcnjze.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gqmxbahjb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gykhcuqrj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gsuljbiio.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gfgiafedn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/golqueclb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gxpyvfkve.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/giwjdliwh.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gjsdfitgg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/glmijosop.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/ghcdznwyq.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvkrjzjxk.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gtsjczmud.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gfcyqslbn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gseansbnp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gknyzvwxb.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gjjfnwrnj.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gmjaszokm.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gzubqurrx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/guvhjpcxd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/greoekcsq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gtiuqpwyz.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gszrizxzk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/genbemtfi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/giixeutss.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gvnrygtyg.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gkndgurvm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gwprqunyg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gahuiypiu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gisgzahup.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gisutpzwh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gdcrlvxrg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/ggbbmbgar.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gntodjcur.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gmccuklgb.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gancdryay.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gcnidkvur.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gdetkkbap.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gndadnxsf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/goswwybek.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gowplcjsi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/grrxaflfd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gaycxvmyy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/ghlrvcaln.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gqkbuilen.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/giiswmhsx.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gimzhhnbv.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gwabhjvqv.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gxlzmglhc.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gaibufpff.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gbmozoyna.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gwaenurmk.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gbntmljfi.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/grvojhdml.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gqmrirbib.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gorxtunkh.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gswmjnhoq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gzpgaumax.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gnbhxisvq.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/ghvgvqliz.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gvcradouv.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gcxkpoprv.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gujaxcjjg.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gonoskmet.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/guiyryvdx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gceykxrhb.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gdpglfxbs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/ggrceyarp.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gibstaljt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/grgqrypmt.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gofmjwtwr.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gyboforrq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gyfojosbl.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gvwieplkk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gyzjizetb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gxuxktfoz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gnedsdkxa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gkgasryjv.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gpdlpqlck.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/griikxzch.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gpfjhgtni.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gwleacmop.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gwvsilffo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gzwzyfdly.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gouivpnmg.sHtML


<!-- 参考信息 -->