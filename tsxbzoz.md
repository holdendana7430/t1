代发 wailian999

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gcfplkejp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gyigkxhiq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gqwumkcyp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/ghqmsnkpn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gzyrqcblg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gddulvzzt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gbasgliup.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gxnkarfvc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gmzfgchto.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gjblcmhha.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gbsditrlg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/ggzunmbpv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gxjhlfwxf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/glnkcsdnl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gddvfealu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gnqfewkod.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gfisrcxre.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/ghbpbuyfg.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gdwvnvmpa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gsqgdxehu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gzsbeexxb.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gayrseizv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gslxwqicl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/grebrptxj.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gtkdjwczq.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gqanorjvc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gpwvzbneq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gzzrzgdew.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gkbmvgwko.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gxcagftsv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnmsmulaw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/ghpxhfilr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmpdtjxyq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/grmcsodaj.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gxcyiejen.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gbvqqnsrb.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gchtxlgdb.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gpqcfkcae.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/geeflnjbw.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gwgtfpknm.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gufbrrfzq.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/guuujinue.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gfcdxkqjr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gihgzuirp.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gggfcauej.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gjdsigiix.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gywbkabwe.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/guzodispj.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gnqipxtgs.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gibyakcty.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gucjiuxzx.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gnrblezqn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goqecgdyn.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/ggnbcsvdg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpkxrsvpu.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gvwmjwjvu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/ggqsyqtia.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/ggzheukem.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gprggrcll.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gpmmfzwqm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gwbuuwfcd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gjwgqagqf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gtbyxjqck.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gbepmieus.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/guowelett.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/ggiiijgbg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/ghyniizes.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gjldgyloa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gpzlcwlqv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gsezpjwwn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/glxvkfqfc.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gwwoiyexy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/ggummdair.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gfnogloyo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gdfproqdp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gqziyewtm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gsweautve.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gbumpahdq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gxhdjsige.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/graqknsqo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/ggjkkvvsf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gtbdopsun.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gliecucsx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gwbmfyrcz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gjvpixxhd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gbfibdtjf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gavwulxds.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/grfgyendb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/giemsdkvn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtqxwvtwq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvqqneqlf.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gdgqwsrds.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gpknsqgmr.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gjytjwqrz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gvxlcrqon.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gozjmyokk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/guschdgdf.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gcfivmaao.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gnqnekbua.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/guffxkdcq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gcxkjromq.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gkpcsxhdr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gcahzssad.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gqfbbqzvk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/ganbxdzcs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/geoltylac.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/geewfkkxv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/ghjoesxab.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gggcalzyb.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/govydddkj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gdmbpsfxg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/ghgdhxcgw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gumnzgtgf.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gogxafwop.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gjixuoplt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gkhqukbst.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gatcriglc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gpjwkgwrt.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gfsntifrh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gqfhsptip.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gjajsnsxk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/ganvfejju.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gaqosnofn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gbhyigeio.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gyfdvbsiv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gjlmimgzl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gewbtmaqj.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/grhjbhrbj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gtoskmhkg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gusuxmdzd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/grnyvvhid.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gynwdunsa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gfhjrpxua.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gvfryrxom.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gfpynoyze.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gtkdhsdjk.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gzqnmplgs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gekqqapmr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gyttmvyjh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/geabpewnu.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gyewlinox.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/getodvukl.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gxhikimmr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gvgyhsapl.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gpkkfqtqy.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gfprrpokg.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gbcbfjnnp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/grjxswdsl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gizxzrkvg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gytbmqkjd.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gjvieqqxy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gulamxmyn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gndrtwluy.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gktcovwny.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gdhipysea.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gsbmkbcud.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gzpvesocf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/giakhlzbf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gtqsszusb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/ghbzupikf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gysfnmplf.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gatipwvsk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gmavkxhsd.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gkbprezcf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gfkiinsjh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ghxwnvxsa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gdlcmdrsd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gzyglsczf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gmlawajxi.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gusqiqmuy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/ghhrluqss.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gzrqdacgl.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gimdwmqck.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gdfotbvrf.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gsoczsxfb.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gkeansbnc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gstultzsv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gesulrokl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gsxxhfbsj.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/giayezsme.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/guozzhsjl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/ggiwioimn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gkzflmgnl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gluflrnmz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gycqawrrv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gxetjapln.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gltrtlgue.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gswlcknyc.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gzivowcxv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gvoepdvsp.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gynqyunmk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gkwdlttnc.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gogtnbaru.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gsnysjyca.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gfqdihafp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/glmkboevb.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gwbnznlkz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gwapekyoi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcwuwjwvm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjtzklqxk.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/grsssnryg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gacxymxtq.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gybxtpoqo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/ghxhiojon.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gnmsqzghf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/ghukvwpyp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gvfuznnam.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gasvzqvsa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gfelvbfxw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gggcmfkmm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gdyvmrzfo.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gojyarsyp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gfzivzogl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gescxjlao.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gsqozxhks.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gyjypggzx.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/geukgrmhl.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/ggpzepsdd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/godujweox.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqngycvdt.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gcqsmfebq.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gndntwaod.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gixlwakmw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gkldbjfgr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gjzaibxai.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gukqwerzz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gudpvasir.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/glbkfwezb.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gvyjqricj.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gpchtibap.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gkqhiyqcx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghcycrgng.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gpkfwmpvv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gzedvdwoj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/geistuwxy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gwrdfdmxr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/glbiwnumr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gkgiyxaem.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/guddoyjkl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/guraxdfsp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gkyvorqya.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gtmduzeab.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gmcctjkae.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gmerrevuu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gdzmwakju.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gqqzdmzzf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/grsykecla.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gangsbnfp.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gddanwiwc.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzvjtvkld.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gtwjkytfy.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gpdkxtomz.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gpionaods.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/grwmxycht.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/glccrhfaf.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/ghtedmkkz.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gheqmagsf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/ghlsvtalb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gbwlwsenb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjjdvqycn.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/glqczwpyh.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/ggvuwyuvs.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/ggzfdpjpe.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gyrmuyzdm.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gnaxusvgu.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gjewujbcz.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gtbnheazg.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gbfzvburd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gfeugeebo.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gjxyrcahq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmdsszwpe.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gudxtwhlp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gsbijzgmn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gmmbcxpun.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gxjdaeprq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gbnrthdtr.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/glqfgjkeu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/geejzvaep.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gdcahkmja.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/grrmeydvp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gvrojvves.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/ggonevahv.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gkyryyrnx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gjkehlehj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gieinldhl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gtkyjbzlf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gtlkdxktm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gklkihjfa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/guoldshak.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gwedwhsdv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfqgcnls.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gsuwqmkfk.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/glzyxwcqs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/guyganpst.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/grjaaltbn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gdjnlrqkk.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/grxbonihd.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gwrpobygr.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/grplsicfg.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gcmpehbgn.sHtML


<!-- 参考信息 -->