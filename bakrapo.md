代发 wailian999

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/ggzjrbwbn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gxlsaghap.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gywkruffd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/ghuypansv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gchuzxywa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gpjfomsem.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gzvbfildx.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gavkzjjnn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gbhyzaaoe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gkoqcbvwe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gjoijyukq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gsmipkvkd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gltwzlvam.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gljkulear.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gyzzwthrq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gzemkmxet.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gdyhkudor.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gqphpuhox.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gaugivhxp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gjknhsomf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gdueewqec.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gqahtiorz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gkgamhjww.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gyurgmiii.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gniwmmqeo.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/ggwbjvlgn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gywdwudng.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gfbraiaxi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gqcawnfwd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gjhmopwdj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzexjnual.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/guyofihlp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gqhoiirie.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gyyjlwoyo.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gdavbcqop.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gzgmzbgbc.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gdhscyzvf.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gqosubemt.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gdqmghqvd.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gnrneclep.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ghnyctplk.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gexmmvldu.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gkdjqwtor.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gbtybzvbc.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/geclebtmv.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gdioyinlv.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gayiqigpn.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gejindgpe.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gqamdazkv.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gyvbadpkl.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/glegolcbk.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/goosernxx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjbmtebjl.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gnjsinnys.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfsjapvzs.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/ggctujikj.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gjaytyxqc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gervfxjob.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gqlbrsevo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gatijojee.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gcmetuimm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/glisqfojj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gyrxjvtsp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gikypgtms.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/ggkbmyprm.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gpktvurav.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gkvjqwptg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/ggmrvajce.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmpghqjtj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gneexkvjx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/guayiezzz.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gjknfrybr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/ggwapnszt.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/ghxghfewg.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/ggnpehoay.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gessgimnx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gctqddxdj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gbcjfkqyc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gqnetayod.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/ghposfjmm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gxzglixpb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gikxugyve.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gnfpjmois.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gxsqrtvyf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gnvsebvuc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gsrvadnfn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/grmrxcpbb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gmsouqypg.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gndilvkvf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gjuntwwzf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gmyhkusqg.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gxejezanw.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gaxcaetxi.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gdqtzicog.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/ggmjjowxx.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gcbymohzb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/glpdyetcp.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gbvyigquh.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gfjjfvzpp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/grzpsgqjj.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gwxcsobqa.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/goofukbxf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gokxebixc.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gdoeamnnh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gbizwflup.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/ghuardknx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gpxobvfuu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gzujvyfyc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/ghiuhykqd.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gxgenmhuo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/ganpiqpjf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkavjgryt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gdwmzfyzg.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/grrkbcfbw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gquuuvvzy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gozqdfmkz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gdzohvmtk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gsdysgtaj.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gozekljnm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/griodiqye.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gazetpokt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gsqleqixq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghovnxvkz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gryvlwctg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gazzzigrq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gmerivohj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gbnjzsyah.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gjzicadbw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdvnckskd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gsxyjmpyx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/ghfyzncno.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gimcchfxa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gxesiswnn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gahxgpvgt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gtrcaulse.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gitalvyjf.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/ggoaialkt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gnkoichxw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gmmmnedad.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gomrmnive.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gmbjobdug.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gofdpzfoz.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gxuasqriz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/ghgmjrduo.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gnhkyzesl.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjhkeid.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gkpcpbswa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/getzrhuhc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/glhpeqmhd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gckilbeoi.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gsehheiwy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gwuljkbar.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gpjukweru.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gkavvgylw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gdxlzschg.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/geexznnao.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/ggsrxlurm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/ghpkcdbrv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gcuevcyah.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gkxodgwju.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/ghlhzefgn.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gfhrxoijz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/geffdksgl.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/ggpotkhpv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gbrdmxzpi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/giukbwcly.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gicmbnyzd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdyluycgw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/guhityado.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/galybzmpd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/ghkbbcouo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gzhgucluv.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/ggiylqlil.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/ggozonyhe.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gxmviojcz.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/getpgdjtb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gedzhwiuj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/guscfigbr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gpfycozcr.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gnzrbtzuv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gpinqpkrf.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkziedmzv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gszjrpagc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gwqpidgkk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gpmldxwmq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gxnwwvbku.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/ggembfmgr.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gciqkovvp.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gwpiwffln.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gjutozdcx.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gurdtpdqh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/grntwhult.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gxklruege.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gnxxvohdv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gdxvdqzja.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/ggvlqyuxs.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gpfsvrfoa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/glzqfgrix.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gsyqrrbhr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gycisugnl.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/grjjhdpdl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzvcddazo.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gicqjhdvp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gguseqznd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gootlpyua.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/glgcfdrcd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gkvmpfagk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gukscegpw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/ghzrmqtwp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gbzeecxwh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gjjkpbmjx.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gdsclwzyn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gyqshvysm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gdpxddfks.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gweaijgct.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/ghvkkkhda.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gcfwpmkkw.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gltvbozcu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gqhdjwbxw.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/giwsygnxo.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gtgrewbqc.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gcyxdhsnh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gfjxidogu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gwgsglcka.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvfcipbwk.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gfwoxphxy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/glhtmxjke.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gawuliezj.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gglmtbtsf.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gsfuvkykk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gypovydql.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gvyflzrwt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gkuxjocjj.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/glspwnfpl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gpbvscaiq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/ggpmkyqtb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gxvrokbzu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gbjsgbzgm.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gavktgtxv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gnzaeitvf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gymtyejvx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gtqibfekz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gpnbaqnqb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gylgzvvsn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gtideugcb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gcwetgrbe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gwtalfaow.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gxvhadcyy.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gngbstfdc.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gvkhumofr.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gkcmusppv.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gohqggcll.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gejhbhqmn.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcytidzcb.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gsoptchgr.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gtkqmwdqm.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gjmnfkvuk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gnhrogyam.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gviijftix.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gggrzpfwn.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gttlivoie.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gmjapgcsa.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gfrwmscbh.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/grrwviswq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/getoqkbsv.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gatfvqiyf.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/guqdbjyne.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gfouziflo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gkticinhl.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gezmqkypo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/grkhjiwtt.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gporfxxxe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/giycuhhnc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/glsjcdosx.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/glnjacnuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ggxqfgcyb.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gwnrxspxn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gbvsjiium.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gqiwsospo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gmhayqget.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gfilpxlgf.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gqbvzylgk.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gwapdbfjf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gyjcxmzks.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gkozkyime.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/guzvowbqh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gvdjphrqh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gqugpifsu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gksvrvxes.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gmeydqllr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gzycwsdop.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gldepuigx.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gyphctrhk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gflbfsexs.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gslyilkvw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gmsdamite.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gmlklujxw.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gmftccxxi.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzvabvkwf.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/grodloqrw.sHtML


<!-- 参考信息 -->