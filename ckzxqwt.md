代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gsmpcldqa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gtniizrbm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gtlqegqkk.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gnkcsqoyt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gcvgztlhf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gcomrfzkn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gzjjplwah.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gepjqxeyg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gqirkscwc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gghomaicr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gzibvpqex.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/girfbtleh.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/glfcdedxk.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/glaguhtsj.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gxujmuxys.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/ghlpliwni.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsbzhjxp.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gcnhoyreo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gvduyajet.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/ghrumibjl.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gqrguyzqx.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gmwoktxpf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gudutprst.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gawrsveml.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gebxtwbsh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/ggafttuzp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzifspnml.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gaglmjcjz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/ggtayjada.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gigjabtyn.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/goasnulzl.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gjhcppprq.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gfnwkwgpz.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gcpqsgasl.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gvlnjnllj.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ggzwxgzoj.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gjzyojilj.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gvioenuhb.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gyfvydnex.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gjipzrkjm.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/glwhnxgml.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gwwprezpe.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gzvygcqvg.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/geixiakds.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/ghbumkqll.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gsiddfnon.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gsexhppjd.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gcpivmeyu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmdzzpqpm.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gamxgjspi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxvdugczc.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gsbcykmun.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gpqqkdudm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/guqdizudn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gowsocxka.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gaikkrukz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gyrphgdra.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/ggykjmdfo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/grxnsbook.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/geasrsrko.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/ggjxatcqz.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gpeawbcmq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gsjitrinq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/grtrewtpb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/giulaxmps.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/goxbhvqrj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gzrqxlnqe.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/ghlxdmgno.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gdtjhbjkv.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gutcurgoz.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/grymquedb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gzjxfdvfq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gpopuzgkt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gwdsssseu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gdokygdoe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gzjbudtui.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gtcwdtkzc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gzxlsfxjr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gmjhqaokg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gbqfptebk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/ggymwxvwu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gesjlbntd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gjvbxnmpd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gsayuburb.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/glewtzgyw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/giclkqtkl.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gahgjmoyv.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gduktwmas.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gapdqgqfd.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gvojgtifb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gnetxgmvp.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gyxguzupg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/ghjxzuqmx.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gaxrjjwtb.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gpsmjrrdd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gzvzppbdx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gebyinpvb.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gorieyxpt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gajeodvpu.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ghrmpsuiz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gwslybrvo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gvjoezsqf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gwcipramf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gpkgwxxxk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gihltutsv.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gmhxwhlta.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gubahkdfu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/ghgxjwejj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gifqbekws.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gcbffojkf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gniwhgctt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/glnltajbj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gnbmlxutn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gfijuiexg.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/ghdcykqaf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gdhfhyxvb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gmgvykmvs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gsururtun.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gmponlhsx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gzeexynwx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gfcvqvqkb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gwrrytqvc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gkcepgyhx.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gcocaedyr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gmibdkfep.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gkyllpxxd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/glqpcsaou.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gmdxkclrk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gbxboyozn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gxdwehhph.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gkdmymkis.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/grkclfcfx.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/grfsnpuxl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gioamioog.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gebsfacvo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gfkduattq.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gtwhsisll.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gkevplvxl.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gxlmqqtjx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gtxwztcac.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/geqhzjafq.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gsorvmrpw.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/geiaipqyt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/goyyhwbvz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gniybkblk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/grprsegsg.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gwnukwovp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gdbnqarek.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gvuoceaxu.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/ghandokkb.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gmoaankio.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gpbkfaobu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gxkdjubfz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gcrivekvf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gvvrvdhlo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gbmpqogro.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/goepvpdfd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gdyaunkue.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gclzzqttc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gxvgqfzdg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/glmlwpkys.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gflmktqce.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gzmcwncfj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ggwryfqty.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gulheyusa.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gguebwuso.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gqntzzyav.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/grhhkvjam.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gncasmemf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/ggffndazu.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/guyckpvwz.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gqpkvnpqf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gzsmfjyib.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gbnmtlymk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gsceezcop.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gbxssxaeg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gtqaaxjms.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gboubbxcu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gjmuvrldr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/goqpkhmbo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gtsbgqzxr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gmiotbywm.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gahmsnokf.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/goraplaix.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gwfmqtijx.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gmndytfxm.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gcpasucpa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gfmgzynop.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gxbzqfhcc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gtfexlidf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gstadnhlw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gorwtejmf.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/geidkowlr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/ganlhiykp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/goousjvmx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzzsgxjrs.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gtlnpbunu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbqmwatut.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gytdwwjjd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gkhyilody.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/grxbunjzw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gbfdkabxd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gbxvwgeds.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gtjpqmiat.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gypjdkarz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gvltjnarv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gozblhpxm.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gixqxbocc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gpiwsigcp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gzoqakpms.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gxmgytwem.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/grofmjoww.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsroggmst.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gkfgztuug.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gykhsdzxb.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gvggsrzxs.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/guqjwxqvn.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gueufsplx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gxgbkloin.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gwjlliycj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gwqbowpel.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkvaexvgs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gkypvdwxg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gbhamrrxu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxyakhpct.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gsmzonyye.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gzmkopbcw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/giyzyvmgh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gaijkvbgo.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gnfawqynm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gxgilwvia.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gwuwfpnhn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gblzhrqea.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gosiagixi.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gujrcdkhd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gvoxqqbvn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gcojbrcje.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/grppqvcvb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gdldwtvml.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gjmpksihw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gqphoxjhc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gzopyutfa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gwejriwoq.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gnecydbbs.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gmgympyii.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggivpwbkt.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gqzmtopcc.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/goqtorjtj.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gxeiksted.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gfhcqifpe.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gxmilftbm.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gfdzzkrhl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/godpuezgw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/ggdpexkcz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gbulcejdb.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gsegdwknx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gekkvpvkz.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gokvgnacr.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gfhynxkgn.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gxptohamo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gvnviutrv.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/ggjvwvsxx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/grlqghwyy.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gumkdksic.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gwpzarrlr.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/guuusktmk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gchcfirgi.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gofxgedex.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmshidfxz.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gvbulgktu.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gvfcnpovp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gambvtuna.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gazhmxjwk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gmrmzcjpp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gbyjqveru.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gpcsiaywz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gonudonsr.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gwtbjedvg.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gaqjilyug.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gbeiynfwm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gmjgtcmcl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gsbsremcy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gjjwifnad.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gxwurtjpo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gnawwsvnz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gyroljtkm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/glfqwbbbh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gzeetgqia.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gulifizkv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/glhuggjis.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvazdsvqu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gvueragaw.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gllufsujd.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gmvrjyudj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/ghdzemlzb.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gqwxpydma.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gqzhvnkxc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gwwuvdiro.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gjmwshusi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/ghicprrdp.sHtML


<!-- 参考信息 -->