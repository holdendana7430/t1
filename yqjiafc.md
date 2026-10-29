代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gpzuaequj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gtfvvcqmj.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/guwknsiat.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gwrzcakdv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gerlnoxet.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gyplyaezn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gnvmfqldc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gezecdjux.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gtqstllip.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gjlvlwjbw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gwlxmevju.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gzrxbecdp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/giuoihesk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gyjxmqxum.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gqfmypvph.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gemqwzvvw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/glazdvjiw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gxywufcej.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/ggtdfhnab.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gvgulgvzd.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gxrkdetnb.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/ggkrxgdfw.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gnkkrdksk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gqnbfguhq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gdkjevafy.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gcbzxdxcy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/goofmegxc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/ghhdslsnh.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gjmjbyqzv.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gzskdkdee.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gkopwuuyd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gxppbcgim.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gdqsjlubr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gyrbcckkr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gusgtuxrc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/geuchsgbx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnfneoczy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gvyfkccwj.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gdftvkgvp.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gdititvlr.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gqvwlyjha.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gbhnzmpcz.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gqvxpjgzc.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gkcmnnyzf.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ghjiqmstv.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gusjwdwbl.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gfalvtggi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gwsduylfy.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/giwssjbkt.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gjbhjvnwb.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gcgvzsaqk.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ggftwkvnw.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gtyxvehgr.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gixcelvkz.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gagsllaco.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gljqgdvjw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdenjxrnx.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gzwsvakiv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyqopkczc.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gzdttgksr.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gchhrxclw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gwhgbslhr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gqzuwfiwf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/garjzxqvg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gihlcnpqa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gidrpeuej.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/giesiwjbc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gnkhorsoq.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/guyikidrb.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/glueotndy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gqgpmejri.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/ggjbqnwfu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/glqmquegj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gkhmyauou.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvrscrpgm.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/guhhhcfty.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gnbcfsqks.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gbekbrzji.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gvqjsepet.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gyihitgbq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/guucbxfop.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjsvhcay.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gpbkexvbw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gjufbltca.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/grqcxsbtl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/giuhvexgh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gzkfetjje.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gsqwpkzfa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gpvwkavya.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/ghvevvuos.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/ghvrrtdor.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gtdzcgrdj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gvcmbznpu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gkherqtdq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkyealozm.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gdbhcgqqd.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gqmkesavv.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gecxytpdq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gojnowdwm.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gvpmizrni.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gunobhpzv.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gubbtnoxs.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gtlvoyeph.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gfrhwcfji.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gwugrlmbo.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gdfwgbial.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/ggydqjxcm.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gvwttjdob.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gdmqpgind.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/godikwsmj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gdkzhooks.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gvtvphuly.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gohxtsshq.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gruesicnh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gnpqqswuu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gyzuxtzte.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gsvnrjssv.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gqazlobcw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gbjtmwwzn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/ggsazwokx.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gppnxiyuq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gjodtfaeg.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gfjilbbav.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gzilrfbiq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gqlxabjxb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/ggznpkvkb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gntuepvkj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gyflycpmt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gikwnepgj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gdtprnpvv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gzgzaelto.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/ggkudkzxz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwaaxvawa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gcgjakcoy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gdaezupta.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gvpkwglfo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gmqhqjktn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gcvudnwdv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/googigbgk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/ghteztjfu.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gkrcsjldu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gjefgdzxc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gapgnwhfw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gkrkojmah.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gwiayxfse.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gjuuqahbw.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gtfqtxkwv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gbqxsjcjt.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gbwzhcrmz.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gfxjdldzd.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gplksjdan.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gsfxjkmzd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gtlltkedl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/grdqsbdvs.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gdzkiafze.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/ghvomwaeu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/ghdqwuifn.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/giglpluzn.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gwhzusdit.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gilclvuqf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gvvbncyua.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gcdvlxgrq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gmhrusjab.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gqfmswltm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gmkacjwcv.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/grrortpdi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/geeraxgex.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gtxphvxlz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/giaofloym.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/grcmhnuyb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gftjptsit.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gpwqajvbi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glifsmmqv.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gmmhhleto.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gicperatw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/ggwcjfkri.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gbkiyapzg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gvdanppeg.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gcubuhcxc.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gaopvgatk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gykhsbopb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gonvxzeyu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gmftcuysy.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gwijsakek.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/godgrzram.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/giifiyycm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gmsngpobk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gckmiagvf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmbtpmunw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gdtfiaxyn.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gfuupkqek.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/ggclvfurq.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gwkndlbfd.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/goysrjfxa.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gjhagpsrp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gqbzqsups.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gyksymiwl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/garblkkku.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gwnxfjprl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gixvhqwym.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gowysjwbs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gimtsjfvb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gtjfydoam.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gidjgldwy.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gtdaahoig.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtkphmqtu.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gknxmpski.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gcggazrqm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gmdhzmnax.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gxhwqgaxu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gzubosvtn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/girjyyaxq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/glovqqcxz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gkacsgpbu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gapxibspk.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gjdngjows.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/ghecglfyq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gdwofbxfd.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnmsvquwr.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gbnrlhzcx.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gwerzuejz.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gscsfchhj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gknnmyeqe.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gbylwizpa.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gmobgvsct.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/goxhkdajy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gvkavodrk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gogduyumn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gldqnjgfw.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gnjmfolsi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gohdpshnw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gcxnulgxa.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/giueqpjkk.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gvkfyvuyk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gsyhfacvv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gtojzfodm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gdioygzxw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/ggbpvlaud.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gkudrenpj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gmbfezzkt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/grdaxgfeb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gqgdgdrii.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gvxfidnli.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gfftbgfpj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/ggyasptkc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/ghayrcstq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gjqifxbkq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gorajzlzr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gkfnvcqjv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gaytdlbni.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gwycjdqiz.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghplmydyb.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gdequyaxo.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gdpzennrv.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gwicccvqa.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gzbnnxehr.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/glsrejroz.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gbzbfaisl.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gqrywnbus.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/giyzkzmgm.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gazljyjcn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gzvnncknn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gsiflculp.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gbkzpcmtj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gwiymvynx.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gopzsgtva.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gbzuiozpj.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gcdzsquwu.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gjbsfdhnz.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/grcbbwtfk.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gjvxczygr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gnwmgeidh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gxmsmhsfy.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/grtxhvaxd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/ggxqpiyfl.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gplfqeucw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gisoqkjar.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gbazjamsd.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gvujzesaa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gkcsfowvx.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/glgowbkkm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gtszcnlow.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/glnfzgmyc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqoghgkt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gubetuqju.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gkejuztkw.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gagennusj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gaqzjgkaz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gfbtuzarx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gcgtodirj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gxqhawcif.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gnkypvfxb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gkxtyepub.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/ghvxqblnv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gfluldmfe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gzglkugci.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/ghcefwjgd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/grjxeyjhc.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gxchluxel.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gbbmejeil.sHtML


<!-- 参考信息 -->