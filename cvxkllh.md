代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/ghxrxrkbf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gxvgafidi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/ggtxywjzt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gagbckljj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/giivqjvot.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gsmmcyfas.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gcipuxbwb.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gxakrqfgy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gyqpnhovo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gktemgokw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gvneqwmxq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gvmvbudbr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gpohzbivp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gdcfndjaw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gfobtvmou.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/grofyttdy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gbqnfxqky.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gsfiutygt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/govxicuvs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gqpwnxcoj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gvlydbhmw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/ggfzzvqng.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gcsopysqm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/goijraezj.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gnacevojy.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gubasldyn.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/gpmlakwkw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/glcqdzoni.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gfoyqvmxx.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gvykjvehd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gjnmnduzs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/ghaqljfqc.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gjufpzyjr.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gqkkrupdx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gomchpyra.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/guzbzmeec.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/ggemrpims.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gscorfgws.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gzfhfqbot.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gmedwshow.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gvhzakmec.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gfozqcxvr.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/givorhfge.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gblyzzykt.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gdyfxkjlk.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gnodzprow.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gpivuezpl.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gwsqosdli.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gknmanwib.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ghgvtzskv.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gpmdlbrqi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gnaksxaxi.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gkrsrhdks.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gzwizakth.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gqvmdgzpw.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gyjlivxgb.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gdbclnywo.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gpnkahbmb.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gezzjjcdz.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gnbocpnul.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggkybowyo.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gzdnoyjrn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/givibgidk.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gudxnukvb.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gymqydpvc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gmeijnfrs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gczluiikn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gxlhqbakj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/glijkwkmy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gvabyrrqy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gsisbegyi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gbmyayjbq.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gdgmxdeij.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gvnexwmtv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqpsncbgn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghxciobcc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/ggkkrndha.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/glewzqtuy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gobxgecpa.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/grmtqarcz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/glvyegehl.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gefzvwerw.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/glvrwcpai.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gtvqtprtw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gmxjpoauf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/grsyqqwtt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gztafpmhl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/geguuescy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/ggaptgjeu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gmgyxnyzh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gnrnfguzf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/ghmqyypdp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gugfxxtkf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxdvtteqg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/ggmrabsln.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gupxhhjxb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gumxxksel.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gysmydlvh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhbzcnca.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gpywhykfv.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gxmrrvbkk.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gwotrpnjj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gwfmiqlkw.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gccsxdhac.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/guxvdpkeb.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/ggbdxobge.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/guigxzlel.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gysmyqqpo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/graokulpz.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gjggyvywm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gjciphukf.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gpbdoyqep.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gjmibduiv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gbyqbpxwd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gfxeoxmme.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gorsvbipi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/grllvbayi.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gdrzadtaz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/glptusgyx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/godkacotm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gefjwhdqu.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gvgqjqssl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/ghwcgyhjr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gclakcpqr.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gyvgxsvlf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gkfghgmdm.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gjkswfsix.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gtvctucdq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gmhehaunv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/ggechcdpf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gqxwhyymy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gnfmkikeq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gikjfnmko.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gvzabpqpd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gtonygmus.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gdgzfwjqt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/ggfcuslnz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/goycejevd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gbgmwxnkk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gogqfeurb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gehyellut.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gylzigtik.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/ggsnnzggw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gwmfkomub.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gynwpeawt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gfddzdaob.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gyngxecrj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gkbnfdrou.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gmfqmgfhl.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gzzxdoluq.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gfsqbkmpr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gavskucew.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gahoxfoua.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/glhntaoxa.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/glczcgrse.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gglbevlaj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gdvslbjio.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gutpodwtd.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gdaxccexn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/grgwfzjfr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gdrkzfuvl.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gmbmmwrqa.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gljaezyzu.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gljuiziwb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gculluwwl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gzzuoudgy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gmdjakiai.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gmhfsyxuq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/ggzmqzons.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/grvamghoy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gqduydqao.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/giivwlupo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gkbgrtkmu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpusmmyht.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gitsqfrbq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gsyruceau.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gedfvydwd.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gnprhhjyf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/ggybkiyju.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gaxrzaqay.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gyttnuhff.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gqbhgtczh.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gqpdeiugd.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpmrrfwwc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gjuhgknev.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gqytvdevm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/goanrpgjq.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gtcdvghwi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gzecrwpwi.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gpwsyvphn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/ghajxkois.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/ghbczrsdn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gjdxyjmfk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/ghpnerfmu.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/glgfleriz.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gqhpmetrs.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gekwkbulx.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gnwcjahws.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gudszzstw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gmbbpfgsb.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gzftuhmbv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gplmedzxz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/geijntjfn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gidsmkksv.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gqpkjqpyt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gctkkejsc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gzunuljwi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbcxujvew.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gdiqiwjyk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gebszbgwe.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gkxkzbdar.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gmasbajuo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gbilufquz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gxqrvziqm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gyftbesbg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gldfossun.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gtzbsnxjy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gcburddnt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gdbidyexa.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gfoarornd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gvkzfuoic.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/guuotghne.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gcveumyvs.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gwhtcixlo.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gujtwijlb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gizhqqrjv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gpbwsyyja.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gihiucwnm.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gwicpmrtc.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqpwjfrww.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gqcbukobo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gbvotyfvl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gbjkpllod.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gqvnjflzz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gsauwvudu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/ghfdsalct.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gnawcmxmd.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gupbhmlhc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gupxrdzef.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gnijqzymd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/guistktml.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/guelxmmwj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/grpvwkfeo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gfeqejjqn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gqdcfrine.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gaeeelcio.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gksywrmmd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gytyiunai.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/giixpgufc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gotamafvm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gzwznxnux.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gnzpeobvf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gyiapcsiu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gsepgibhy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gfcyaqysn.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gxocdavgw.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gtbroyccc.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/grusigiuh.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gsakfnpnq.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gwnshnneb.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gakqirgvk.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gltplktsy.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gmfhmtyzt.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gwdlugfde.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gjhuioxnz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gaeatmhwy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gpotzobrz.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gobxrwtqg.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gcecsakdf.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/ghowhtiem.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gcvlnulae.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gufxurcbq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gensdohst.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/ganlxdeys.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gibixmtam.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gmvcavhwp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gbwbaicer.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/glwvytntl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gqlzdjary.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gyhosdkce.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gtxrkjntm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gcspjufjz.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gmswlgoru.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gqrwhpxvt.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gytcaqgnd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gbmusecwv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gsohonjem.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gkyjksqpj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gwfibnbay.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/godtpviiq.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gqnwmqeyk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gfwoaewid.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gzzzuwewu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gedqxaoqs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gqphqptrr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gaqigklan.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/glghjvluc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gmpjsawra.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/glzhegqqb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gzzcjaksf.sHtML


<!-- 参考信息 -->