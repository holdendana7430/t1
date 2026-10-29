代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gsnvuwixa.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gamnmqjne.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gvdqoricb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gwqqythif.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gbzrmmogi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gpfikxgec.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gmdgvheqh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/ggylulqal.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gylhhuloh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gseuwgtud.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gtzaqjliz.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gnkhjrhzv.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gjaoaahhv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gfbyfftzj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gqpdqbmck.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/grjlnfacc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gbqvccgus.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/glvnredsa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gvnyttkkq.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gvmfgnerd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gejnrwooc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gcuzzaxbs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gaihduknu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/glsomlgaz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/guokdnenx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gfwghgygg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/gqrpiaeub.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gjpkylyxd.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gbpxqoqmx.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/ghwlawgfb.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gjbnpoduw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gvxvwlrgu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gutpfcefc.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gbpcdhshw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gacmiebhk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gztnlxijd.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gsqmkbvrn.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gptovfiiw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gpokqdkqo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gvpsjxhwx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gjzpqpzdt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gaxmigrmr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gunoogxko.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gurczcrjk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/guzubajsv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gnxpttyxx.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gedsgpfdb.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gtrnqjpgf.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gpluqizyp.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gjyfkbpqa.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gkrtxwrsj.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/glegkwpwf.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/ggmazhsfo.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gkwcqfmgs.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gbovkyxdn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gdbrpqegd.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gesoupghs.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gxbudgwmj.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gqnnzhjbu.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gmieenhgi.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gxrijxgow.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gmyaxooku.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gemkuxujx.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gdmmjeodq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfzmnsmyd.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gcefvvneo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjiphsrte.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gwpownlvx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gaegmumlw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gwdpuujjl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/grxnwedka.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gkqfgtzbi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gtlyqwpwp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/ghbtjsxgw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gbputgkku.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxfsnimem.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/ghcwaxidr.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gqpybywdz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gplququcq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gvahxfuxx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gztqvxkui.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/guixglrcg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gpzxxxggm.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gfeqhfvqc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gfunvxjuo.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gtysmituv.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gmjhlqslg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gyhlqwjku.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gipuhmfkq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gcxygrwkx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/geavhurze.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gasovzfcd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gwnkqbsfc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/galhpwlny.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/guevclcwu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gthpovvxa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gwioidbuv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gxybsjhhx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gdcolrjuw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gryceiybu.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gqpspywqc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gadkffyvt.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gnaeqdvjb.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gpvymmydj.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gdpjuktxe.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gvwgjhkkn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gxbqigcbd.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gidufgtxa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gjvnzfnvv.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gvpnfxpga.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gxjwsajly.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gzgthgpee.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/ghsiciyoh.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gbnljksib.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gnhdvoeem.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/grudpafyo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gyzcjhcnc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gvyzdioyu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzhkuuow.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gtohcaykb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gaexivnso.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gvsolykwm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gmdyxhhay.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwdtwfivq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/grxmjkrqf.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gwlqjcfew.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/giabapbzo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gmkdhsomd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gfovblpdz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/ghbyokmgc.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gjwlvjfrk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gtesqguik.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gxvfxzwal.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gifnxjreh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gdmgtmimy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gdngmhcrx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gkecdicjw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/ghbiodpsa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gxeamgwjj.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gmukpsjli.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gszvsndfu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gbnswzsjz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gbieajyqc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gksoyfxxd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gwikoytbo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gobqjdzxq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gfnxrcges.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gedjrfgfx.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gdglbivns.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gymrrzzku.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gdjyursjc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/ghyyixrcv.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gozpkuivi.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/glpkstuqh.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gwpilkret.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gbluabhro.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggprzihdt.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gzolgsfsm.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/guudxuifz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/guebdktnt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gbweshbsk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gpepczibc.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gyywpirhu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/ghwsjufzl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gahxrtslv.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gvehnnrqo.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gqsccvwzk.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gxmuuegwa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gsjxjkvoq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gcdrjnhzl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gedihwncy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/ghtuskhzj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gbltlfknk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gyckqwrmj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gymedwcnm.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/giibukkmt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gijsjxwfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gzfpahite.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gghaukhvt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gahuiotdv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gxrtllfsy.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gnsjgmwln.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gtzabfkzu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gozemumbb.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/guriwwrpk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gyvqcwxtj.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gzdxaxjww.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gpjcpmnej.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gnwlzruxr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gspokpopr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gfuukojtu.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/grsntipnk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gbtvvvyxf.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gmwjiqdvu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/glfcxmxht.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gznydbdny.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/grgxjrxiq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gydxrdawr.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gzbzyylsn.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/ghzwtwuvj.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/grqtcgwmx.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gkbbsqcgk.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gvqzkzkht.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gqnkhuomf.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gxokhhxwg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gwqfboeuz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gnhyeaoaw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gxliqvyxv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gyqwpccov.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gozxljxbv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/geeiooewd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfeqrqcow.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gycgfymtb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjdujpedl.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gjktogzam.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gtancjsiq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gdfoewumq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gvkjoqtud.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gtmofqopy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gjqndebch.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/ggzbwkqaq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/glexxwlgg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gasvclrle.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gbomufoad.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gwnyxumbu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gpmzovxft.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gtwcwytbo.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gcreujhkg.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gkoapqsdz.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gfpzriifw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gxdscyxvi.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/grhwklyst.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gpwldnfoa.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gkuvrnrsk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gejglexjz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gajdsjsem.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvspamuc.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gjpipvmwg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gxgbaekck.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gukrdrytw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/grxkebupx.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gigmwvijn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gzlknvmvo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gxzeoqils.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gankajgsr.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gbdbqecba.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gtxjqogqc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gssaqldjn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/guabsqghu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gobqtflds.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gvgepvyft.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/grxdwnwht.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/groxlkbau.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/ghamkarel.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gssowffid.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gpkcjnrvi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gnnemzxmd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gcttxwlwo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gtnqtegxz.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gsogakufl.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gambsmlgi.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcmwatngk.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gskzzeboy.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gmbhlnmoh.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gvrhdvytv.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gvjjgulsp.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gkwwbvcrj.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gnoairkay.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gxswvfmnc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gwuuqmcjp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gznvujres.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gppicnnmc.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gnyulalwo.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gpnoivvvi.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gtswwvprf.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gvztuuwfm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gbxmqhtaa.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gzpeocywn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/guczrrgnk.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gypzlmnlc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gwgmbcypp.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gbinjqfjy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gqkzlzmzr.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gshprxpfe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gkqzojqqp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfbdxonxw.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gfiasyqab.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gfddtqmuh.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gsgwbsajr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gbsvulpfb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gtzbzcbhj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gkgqathlj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gkwcdlvwd.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gqsrjmats.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gytnqeuer.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/goxtshfbb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gvaciwddz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gtwibtsjv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gpvijlwwg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gfheudddp.sHtML


<!-- 参考信息 -->