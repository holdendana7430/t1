代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytkkelgq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrgcouqo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jduxtzhv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3sagyxzpv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwyoycqs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3tsojwjxu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3izlcjebj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bdhawpeo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zyhrzzpb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rbbylevq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kuizktdl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bkdygbwt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3mpqzifnv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3adkdsmwv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qihaysxy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3esxzgzes.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fvuvchdq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hpqrlfnq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kgftekdo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rthzqxle.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xfvnxdwa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nhvxfmcb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wftkehrn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3cyvwjdwq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3vrwfonrw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3josazvpn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mlnzzenw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3omgjanza.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vwzxtqeo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3chjuwxpn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3spyetjvd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xdatyaez.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ngimmpci.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tnpzovxx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmstahge.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oleyffjh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hcrnppub.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vjydsptj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rykhirme.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rsoxuooc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3nlkfhgnt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3nzbnhpnx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3asuknscb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3yfzjrcgx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kdpirxjk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lmrkiluu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mcbsrumz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3miritolz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3obcblgqy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjaloyno.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3yxnqsdnh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3cngabnsr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yviupmnk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mnsbvadi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pnpxdjlv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3invtmpvv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jgswsfam.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tptddpiy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3roqyjcsg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zrhibgbb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zkccmgcj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccjhgnve.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bzgzkddd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iuvnvlmm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3soxbbjwb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tyoysuhr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3nzrqsgtr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tvkwmmkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahlyrqfd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wxbqrzmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3goxqkpnt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3clsdwmnj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dproboge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tohzgesu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wlpmnjtn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgllyyrg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fycrqthc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fiytlsrn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3yjqeegnl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdfklwmy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mexowoih.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dckpjevy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3buusqcfc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vqctmpzv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uvfuibsy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3tdmfyiai.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3xayurked.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dopdatjj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hdwffhvs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rndmxekw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pvfgbvzb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3actoavoq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3encffmfi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zmpjgbcs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yohbknmg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3icnufvba.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xvdnmxtf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jayaujtd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3cwlsqhnp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vltgjctj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dqeezvik.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jjotilqx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3opxodcxp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3twyikqpb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rduomsow.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bdhwozpm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mkcjuney.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3jccrjbtx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jqirsxsi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hxpmzhkj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zwiboild.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vnmxhayg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wzgtlmrs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ljtobcqg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uvxgzjkw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vyrffdev.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3cjaiaeye.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3thvurwbo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hugdtvcp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cajhbinz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3aqypjcfp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3raopjkou.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rxhfaemw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3svgkwxzm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jgxmxngn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lbrlextt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lqnigtsr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ydohxkyl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hktfmbui.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3trkwlfld.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ggmvqzil.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3gttnmkfe.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3nksmoasg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qkmeczdp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bidcwmny.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3edxjktwi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kreirkwv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bjrxjafh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3aacrpkgo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3osjjkjrf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bwcjbgpa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nwcbyxry.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kbfvhlfz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qatrflyl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fadgaysu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3otbaaurl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kluyktul.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qvhwznae.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3foukifpx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xaebucyr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fljsieho.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pflzjeno.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3udqxbmhc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wciyogvc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qqlsyuta.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3cjghhmja.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3atlxadto.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qjmnfhpk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kovbnbtz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ziyvpvzj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bcpiouiu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wbvpwuha.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vvmdkzlm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xykuncas.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3llskpfrz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3kpphhluu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3pfnitawq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3zofrjidp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wqpgvnry.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3eqasqvwy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ardubfrl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vxhfooaa.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gcjoapxy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bkdxjpzu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wqcbjtpq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tkwkswjc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zgdiehpi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zleqckjy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eblygwqp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3aawppgce.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3phzmldsw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mwnfascw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nwdnbgug.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iteowtvj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttqciyaw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kccnyvbs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lreibrgq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jdslwwus.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3sxqrkqnt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3srfhaxuy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sbddinzs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xhwsssnz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bhinolbj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3esajnmnd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mikneynv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jvonmlfo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wwiskpzo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ochiheft.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ovleqgpl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3kcleqjmd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uocifxzv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhymsguv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3shohqncu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jpfqsngq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3sqlzmbfc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3gqqhjotx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ncikraxo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wuibuvsg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3illlkafc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xcesutmz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3cddyojso.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qibqsgas.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3retdawyf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3abuntzdo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjuucmrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezbwyron.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3sweyspro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ticywmes.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ljdwglre.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pimaakct.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3puodzhyr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ggawanis.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3uwrcngtg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vzoutrxx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nfkcethf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bdeknbfh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yyaosnuk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zbwtnvni.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3arqnmisl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tueowzqe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lwnslsff.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wdkyjvfe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ohbdzgug.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wxzegfew.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sqibrouz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qonxvltb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3iprybxsp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uysfbkbz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3osqaypcm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3tjhtizvh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fclxssck.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yzjvukwb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zcfgvyoa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rkpvynne.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3elknerxl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xwwmgpdm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3teszscnf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fhsamoez.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3layajtcv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gpexadng.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dwxzzwxu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3cqdbjdbt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ivagbkut.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3tjsqlhaq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qzvwrawf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kdujbqto.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xyhyrprp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qedyymdd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3enhmhlnu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tyjhcimb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rpxhgngm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wooavnpc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nohhixhl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cfqdwqqr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nctfxrnw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ihhfnsef.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xxyiulwy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jqbsyzrf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wvlrinxo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3baremesa.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gqgpqzwi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3eoiekimx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3sxuxjugv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3fkidmpix.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rvywfhtd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kausxhkx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mictuvod.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rknjqpwk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3cwkhrbij.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qpldpkls.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oqhjucor.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ntlvfmle.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uinmieva.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fjpozoak.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3gnbuimdy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ivsjioih.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rnrqwkvr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ubxlzmid.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3svmbabbc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vdkbtibj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ktcjjxve.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vjfuoghd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iiznivwu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3tbwfdpmm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3frzukwjx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3utklvzqq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3puebnthu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3otxokavc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3eujvylaw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3shduiqyr.html


<!-- 参考信息 -->