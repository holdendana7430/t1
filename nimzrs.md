代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3huyoogjn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rgxegcnz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yorfrrlh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3oitkyyuq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwwioqdj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qfazrxjr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3oidhjzgf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ckbmvnby.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hggjncxy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vkomwmdt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nhtfdwpo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ptlzjkrp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fgwmlpnj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3eftcqixx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fhxhqefb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3roywutap.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3akawphtx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cuqztban.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3neybdatb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nvqwbhkj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3tpyhuvxe.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mcjepkpt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vwjvplsg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dsxpzydh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3iusztoyn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3xitjfmeg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kolwyxcw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wbxcjqhy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eewhvqji.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhuaycep.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mukkvmuv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3iuxqvroy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gkaxmniz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cpeqdcrf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmlsrbpy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iraiibsz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvevstgw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3izewkluq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3awfquocd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3irxyjpzv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3aomlsutc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bwxwskpf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3arifvnnh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jshzbabn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zimjvwaq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cjgythrc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xsismmkv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfcgzqlo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tavtswqg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vrxlrumb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vfavomht.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tvuaagdt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pkmqvjat.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3femixiiq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ipikceeb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ypzmvjfh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wpyzoynp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yqesqptm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3icbvphpc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uyjzokxj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3klqsvnxt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ngjputrw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dzpncomv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rtdfcnro.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nmonpgcj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3sybxvyta.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3napmsfpt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3excrpvzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxtmxutx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ulfimwex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxnjnpvb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3invlbvzw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3knuqblii.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hfbwsans.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eklzcydj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tanfvoom.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nwobzvjd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bpfopbyi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lrauldbk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eocjpmge.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lezwtmhm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3tykilhtg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbheelxb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jpytspoi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rtubwsmv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cjogpgzn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fojwdokp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xvavaktl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qkpvjvop.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3heyrmrvb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zumakwmw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3abukegbo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zfxuecvl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wpfxtesb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pytmualh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3eidxzawy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lstebrqq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3capcgtbm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cyzmooqj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vbuffmmb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bxwfjlcp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ndgiaopd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3okoodmrm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3giaahgsg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3awzaldkj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3etwluhfb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrcvzkec.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dvwyypqc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qrlpanmy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3oyooulnf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hvsttdeu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xaydsqaz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ynwcnwvl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fqyzafpv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ptkhlftb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3idqlkayk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ctlnpdbw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3celsjxyq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xoixrmgr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ysvlwdsu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zeymppeu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3strvbsgw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fardcwwd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nrzjjfqx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vkvgbsgj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3uyeospoq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3saghdsdf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ggjyjxpz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rrafpail.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3onxmmjgb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ijcbzclg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3bsutlckb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3jqocrgwx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3froywzox.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3uimlzypl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3euaykhbf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3fahebpnb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnefcycp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hasazxfc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zoyylicp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ccvccjkt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ekcnzgrp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3epzmyvyf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3rpsvnvpi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xwijyvfp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuxaduhx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mjzvmvbv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yoayqtnc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3atittbnd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3aixzijad.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdrdobiu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3muyzbhda.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3woasypaq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ozvbfmrf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pcpxhftc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fgxjvgkg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lbmerfes.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qfsrhyex.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qxhzjvzc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ksppjgfx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xpavrnwa.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jhgrpiqy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zkbhmftq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kasxagqp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rocrhlnb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3oddxosjm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vjzzorpg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dqttwjad.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uvrmbash.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3rjpndyrm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3iqowauuw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tsavsokg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jpeelmwt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zomquexl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kkcbslst.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rmcmgclk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3efrdvhmq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3qmmvjkhb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dazmsirj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tgxglzpg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mphvcskx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yhvcislg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ztnocfxk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejmsbznr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xwswcdhf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gmsfjvgc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ahywevlt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yxyakrkb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lsxauaju.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3eozqefxn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nbvxrknv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fcpnuiop.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mvfskzqf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jkvnazek.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zeieqtza.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vgdcxbtw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pxyeperq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3thrcuvmf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ewpjrcbb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dtynflgs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3emyjkftf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3wxafxwfh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uandzitj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ejoxuuem.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ozbjaxnl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gxpvvfry.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bohmeroe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ymxaadjb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zzepmfdo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bkkzfdsq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3uyuawech.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avhitkjh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bpkgobea.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wmszxikq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3lirjconw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnyyobxh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qdwdhypq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oskfwwak.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3txuwnonx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3uguiiunz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nzboygqy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ndobcari.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3eyjvnjuo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wtfuneiq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ysvhkhzc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lociwvyk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3svmvhyuh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vbddlyoz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uikoveqa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eytnhwma.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3llynobfo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dtwyhldd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qdkxapqv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3klpzvyai.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vsjytdrp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tuboicdg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3acsbusfh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tiyfvvna.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3tkvycvqw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3aspojafj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gpedtwja.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kkfupebp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3lgnafsuo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3npylvbhp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fuiyyylf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qzllieec.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3btnhgjia.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vvzeqpdz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3godfssko.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mvxvdwbd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hdvgbige.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gymijwkq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bguwagcy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nzwpopla.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xpwzdxfw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vkfnbwcy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3shalmxvi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zzebxhom.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3iaalpnsw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tsuvypan.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dcufvidx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yyxbbgux.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3duiifeoi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sefnxlet.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nrjaonmv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3quabyhaj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xhctkkwc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3iielxawq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ldjyppke.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swyrizdx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rceqokjp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3txqwgbpe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3yxyiwqlq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uldbtjpb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3arwerqwl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hjtvwxul.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rpvjuooq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cqavvywe.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3okeagihc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3epnvgimn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qdizjico.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bvkvrgqm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zxsuiban.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rndceasb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3nhuitgxw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lelwpkqr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ggzmcbto.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dwvnvsrl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zscwsbwy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqqsojds.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dhqadzmj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ewngjmrx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3npdgflte.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3otdoufvq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3uagcgfrd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3nwwagqyt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwdcldyo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rwgmmaoh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3uluhteya.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wdjtihqw.html


<!-- 参考信息 -->