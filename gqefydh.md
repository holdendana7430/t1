代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gdieywaqz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gvptjqoll.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gxzzgdfcd.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/gxdqqohze.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/ganduband.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gfnlnjiso.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/ghgjrlttp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqrwywqol.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gcikxqzgl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gltafydra.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gkjskpumj.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gxbzuqbvu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gbcjqxopi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gkoljhnjn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/ggibcwcub.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gwvdshzzq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gxqieewes.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/glbwivtaa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gdasuguxf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gmnzpjtvt.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gouvpfbmp.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/geizalqgl.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/gfqeamdrm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/ghxfheygm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gqjhpeccw.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gmoqisztc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gdekwhupk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gqosenjyu.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gqczyimnh.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/ghmvqirde.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/ghmyfstxg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gtyqhzubn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/glbmdyvwe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gsibyajbp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gzfhhnqwm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gycopymke.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gyshnoztu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gufqakuei.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/golnnbjid.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gikkhecuu.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gxhffqrdt.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqbarobje.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gdjquzxym.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gyoxpvzon.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzlmwscck.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/guzswiuwp.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ggcybsmer.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/ggtenmrtl.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gqooehouy.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/giyykyykr.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gqlzqttjz.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/guvfwgrmv.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gazoeymiy.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gwufrczyr.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gxnuyxbip.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gqhxnrnrm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxztnsmjf.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gxriapalm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsgbynuqh.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gfycjthgu.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gdnuppsbt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gsmwufcyv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gahbxtvfw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gcfhltnpi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcugolqlf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gdwnyxcaq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gsmcnuaze.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gcixbyuig.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/goobrkvsk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gvhknctew.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/ganuvqenf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnfudmfsm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/genlimeky.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gmboloowi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gytrphldp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gmrwiwtrh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gjrxobwmf.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gyvtkyecl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/ggziunziq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/grvlidlah.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gzynsviok.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/ghwyjdbtf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdbxylhvr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/ghfrctaic.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gwpuglqyr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gmvtstwvd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gboiumfms.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/guyvcweij.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gdhyvpcwe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/giqyqacwr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gnjjurrxe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gohxaohcd.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gmaqsdack.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gfalcfuuc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gckpqwmzq.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gddqyvgyc.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gfmwjbqco.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/ghnqbpztg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gxibnfuhu.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/ggyxrqfgo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gyohvasmb.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/ggqknsbpk.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/ggvkawkzf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/ghrbwpbee.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gtejvgozf.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gzpxfpywu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gjkfllhxc.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxmqxffnq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gocvzsowj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/ghxhrbhay.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/goenzwyik.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gwxccfqca.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gdlgyvurw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gwpzbkcrd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gyldjzyga.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gogsbdnpv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gohygtxjz.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/ggotybicj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gazeeljye.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gmitwpbht.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gpucjieuy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/giunqpwlc.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gfqcvjawz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gvmuanqta.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gwdrlixeb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gkdlbqukv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/goifqlocz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/guzighwep.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gtvyipsrr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gfnvjxrwc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gcazslrqa.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gqtfvnwtx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gcoxrlnvm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gtdcegpty.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gmzdzppig.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gcfhrujhf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gibkrzdub.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gxwlphhqq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gupjotjuj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/glmjwgzgu.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gjbqtzhem.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gwbaporia.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gawyjroaw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/ggdqhscld.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/grkanocdb.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gbombwzyj.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gbuchyife.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gcoyhptqg.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gpdaljifv.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gbtlzlpfj.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gkzquzvpz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gzauohtln.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/ggeejueum.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gsuwoejyf.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gdicqigcy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gtfhrarej.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gqqnudhsk.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gqmpdbxbj.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gcyyxwisv.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gdgtyopry.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gjmrnjhcz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/grdewuosu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gpagtfxwy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gqkttywoh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gddztzlcg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gmliybuhj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gaasgrwwx.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gyzqypirk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gmzdqnobv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxllwxahc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gnqfgqrge.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbvqpabcv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gsjnmbfvl.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gbroxosmq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/ggwxfyjwh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gqoumdnxz.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gepxtdgvv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/ggygdwxqy.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/geenkudwq.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gjtxkxiel.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/grjjjejkp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gblswgcvo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/guvbzwuts.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/goukazveh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gwljykmxc.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/grzvlfenk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gxozqdamu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gqhzlbvnm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gmjhkfqws.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gjzgippbu.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/ggklojtwt.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/goukettli.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gbbdpagze.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gphsapdnz.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gpkjfzjtp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gjnkjsrcj.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/geqwmtrvh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gxmomeldm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gipesyvfz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guajdtgwi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gcxgpiyjz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gchaeojhj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/glucofkel.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gucwncxdx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gxwgzuaqt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gacmwfafm.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gjcelnmjr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gmwtxkdhr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gxpxuyfud.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gsfgwajpg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/geakxtgts.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/ggmnesbhd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gqyqljzmx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gjvettbos.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gaaqzmptg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gnovcsmae.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gpjdhudqn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gjrvzgkak.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gojlwygzz.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/guxirbshq.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gzdisehcv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gbhqongso.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gsyuxeocp.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gdtoqlxbn.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gthbvegaf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gioeyegim.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gmlcpfshz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gokwhetyv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gqafjtpil.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/ggxhqgwhj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/ghfuhazqp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gihbyjlwx.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gghhwvjyd.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/grhfgdsoe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gqehinrah.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gyahtnpof.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gimkdghtu.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gxpztbbnn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gzaomtpyv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/guxzefekr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gogofmbsm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/ggupqcdrj.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/giasvouaa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gnyzgugli.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gbxhrjlhd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gnahkmdiq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/ggdocasgq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gcevrbudf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/getpzosje.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/givkwvokg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gfuyylnop.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gxfwisijc.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gzqijmvtj.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gxbzdatix.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/ghirshrmq.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/giazqwzos.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gmzwsbsvy.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gmtuxjjja.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gbankjdvq.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gduuzfbto.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/ghoqzhhxm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gfzevobio.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gijjclbct.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gugznuiny.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gzvjfohbl.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gwkdzdjuu.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gvyhldafh.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gpeypbyur.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gnnpicvug.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/guvftcsww.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gpcxivkvg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gnwzenuya.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/grnohglka.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gkmkhfngp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gtnmfkxbf.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gfbcolnsq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gnqahpgmm.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gyrizqjuc.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/grwnjzlvm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/ggfjnscth.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gpkhqohrw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gzxyfqyca.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gfoznkcds.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gqqtefzsh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghvsiouun.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gjqojzbod.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gkoabhhve.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gkrphrgaa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gkjfwwzpg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gdufwoflb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gyjjiqkpf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gdtksvnfk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gfjbfxhit.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/grdxgmtdo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gyhowcitf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/givbtmltt.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gdyckugcu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gxedfldmr.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/ggehwnajh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gboklesih.sHtML


<!-- 参考信息 -->