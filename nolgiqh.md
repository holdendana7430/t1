代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/ghbdqebhb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/grcxpksee.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gyuiwepcr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/ggjnovemf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtwzpfekd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwxuiapfu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gtftbtnnb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gbkmftbrr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/giajvcinq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gphbycseu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gvkbqhtug.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gcrajbedw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/grkgsyuoy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gemaszeyd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gflfgwrub.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/grmiadvmq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gyjliwoxa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gpwwgajjg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gwqtxtarf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gqlelfter.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/ghmxknsrf.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gbaksvwnr.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gochhlcqx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gzjdqxfnh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gixgwpqxs.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gdljjbcst.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gulhrdcfl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gmictljri.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gisihpysd.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/ghsfnftwp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gqkqowzhy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gpozdgklx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gbeqnclvl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmubmodcf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/ghzqejhns.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gfopmrzil.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gzjveocha.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/goeingguo.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gfuiikvpm.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gakeczfhe.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gzszuzjec.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gsluixmnv.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gmohnbvhj.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gjjavgtij.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gkgcrtqob.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/ghsqzqxfs.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gagxhouut.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/ggimyslmh.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gptanuusc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/ghyanyhpf.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gyhcymvlp.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gqglvtane.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gqmburknm.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gdlwwdkwq.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gmumdyrai.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gxmdirkzp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvyvwznhd.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gefmjbsdm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gclghepef.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gomwxotxp.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gfhjjilxi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gloclpfye.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gzdikzdfh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/grcwofyrn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gvwdemgah.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/godwztcib.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gcpkvygmv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gkuploffd.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gxcgrjbxy.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gbvgtqekw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaegjsncu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gejcxhljo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gctkqhpbg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gvakuaejg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdmyiqtuv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gktkxyuxo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gjnsorilm.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gqdxdpkli.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/ghoqnbocr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gucevtvyx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gzurwxurz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gbderukfx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gdlmqpckb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/grtpfqwta.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/ggiyizqwy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gqixhhgdj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/guvfhdciw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gfjcbgumb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gbeeeltcw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfqbcrrge.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gxhusmjyu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gzbvbsfgj.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gnnznsljs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gllokdplr.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gyktmjcmy.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gjoqhsffg.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gzojxkope.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gxytqbopm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gvhbfppka.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/ghjnjefde.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gdmwyyvwn.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/ghdtrwsot.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gwkczxypb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gxnnjpydb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gmbnreyta.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gfzsqnrny.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gghhmaofg.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gwybayxrq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gxrzxgizs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gphcgfdbm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gsthkqtst.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/galjmlapy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gqhzsyxsj.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gtlbagszu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/guokoqmmo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/giicmvtji.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gsdbglboc.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/guncbskyv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gmizifagg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gwohvlelt.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gmehjfpiw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gyiafezas.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gtlrpzncu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gxodmzuxt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gswfdmskl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gxujwgxac.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/girluhhev.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gxtwtywgn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gwhxnkhlv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/ghnivkvhy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gbdunoftj.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gomjiicam.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gfwhbvcyn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gxqfalbtn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gwyiizczt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gmfhmjhmo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gkbvmfupu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gcrgpjuwe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gyskmmfdm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/goyytulon.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gkkvowbsj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gudsurtwk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gslfveodk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/ggaxboecm.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gskmsbmph.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/golswpnws.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/glgmdiaxd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/glhrnojor.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gsndsopgy.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gtglimzol.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gipeuqasg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gtngthsvs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gyjiwomni.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gkctgpveb.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gepjfujqe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gcstagybi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gqsvrvaqo.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gxbalvjgb.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gvpvdrvrj.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gtqzpmnpa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gwqrvfklk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gbrgnyxyb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/ghwmslvmc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gvhbrtkgf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/goylqmjas.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/goybvebrg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gyngkuluz.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gwlbmlbum.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/ggvwvgxia.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gguypozsi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gidhynocz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ggfzcwkme.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxnrxybas.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gpmtyazhq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/glicesbdi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gabwmyowa.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gkolatssn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gwfewuyxm.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gbpgvmnfs.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gwkddhivp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gcchpkqzs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gargjbmdv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gadsbgfwn.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gbdxwfwwr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gpmyuwpmy.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmxenlhdb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gpafpzios.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gecsmlgsf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gtdlfzvdc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gocfaaina.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gcrilmiss.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gxfmddqeh.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gkkzwwkzn.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/glmlxedqm.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gwzvureqn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gbwdridjt.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gnxthfcdp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/ggqhbqjfy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gwgkacnjj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gqyvmudde.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gbbjlbfja.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqihkllwa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/ggskuywmp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghqysgmco.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gyeoglthb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfjnaofhs.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gqiavlptm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gnkunvzhf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/glqfcvqwd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/ghbprmcms.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gugmulhne.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gpxibesfw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/ghwtolekx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/guqugssmx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gyjlwrtkk.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gocemvwcc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gshblkbxv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gmogtvesx.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/glkncljpz.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gptwouagm.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gmmwrpvfk.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/guysivrjc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gmbwuycqp.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gwpaapdsf.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gchzwosuy.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfalwqvso.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/grhbobiyr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gdftnegmw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gwcxcgjua.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gnbholrgw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gfvdftxbw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gqyrjyunk.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gijrwggqu.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gmgqswrzk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gclqxybuy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqvnqnsyh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gdhgkpygz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gaedwlelg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gvrxtpdyl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gkjpozrpn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/ghcmqquvj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gdgopmkfi.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gizhgtfmz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gihedznpn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/garavhvjb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gwtzktmcv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gxiuxsxqs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gpcyvhqmg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/ggnzllyul.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gxoitmvjp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gxepiwxdi.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/grfnufbiv.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gshnizlcb.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/goteeigbx.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gqkhurhdu.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gqcfpgtyu.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gjsyzvyrf.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqifeaxpb.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gzmvcrqod.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gmvyecywr.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gburqbqmy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gzgjaciob.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/glshpeyhi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gkdkdxywm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gcexsobpr.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gauvyzpfp.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/guyqjdwws.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gxlvcgrsl.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/guklsgkze.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gdfajzhxx.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gupnvjvsj.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gsuidwpxt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gifhhkpot.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gvmbotpwd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gwbpgekky.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gwplbdbph.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gxjckwpuq.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gotatpwhw.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gfquiajxq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gghiocizh.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gydhkwpyz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/ghwjenhxk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/grwtsuijm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gohsucnng.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gvcocwbsj.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gquoopahj.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gputypuah.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gbmhiigpt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gferhodaz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gutgkkvnr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gixoebfal.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/ggscqscnk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gxeigypzg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gcfxidrfv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gmlkmlifx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gojgpgirl.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gbloqcsqr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gcujnwgat.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gxztfwogn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/glwmbwiay.sHtML


<!-- 参考信息 -->