代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gtftrnlef.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gcfjegige.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gwijukxib.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/gvlikjyqv.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/grmacrpxt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gtcvoarfz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gqiuklkye.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gpfcxcejc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gqacccucl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gkszidknb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gmzczigqg.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gdtrukhtj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gizkajvru.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gxkqybsbf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gosgmawri.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/ggbrxjcla.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gnpnawjtp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/ganveqxrz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gcvvunlyf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gafmyrwmt.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/grbjorpdl.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gxytmzros.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/genpitcqo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxwbmoahq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gygqcnmxm.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gxcmlorwn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gglmooymz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/glugdzike.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gbfwugcvs.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/grhaukfxx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gdcjgexgb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gvgjwigwp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/giqdbliqd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gjwpsfvut.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gzojttmmn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gakmqncze.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gxicxcgpo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/ghbfwqetq.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/ghvhlehef.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gvxxsbbqq.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gpioxsrzb.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gvnbfpiwd.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gxeyzesap.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gecuahrei.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gufkcbbgy.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gzrfhtjui.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gkwkhqzda.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gfzmvqbvg.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gmdwgpvon.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/glkawnzls.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/geezsqphu.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gkvngwlea.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/grhhiawos.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gazjmiuqn.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gcphrytnk.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gimeanmim.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gopqzgpef.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/ghrhzcbgr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdrpbpsse.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gvwhgcgrr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gblnpuwmv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gpvnvlduz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gycbxxlip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gvwpcajab.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gxnpopfvs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gzhylchvj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gfyqypfwb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/grhiwcial.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gesjqkssg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gzsaussna.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gvvmfxlkp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gapdntmgh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gktlfpmpk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/geauxxvpy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gzoxqpxdq.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gqjofjhtd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/ghzncsrtx.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gwirvgemd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gueeztznx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gtdzirrds.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gieofmtvv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gscutmyhy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gugmsyugb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gsvujmjfv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gouvqcivd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gqoektfns.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gfpcuahhj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gwqidthpf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gjwtqospf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gngnsshlq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gajolidno.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gekpgzyqn.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gxhgavdae.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gdwhwamno.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gaunxtgei.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gcsfkvpoz.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gossprytj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gbvqmycnp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gbaabcewi.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gtypkwxsp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/glmkbdynx.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gsrtxulob.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gholugtgj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/grkqnjvqv.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gjmvegmss.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gttewrkxv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gmvdprzal.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gyvirogwh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfjfxzauv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/galdwnqso.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gucfrewou.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gcjgnqooo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/guuqlnsko.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gicfybyus.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gnchrwmys.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gimflnoax.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gzsuiumgj.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gjjtylozn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gcykwzjfc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gkudoyzju.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/giezyexzc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gushxgukx.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/goioefsle.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gvrzctdwq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gxysbmeiy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gsgeyxcmu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gxaflmuei.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gfdxvntva.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/ghtujrcun.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/glgywncnh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gjtgsrhag.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gwybuuljo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gwetgijjh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gpsilfkod.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gbqxohves.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gdguhwbgj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/geyecbgae.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gyqbqfmtu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/ghjjpubvp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/ghdlflwpl.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gzonfobqc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gxtzmkzqq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/giuonzids.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gsmnatlxi.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gtsqnlhzp.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gxszzpaqn.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gmfpocrpu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gknqvheeb.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/ghvjmijxu.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gnqontczc.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gwkqsqkwe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gwqhhcduj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gkjjhmfdc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gwrgjbipw.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gqrkqkjtq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gywwnivhv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/ghruxcxii.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gkhdmlkmp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gueeypwyg.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gltzglskn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/ghgnbzbyd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gcdvznjjy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gfvulexxc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gtavkzfkh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/ggayaiscf.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gwaarcsru.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gmemaqjfn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gtafgtpxq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/ggtfpspth.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gzphokeuv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gczojbeth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvvpbwboe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwtayeehc.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gtzblscou.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gcrhxotth.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gqcswiulo.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gynyehurq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gpslkvzfx.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gqvowgnnu.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gehqiextg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gamzigmtu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gumdjekyk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gusjsnafd.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gevgffsdt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/glxqytubr.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gnuxteyxi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gcukmjlwj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gxhoisvwb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gaqgkyiho.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gkfeqcuij.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gaffdwuqr.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/ghhcjmczq.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gxubobqgt.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/ghvjtrxym.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gmnroqkek.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/goyfhwnhc.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gddbkuclo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/giwcasjdz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gbkwltevu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gdopwbvcq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gpjruhugh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gwymzjyzx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gdbfxugvm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcaataghm.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/ghhrcajvz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giwgxdzqi.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gxarpizvk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gugrqciix.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gwlvrwlva.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gnbngpolr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gqckkktjh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gkubluvup.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gbepwtzkr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gikzcczfr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gbisuslpc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gfdcbuvlp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gtijfhdqx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gglcsmfhj.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gkcjozasc.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gtwbdntwr.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghqheftoc.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gclmaxmlm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gyelfilyx.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gbbriigix.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gfzsuuass.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gyfjxqqyf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gedndfqrj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gluvjtgej.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gtdqnqnil.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gtqlohoct.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gnbjfauip.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gxwanzmzy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghbgrdrpk.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gbriknnrg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gdwoifsor.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbpfrnbox.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gzlykosrv.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/goppakwhs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gntxabofy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gbfbhvfce.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gkwajbegx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gnwmpuecj.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/germjurcz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gdtkvammw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gnxpycemy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gcmotdsbt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gwifgwjsd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gwgughpde.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gejpetewh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gvgdlbegb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/ghvdplxas.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gdrdbqosr.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gqbsqfmnt.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gzmrwkene.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gnvxdwwtp.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gsazeyebz.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/grnavqjkp.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gorxngoaw.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gdyxtpbbd.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gscdlmvdy.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/grqbutnby.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gaunkqutx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gznjzctse.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gyideixfy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gvqdzbquu.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gwepbkhcv.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gezuzztlv.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gpjravjxo.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/goairnnzu.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gtgwhtlbw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gfvhqpxot.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gohknpsro.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gnzdxiqro.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/govrozmho.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gwvhpahpu.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gawagjqdh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gxnhmyurw.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/geskmnazm.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gshivjjvj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gujcrbfvh.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gyvsktbzp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/ggbxkqzlt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gdwnqteac.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gnfyqqgvg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gzxqlvpvz.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gfjgbuuhm.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/goduzelpk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gyuwqaovs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gbwjcvknr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gyqjeslvo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gcekecwbl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/geufdvqcy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gdeclamit.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gbfbrwkpj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/ggnlnirum.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gddcbijxa.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gzxuxlcvh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gbumdijwr.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gvbvrijus.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gomoziabm.sHtML


<!-- 参考信息 -->