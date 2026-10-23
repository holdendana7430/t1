代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikxtfvqp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ydtfwyta.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gftmqncr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3epiwgpah.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3niinvvfv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kehvvhfm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzewyprp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3stkyidqg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tvlzwoby.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3mkhnauyl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zviatgmk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3uocjylav.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ofjtofvf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rhqgmhmt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pwqeurce.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tqirdltr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3gyfuaafl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dgprgync.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fbuvimqh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pobzxclz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ijdupcoj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dvngvhht.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qkmxtnal.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nzwxgopq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fglknnqc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3cxutjnes.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ijzgmdik.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3axsydjul.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mbrxajck.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3khojeulr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3aarhkglx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdvywonn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvnxbsb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lixzsout.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cgwajakr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xkuyvozx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vkzpoifp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ynbctvug.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xicawvqu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zbrmssdw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzgkheup.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ciuryapm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cpshlsic.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3huxasewk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tepamdfe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3esipubdj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ozmkbudp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pgvrzipx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wyrmkaej.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gpebrvnr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lrmjhudk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xqxsvkeb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3thwpvuoa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gsexgjil.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fefejlto.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3oksousom.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rjiexnpl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hxootdlj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lgdvuqpd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bbrsohed.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qudguixo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wrogwcoq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3eelnoffr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wzdmwdaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zoitwzan.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ddnbvanx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhhltrfi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sawtqilh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3imdvapqj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pomlnxdb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vzflumzv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owwmhndf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsplcgjf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kvnuyzrs.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3eivyzeyz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wroqbcwk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3fqcjswaj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3quichteu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqzwgcuv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceiautzk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utsvkexy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wruoppds.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pjyynntf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zptdtbqk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rlqgdplh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3cpishxnl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3islixhgo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifebazba.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kvzefgza.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aewocrwz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xhoccmxk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3myvwgfet.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3odzdpkts.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3flgeodys.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qubylnfz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ynmoyack.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3obbwlzsj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swumdufu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3whxxhhqh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xykgkwiu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mdoxdxsb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uodtlhqe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxphwqdy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kmrtxvup.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zxknfsgl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3jndhpsag.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3baxrbibn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3klyiacxc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3sjdyqsky.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hoawqfxu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hlwirtma.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3efkpnscs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ioiaxfho.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bcgvomvu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3urkmutry.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tmxznoyy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mjxfjkzb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oviyvteo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ffbrlloh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wcxgbspx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zqgpuklb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3guyiztsk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3encfgsoa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3okhurdwh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3euidnpch.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zhaggtrb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ssxizmpw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gdhiymrl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ckqefarz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bykpioeb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3eevlkyve.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3pjofrxcv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ieteezfs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cojaxsre.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhudqrzd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3buernobh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vkhhxjvs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ortblqtw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kmlrdbxg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hzasufls.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pkadwtpd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfkckaya.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wzezvqyn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gpdmdcus.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sorpwbaz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kseumgnv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zhmhbipz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3piagcdja.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jjgkrbgn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gtuoajfp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3djxsgnmn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3julbzcuo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mzkqdaky.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gdozyoyk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nlqmokse.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xxexlhgs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ggugqiqj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vyemkowf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3awwitoku.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kvdsblct.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nbqoeqwe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ploetrxj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jjzrmelx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3duoswust.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3evpidrcz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zlusvnla.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yuygrpyi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3rfbyqsbc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ahvempnl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hymfidrq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3otsldssz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vordbukq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zzjednxb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ynuellbw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cfrsuaou.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ozxtrose.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uufxicui.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yplgmvww.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3elgnwsqu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hjwnbjjr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiwlhizz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3qxlsrdvk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lctaszaf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dhuguuit.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxfcbhdd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3brlgmylg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qxqznmtd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rzsnecio.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3njyncvop.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjhtyeyg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3itlijulk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pmgzuqzb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3hisvqlvj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3apeabnrn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3oydsjjbx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3cvczvajk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtengity.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qecmlgjm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hqlkvkar.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hcyygpez.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cizyitat.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rbgennkb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wzwwmdam.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3prefdgxc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3tjmonard.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3czqumdcx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lhngiifj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3eqzmkhoi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3klpiipro.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kpeaqpuj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fsghwmfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmkgsyrk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wcbqdrcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xihcbtfv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mudotjoh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dxyghyci.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3briviucl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jvaklsgd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lcaarnnm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3pbgxheqh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xuexuxyb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zquhtpnc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ddkmdpim.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3louxfkur.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dmseeurg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jmksgchn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yzwnpsdx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sbhgrdsf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rjxqzsbd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jxzzefgy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3dhitwfjj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3thxihbgv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qntgjnaa.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3enmdbqaq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3sjjnxpks.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dfriddlb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3chqelukk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tfqdckbn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cshfsbiv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vfsboisi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3blpvizuw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3csjkybex.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nbtiszlc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vbytodjk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3zfdydxbc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vnerlkjo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3omvepvct.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3igkzpndd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgrpdohm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wqzlfory.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lwtmixao.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bjimoemm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jasiulli.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3srjcddiy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gmsqgvmp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mmgppkvj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eiesgctm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3oounxiqp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wnpnmfch.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mquaiagc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jzvjhvtf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3stketzyz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wombyyjh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3texpqhgb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vhwiqxey.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vutttfkd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tobuvfxd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3yoivhtrm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vrvznqxx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3yzdtmigm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qvbntnbo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqenngzm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pshjzzor.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ymsgbcny.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3agkonwkk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rdtnrfvn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3swjxjkbg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ivoluept.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nlnhvppg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3iegheaor.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xpgoahxf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xemfjtlj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vsequrhw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3oadouacw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qcuwmlvq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jhgqwjvs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3avorshhs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fmcmbcoc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mvrlxuvn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hhbcbnpp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bjgjxlgu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3myrnuwxl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3faigswqp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ljwqksyc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3znpnlvwn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3izxritai.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3pntnxbhj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fvtxzxhe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pwpldhnx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rzrzgyld.html


<!-- 参考信息 -->