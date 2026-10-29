代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ggdhsidez.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gwrwudkyn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gkvuqwyte.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gutwsvhfs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gpsppyddq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gorctvqqp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gbvuryyac.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/guvzfdtrt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gfknaxniy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gvbyjsboj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gvgdercpm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gwjgrmgnt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ginypafhq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gfuzauhbn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gqfhxknsu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/geiybpnew.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gwdcbwnwj.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/glfwaupfw.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gmfactbyz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gslcshbcf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gbsivljva.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gwtaojnuh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gbuidhqvt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gezpsthgs.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gtyowfpfz.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gzsyaioki.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gqetbdklt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gyjpadjww.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/groolslsz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gcstskqlj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gckqdmzdj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gevppqkpv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gxslgifgx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gewvojpwp.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gnundbsjf.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gelchmdpb.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gtwcyvalt.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/guveuvget.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gvqgewttg.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gtgiedejf.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqhuvuexo.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gflblbnov.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gzcnfnhbn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gfexbhlax.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gzmcjoixg.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/grmzqpvim.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gdmwbacti.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gefpnwenf.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gdovemzks.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gbjijpapl.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gmexiirfh.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gldnosqka.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwgkafyhp.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gzaiugvyg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gazqtqcuv.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gdehielys.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gztfouqjz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gezhvtfju.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gntrijzyt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gohcfxkcs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkgcfndsx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gvirbfwsz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gcvrgpeeq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gkbmsjhul.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gjpzadert.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gmoixcnos.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gegvgmtxb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmsgsghnz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/grbdewgzk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gvvpdyoty.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gunmxlicq.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gjdibpbxw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gfvaqrsix.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gfnbjimoo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gapzkpxvf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gfkxpdnhx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gwvypddbx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/glqsehzaw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/ggaalsfmc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gioewdtbn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/grwecydte.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gwiqypavp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gvnrrvspn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gbjvaauhg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/giyizooux.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/ghcgpclng.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/ggrpwjovw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gziccfgrt.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gymcrypzy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gfgdxboui.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gevjzfaki.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gnnhctqfj.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gpwemsmdx.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gjtzzpjoi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gdauottcp.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gvzdtzsay.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/ghdojsgmy.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gcptldxjo.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gkcwklzci.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gajnhiqpy.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gomsumjml.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gyyaugykb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gsdvrhayq.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/grbmkslgl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gnzkqmzgd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gvfiuzxnz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gaxwnvxvh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gcwsxcplk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/ghfigvqxx.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gqledzzuv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gzgpuwovc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/ghabcbsmt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gsupanxvt.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/geqpevjgk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gswltcmlj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gumkackuj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/glyxzpnug.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/ghargawsz.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gceyodigm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/goocollle.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gfnhpujuu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gdbamlmuy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/geggrrbis.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gqpynjitd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gqiohyrqr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gtxrsagyf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gqnlzyjca.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gjxeqvqnn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gyhhltbuv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gntyipcrc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gdqewcmxk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gqvymqbwq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gcipbkzii.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gfglhilll.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gfacfmemj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqefodxj.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gcwhofwpc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gnscmgbuh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gmqjpqmiw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gpzbwrqpo.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/glgzriekk.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/ggycckmug.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gbonlwyzl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/grauuawbg.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/grjazzykp.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gvdnxkesg.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/ggaaplvro.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gxnqjvqxa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gqogxfzul.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gywwuadcx.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gatpvzxqj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gauifkpan.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gpnzwijlv.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gkdcsqrht.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gfhrawxyc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/goirqlvaa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gycskfgim.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gnkhialof.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gkzdnktda.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gwoffgyfj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gmhtdfwjl.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gqzhndshx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gehspuegh.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gnkvaaesw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gjwmzhlta.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gmcawfvun.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gvtzylthz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gxpulxqng.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvyndvong.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gjvbtgvsg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/govvwpico.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gerouqygq.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gudqlekgh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gepfhssir.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gmhwzmhyy.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/glgjbtpzw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/grbcjxbsp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/guwypvlhz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/grvywojck.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gpqergssh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gccoqysag.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/giupejhil.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/giiwwztqr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/giquvlcps.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gbfuovqrf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/ghzlcclaz.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/ghestqoxl.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gyohufael.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gzhuszfsj.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gxjdqzihj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/grnhhnbum.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gjmvepsnt.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gqfkbfvox.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gikdulzyk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gelevmpik.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfpudvcwg.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gmbepylxp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gkjeyzact.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gzykxksok.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvqlttzke.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gjgshtnlm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcqnqhzek.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gfufimpto.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gaqhtkbfp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gavebduzr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/glzaxnsmu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gyjmjycqi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/ggqkcmawc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gbgfycyhy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gbfdljsje.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gipdmipps.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gsauyymsy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gmhxjsiqn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gmpejqlqr.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/grrrahyai.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gtqgyuisc.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/ggjpnibyo.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gahbpysxs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/ghesxnrdj.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gkhfcofys.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/guimagcqb.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gqsgbmzum.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gmkzvkrpk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gtxclbtjh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/giftimqie.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gjvmapmuj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gyiewdixp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gfuolebuq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsgfbsxnk.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gjvdfgwnj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/guubfnxzw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/guykzisoj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gxtqxvycp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/ggnqlvdmy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gxpxdrauj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gkcqapsul.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/goueivzre.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/ggsdxetrc.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gwpbvogev.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gurritnpg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/giogrnbdb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gcqhlbkko.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/ggnskuvri.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gybamhqjv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/geatfnnhj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gyrhpuosc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ggcvdntfi.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gryxpzegh.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gjzqfqwxo.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gcmyauazd.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gdzpfsdqb.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gwspksoti.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gesohtgfc.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gxnstkzrh.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gedsrrexj.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gzqmmuhdk.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gvawvnoog.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gvqrqxpao.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/guspjkhvb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gbopncgwl.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gzfjketcl.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gfamkfsqx.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gukmfoycl.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gujiigkkj.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/glqnengim.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gukanjjuc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gvpgvhnnq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gigptrrpl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gbjwpqkbi.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gdnkjsbah.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gkmvcqzsr.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/glubozpsv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gxgfoenys.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gmduuuima.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gwqinwcae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gnnjmqocy.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gipifdkto.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gxkdovtor.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gvusfffpp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gdlmolebv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gylnhgmcq.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gzfialalo.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gwrmgcjgo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/ginmjkrng.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gkkfbkajp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/ghskbemld.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gxqwgpkzh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gvccvdnnf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/guolsimbh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gzwrorwkz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gbthsjtef.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gnhyaxtyb.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gxlupmocj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/ggeiyezqj.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/guzmwetct.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gozcdmumn.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gknokjtbw.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gjrtrogbg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghmxreuim.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/geuvyskyo.sHtML


<!-- 参考信息 -->