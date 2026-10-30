代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnyzsfmm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/goxsprolc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gssoeijuc.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/getsktrml.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjjjogws.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gplsgcjgt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gwmshcidb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gpkkiqkbx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gkhjzonsu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gppnvxjbj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwoewdgd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjxwdktw.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusjpdald.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fanxiaobao.xyz/Article/details/gindzjcix.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghagwxett.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/guxpplvsm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdphmbxg.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcdybpzj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwxlirvb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzumoyhwy.sHtML

C#:   x is int or double or decimal
来源：http://3g.fanxiaobao.xyz/Article/details/gjceptsqs.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/gokthkqod.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fanxiaobao.xyz/Article/details/glzfqirng.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fanxiaobao.xyz/Article/details/givmkoeyr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhjcxayc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gfcsbdrmu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkfyrmwq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gevvdtzvk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/goemnkqps.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyguhqdr.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/gftxjptnj.sHtML

Py:   a and b or not c
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkialego.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fanxiaobao.xyz/Article/details/geenpotrj.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyghxzga.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gedwbjumr.sHtML

Java: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gjizcdhtc.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpynxffs.sHtML

Ruby: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gthekumqm.sHtML

C#:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gledvrcow.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goraojzqu.sHtML

Py:   if not data: return
来源：http://baike.fanxiaobao.xyz/Article/details/gseymtqui.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fanxiaobao.xyz/Article/details/gslrljacu.sHtML

JS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gyarwplnd.sHtML

TS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gswzwpvmn.sHtML

Java: if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlvmvkok.sHtML

Go:   if data == nil { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gibvvccpc.sHtML

Ruby: return if data.nil?
来源：http://m.share.fanxiaobao.xyz/Article/details/gijrvjxai.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gkycjdwly.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqjwtkoe.sHtML

C. 函数与作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gzilxvawg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gedwokuli.sHtML

[C01] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwdpexxz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjutsguc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyaczrjqa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxacqxcxv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjteqgoel.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gicbzgjpq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gwdrjfiuk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnttqgzvv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/geaachxqp.sHtML

[C02] 默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/grfemxuqs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsklphtw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmnugukjv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/glgpbdmxm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guziomieo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gsotxlimd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbddmavvf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftaofsgt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrxmetgg.sHtML

[C03] 可变参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrzueenm.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/guzbtrmfb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkzbyxhg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfkschuiy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqogcoior.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfrgezxe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fanxiaobao.xyz/Article/details/glmjdoyhe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gpwayrxsn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gosamoihb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmyhlqfye.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxhvrkmx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawvtgaqe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpavjccph.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnchyyzkl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdugvlty.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghcjooyrh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwlglruq.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpjrxsrjq.sHtML

[C05] 返回多个值
来源：http://baike.fanxiaobao.xyz/Article/details/gzxuofojx.sHtML

Py:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gotcbpyqp.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqefqgjt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/gvxnqmveq.sHtML

TS:   return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/gixrhdbli.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/gtpdhphjf.sHtML

Go:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gejfqawgh.sHtML

Ruby: return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsntylxjp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzswuyybd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwlbvwtl.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwksiyyxc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fanxiaobao.xyz/Article/details/gquajyriv.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gmtwvqzqp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gtjjjvsjs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gquttklpq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbwvwcub.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/ghbvgcrdt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gffzehvqv.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjshxwai.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyetamuyy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gztykbneo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/gnecckcce.sHtML

TS:   arr.map(String)
来源：http://mobile.fanxiaobao.xyz/Article/details/gayqozzhp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gpopvudnx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhjnrhrp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrkhgxez.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fanxiaobao.xyz/Article/details/gstespant.sHtML

[C08] 闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gcamewtgm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fanxiaobao.xyz/Article/details/gqjgycagu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvolgwxwy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpogiutnh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcjapfbao.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbimouww.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnddxvmmp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyweyquk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzswtxubf.sHtML

[C09] 递归
来源：http://blog.fanxiaobao.xyz/Article/details/gkcxzvrni.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkolihrrg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gopujjwac.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gnfdszvuo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gbqmaseyj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkypvcyqx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuzjgjqa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwnvlfqaj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbejhixk.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/goqehtrpn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fanxiaobao.xyz/Article/details/gmsfphzjm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fanxiaobao.xyz/Article/details/gzpxhjvid.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gumzbkmmm.sHtML

TS:   同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gwhcfyxzq.sHtML

Java: 方法内为块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gsmygqpvr.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gcumgfzhz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/gjakdygcx.sHtML

C#:   块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gljucplnv.sHtML

[C11] 模块导入与导出
来源：http://baike.fanxiaobao.xyz/Article/details/gzbgdqtia.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gzwofxxhj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsikwsdy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcankyte.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fanxiaobao.xyz/Article/details/gpubkette.sHtML

Java: import java.util.List;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrcklmhu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpstfbgdr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fanxiaobao.xyz/Article/details/gfzzunxax.sHtML

C#:   using System.Text;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdyfflon.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsxfdpil.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/gkblvrmsz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoowdpzz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gteuvkndb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexfwdtmp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fanxiaobao.xyz/Article/details/grbwdphsi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgqxnujn.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fanxiaobao.xyz/Article/details/gplgpctqm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvzlfismj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrhxjunn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gwppayjxj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glflratzw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiqpnmft.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geboypyev.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzgtupri.sHtML

Go:   func add(a, b int) int
来源：http://3g.fanxiaobao.xyz/Article/details/ggbutovvz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fanxiaobao.xyz/Article/details/gubmutmpf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyqjfttp.sHtML

[C14] 泛型函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqsscjez.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fanxiaobao.xyz/Article/details/goqnbnfqa.sHtML

PHP:  // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmetaevt.sHtML

JS:   // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gvcxzkerv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzqdmygze.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmjzcspdw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcntxdcsx.sHtML

Ruby: # 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdciqkft.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gfttioibq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fanxiaobao.xyz/Article/details/gucmjapke.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxinvwooy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gprdequjb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoqeylbp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/goybyyuro.sHtML

Java: // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/grtixgkph.sHtML

Go:   // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqorbgqsi.sHtML

Ruby: a, b = pair
来源：http://baike.fanxiaobao.xyz/Article/details/gjzuczivm.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gxxjpzlom.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fanxiaobao.xyz/Article/details/gqqesogms.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxtuccey.sHtML

PHP:  // 无重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavnyjszd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gdrdhlzmr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/gicizfuvn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhsynmwb.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fanxiaobao.xyz/Article/details/gkwsrtxzd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqdjuiie.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxxucjymx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzuasgat.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fanxiaobao.xyz/Article/details/gusmlyans.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gowznhpft.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxgqvmpb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fanxiaobao.xyz/Article/details/guxmoahrq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcwopqyp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/guboxemqj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/geiwdkric.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcoxtvuu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/gmvgjfhxm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/gyjuzmyzg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fanxiaobao.xyz/Article/details/gnziijwqe.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/gukfvyyxy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fanxiaobao.xyz/Article/details/gdhselsuf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/glvrkndjv.sHtML

JS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gdpgttdat.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gohfhwepg.sHtML

Java: list.add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfogifupj.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/ggvloosbg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaptqaqgu.sHtML

C#:   list.Add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwhdyqcgc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gywohzrlt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilbijxrt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvpcbucs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwpxczek.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gbzwdmmic.sHtML

Java: list.add(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gzgxtucfi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsbtmndu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxyskruz.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiebritj.sHtML

[D04] 删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gejfemuuo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrpaaeow.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gjrtlriag.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fanxiaobao.xyz/Article/details/gkbldanby.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gxnzmmkqn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/grqgbhgok.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjulkiire.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fanxiaobao.xyz/Article/details/goqjlqiag.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaofwajs.sHtML

[D05] 访问与修改元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxzrpdoga.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gkjfsunjc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyjhrojs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjapnejhb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guadbfhyb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/gcxpsiicz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gtnhhlaxh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahvckqsx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfikucse.sHtML

[D06] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ginkperii.sHtML

Py:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojovnnno.sHtML

PHP:  count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnmzqnvq.sHtML

JS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/gusisxhae.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmftgbkea.sHtML

Java: list.size();
来源：http://www.share.fanxiaobao.xyz/Article/details/gidzqlrgo.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gdguysjiw.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdpumoym.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwywijcn.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fanxiaobao.xyz/Article/details/gmtgmvreh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fanxiaobao.xyz/Article/details/gsscwkdwd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkezhfdef.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gyliqlpmd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgsmkmul.sHtML

Java: list.subList(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gxzcsnuja.sHtML

Go:   arr[1:4]
来源：http://3g.fanxiaobao.xyz/Article/details/ghqxxsoln.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzzycmvp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmevxplzf.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhuvnqti.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkjorjto.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdzazvvu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtmgoxfn.sHtML

TS:   [...a, ...b];
来源：http://3g.fanxiaobao.xyz/Article/details/gurdlttex.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccthtjxe.sHtML

Go:   append(a, b...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwrnzpid.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghodvfxsl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/groungcgj.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddgupncw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/glummmnrt.sHtML

PHP:  sort($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzgibtih.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fanxiaobao.xyz/Article/details/gagwjmoor.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fanxiaobao.xyz/Article/details/gtdjyeawh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmewkukxc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gahjobsfw.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gpvfzyyrq.sHtML

C#:   list.Sort();
来源：http://wap.fanxiaobao.xyz/Article/details/gxquqkxoq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fanxiaobao.xyz/Article/details/gwykgiqrk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdngrcmhj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gjnkoxxeo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fanxiaobao.xyz/Article/details/gclkhaauf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gvryjxzlz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjmbvzcl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fanxiaobao.xyz/Article/details/glomkycpw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fanxiaobao.xyz/Article/details/gzgdgqzfm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyzzjiwa.sHtML

[D11] 反转数组
来源：http://baike.fanxiaobao.xyz/Article/details/gdvtchvap.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrvfhdsl.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpttcdiz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fanxiaobao.xyz/Article/details/gptqhbpcz.sHtML

TS:   [...arr].reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gpxkgyjej.sHtML

Java: Collections.reverse(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gdijdufeb.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gciewdqos.sHtML

Ruby: arr.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvrkodbo.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntcajnqf.sHtML

[D12] 查找元素下标
来源：http://3g.fanxiaobao.xyz/Article/details/gnfqzfymo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbijgzkxe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gzmrecdbc.sHtML


<!-- 参考信息 -->