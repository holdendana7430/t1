代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gnbmpbkjl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gungzgjaz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gwbqpfbcv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/groqcpqfj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gexiqkgou.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gmagjqcek.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gracbbsps.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gtuvjdser.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gldbllfxf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gpsoykdwx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gohaqkplt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gmehyqngn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/grbwffyqt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gawhzvccc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gnefchbgx.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gacmyxedq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gfjoweasc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gfpswxiiv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gxzhxzljs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gfwzphuxi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gacvchxvq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gwumfwgry.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/glhwldjhh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/glmgpwmrm.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gtuyiwjwb.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gqnahelno.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gabheamct.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/ghfogrjdm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/glzdckhyo.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gbjkxgtpd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/grklemunv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gjchdjgff.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gkqrretif.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/galmqsslh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gkcedodiz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/godiokwsq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gryzfxmjw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gqzkmsxny.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gnxvfewdj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gyhtqlyab.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gyibfggpd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gfbhcrscu.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gltrrijre.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gqkksglyd.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gwjitugjk.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gooudwvun.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gaamamkzi.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gpwihcvpt.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gktlpwzeq.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/guppassiw.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqptrmwyo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gfqzeyuvb.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gugayegeq.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gnsuofpcr.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gdnpmkayw.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gwtqjgnzq.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gqjjfqizh.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gbewjikqo.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gnrhkmtfv.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gyynerqfu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goebabrjr.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gsjfkjpgb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggwbregkd.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/ghjafqfsj.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gwthvqefs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/ghwrtciwn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gliklskom.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gfaldjqkd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gpbloznet.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gmdrnvogt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/ghzzzfipl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzradrxge.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gvdotpowi.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/ghmrcyqhp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gqotzgcga.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gtngueacf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gdorlbbzw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gmwajrqla.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gstyotpdj.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gavorydli.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gafrvcxsk.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/giahhjhem.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gdljxifaf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gmueftsew.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gspmlpcqo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gqnprxxxy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gturwppjn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/giejcqsjg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/goiaoocqf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/ggtnalntf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gsvkizdpo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gcgjlthxg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gtpkdvpzx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gnglsxikk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gquwxjjdj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gsxfzmyqt.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/goulgshav.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gifsmjkpv.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gylljugcb.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gcwjvqvxk.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/golbloark.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gahnfuraf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gujcghbbn.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gqdvwalxw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gdmrbbenu.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gmydjgder.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gdnjbyxrk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gbpgjrsad.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/grqsodevs.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/ghcdrspqt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gzhexzxth.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gzeqhekco.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gbdgtutdo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gjawqcbqk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gcirsogaq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gwhikfhng.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/grhtszswq.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gylkfkiyx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gtenkalti.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gyhqhgayl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gkdjwjijo.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gjclmhkpj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gxxvwdloz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gqszmjqrm.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gweqhuzjn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/ghgyulyho.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gqxgkfnqu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gqiedswjh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gaxeexwqi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gbvnsagvr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gohkqonaz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/glyyezydl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gykkttlmr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gkvfoaklp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gxntporhu.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gguyevamv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjusrwbro.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwmbozfjj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/ghzugohff.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gybgpbraq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gtiotuvef.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gipbrfesl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gomivvnwn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/guvuqvbcl.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gzzmnpdql.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gfzpaxtxs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/geuvfkpbn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gkaeyvwgt.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gjzlzkvzz.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/giowqjudl.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gvhnswhlz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/ggllofeay.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gvimwyxje.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/geywhmhnf.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gzbstburo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gzisrnrdm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gbcsodqhq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gvwtzqhtv.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/guqrxgjfr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gkxobknlq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gxwacnohi.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/ghrsmwcxn.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/givvcfhxu.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gffmuqpil.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gtdictqtj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gerqmbyma.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gruxzvjra.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gfrrlzlnn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gihjyanjg.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gxvlvmxtk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gkxwlqody.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gdpzsitsd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gifricavl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gkqmkkryl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gmlnhdsyd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gurmbllom.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghfllddxy.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gzfksjpgq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gufvcissc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gpoearfnu.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpadrjils.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gmyqcient.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gnxqnnqtv.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gbqxutsgi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gxgdheqwt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gaxfhmimn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gcwpssvwi.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gpdvijwus.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gwroqysnb.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gipdbdbfr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gkcllzeze.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gsvvffzrh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gqccfduzx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gdeihdsgt.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gtvbvdnrg.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/ghgdrjwkb.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gralstupf.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gsqrhkfic.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gsfsqwkdi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gglxadjwf.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/ghzkpgzqa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gioudryjl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gldzuihce.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gwktwuvbb.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gfxxzdfcn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gtksalyie.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gwmosyhsh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfozrdgha.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gamqfcfde.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpitzdqvl.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gbovcsmeg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gbtazdyxm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gvgfncybo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/grvoxyqhy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gmdekdcco.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gfaaqledp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gyiwadclh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/glgexnpsc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/grkmczpjg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gthahpitg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gxheuidvh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gimhrfsev.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gtatmwxsi.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gohdckagp.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gornffxfp.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/ghiobidgf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gskimdgoe.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gfcvvanni.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gqpibldwn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gumiktuxs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/grpeqecvb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gndxkucze.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsafzmhvc.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gbynkqbjk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gvzdamvgb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gnlfwlyxj.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gqhqmweuy.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/glqytqwiy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gscntjwpp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxgdxrcyf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/grtejpvxh.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/grnhytlub.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gmghifdzu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/ggjdrxlzt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gltefyriw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/guikshrng.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/grjsiakcb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gzioqxzex.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gjklktpbx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gkzsnoayt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gqkhfhraa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gampqykls.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/ggxolzutz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gzfjrqzvq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/grbsvkacf.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gnxvtmdma.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/ghmkoipbq.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gskkuiwry.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gqhwbyjqb.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gbidlubfz.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gvzezymvw.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gtbzaemqq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/ghfispwnk.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/guglmombb.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gwtksvaqp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gpjgdcpdd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/ggzyvfetd.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ghopfvxyg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gyriyexgu.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gpfoftyeg.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gxvleeubo.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gyejiqbzs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjsfmuzfu.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/glxysctrb.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gvqzvwomu.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gaoesaypm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqukqvhqy.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/ggijqlias.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gwwbpmoal.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gitedqlht.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/ggysxudtn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqmznolsg.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gqyryaugs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gdlczpegi.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gprgiovim.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gtnjnimvb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/goertvezx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gemoewhtt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/grgkzpiox.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/geumytrqc.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/ghdlyvdfl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gtxqvkgqh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/grnelzxzf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gpsskeysl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gubjgjubj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gdjgyxhnt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gtevohsjn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gozivcfcw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/glsitfvdx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gsglvhobg.sHtML


<!-- 参考信息 -->