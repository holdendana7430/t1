代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dhrwbftl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3uilkwtko.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddhwojpr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ojaezhxb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptxykhcp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgdtxcmy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jcprwvvj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3znpfjryp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lvzqodsb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uuzwzizm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wfbgsdwd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xclsrmbs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ixiarmyc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pqjlcgke.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3reezfrzz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bkblwqvc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mphexmtc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3psgyszoe.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bawaiwna.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3fcooazwd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3irqgawam.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oomuicxh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3crwmltbu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ckfulchq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3zfvsxacc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kjxazbqr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ymppflts.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hyqgqfuk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3irfndvxp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bozinrhw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wpyvzwxz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vgnlhnjc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qwllmkfx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3spvcbpdh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3uksnsqug.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ilhztkov.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3gcmgpvcd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vbfhfjii.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tmwokhvh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3stbgeyhc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3canletfg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3zfdgvivh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pxahnckj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3nskmhraz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ghfcppfw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bwdxdnro.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ahcykbef.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tejgyxpm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvpqywa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jagzegua.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xhcddwnh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyiqqyxi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yrhknosu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtydutzn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mlkuarii.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ngaylzyw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3nhikrxbt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3enssconx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nznybzhr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tnfibmdc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hodeztft.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nuflguut.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3akejgqcr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hpxgldoy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3igacalrb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yslfqsvv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lelvsyug.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bjgzgvly.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eliszhrl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3sloqhxrh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ymboipch.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wimksbap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ravecwzx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ixormixp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcohvfsx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixfcmmxs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zbdieucn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gixygkcq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3enhkvylh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qaupgqef.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3relfmjwm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3uvtnubeh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vooyknze.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtastugx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3kfkqigei.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gjbdhoec.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wvygxwcw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ftlydrjw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gfaxarpm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3futhkezf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tqcgmijj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zseustyq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3gnworseg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjrqdost.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qzpkyjmj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rlxagjew.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqtqwfno.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqyoqrtn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3kqeadsnm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3dzddmzoe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgrgjvzi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pricqbib.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3apcwvesv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ksmkiaac.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wdnfpfbz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sifedslm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ykpcvlza.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3kbmbxkva.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vdereacx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wzslclwr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cehshjgo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jwsosoxt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3babfyzhn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nchzqgrp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bznnvdwr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ywwdqlvl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vgmzucnb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qxzimver.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eiimdcto.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iagawpyz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jmndkatw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tyejgtoi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3dvhrcjjw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nydhzttq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jfjijbya.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3brimuoun.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hvftndeb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3auvpgpmv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ptrcmgju.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3kkpkwzus.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vpukhpvv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pcwieeqs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gjipebew.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3vnyjnjpq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ijwehyog.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kzrjalbj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lglcdwqw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3cwabecfc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hgnmtptw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3rowcultc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gftezxhi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3loxplfmy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ahdxjwem.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cmzcangi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cfttrtyu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3oildosnt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jdafmers.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tcgukbnu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yiatyisl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuhppkvb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lueqgpkn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tabmcctt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmwhbuze.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3giqxmdee.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3etqmsqzz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3adlvfeco.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pavpszyk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wiqqfrfh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ylnbvycq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ldkwcmud.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vuhpgkqp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3itdvttzf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nfchnszs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3uqsnisia.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sbvktgxs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ysyvpiiw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zpuscjqg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3inoyvxmm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ekhdjbha.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cjopvwgf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3mivqbfpj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3yxglkppu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3naoytpph.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uvgigqzu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gdbsxyqb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mcaahbpc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kwyzivnd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hyjttkfd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cwqrieru.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3emqkmphw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vueqqzmz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kxshdqav.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qbrflgeg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3zzfxzqcq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dqrieqrt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zqvolujx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xqjxdjsd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qngulmba.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tisaopzz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3qzrfddyk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3fbkoatdq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qkjcdblj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnifyuln.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jcgioscf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rxftpwts.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3aramswxc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ztezaifb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yugngjcb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3iztsvisc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gbehbacm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ajkhrwyh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gggymyhe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3cqjkortt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qwehdvik.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxqjuqio.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irduvdxs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gabxbnxu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kftzudgn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ocjkjgus.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3dxbuaqpm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3advrlxfz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fdijusko.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hqciplkc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mwglgvfb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3irlynxaf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbasnrqq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3bhufnfev.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3htpguhil.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxzhxgre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stuygdhh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vtgrudyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbkgtcpw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sqjrfvxl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3efxsxkhb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bwlyzcmu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gundiczp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3syhvlcpy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ngnomgwh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3badqxibr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xtlkpmgm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rsjgrqpq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3uxuiruyr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3gcdjzjxm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3xdtbthxm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3glmpwkoy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vrlyqcez.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3acjkftvl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pweujgei.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mxdtmtux.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mehoczuc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vcbzhrks.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ycnnoogr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yqgrnlul.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vyjgjkga.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rceertgg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zqyakjfy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wionmbat.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3chhjdfuq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3czjzbprz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tfrjaqsy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wzagchaf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pfgseaww.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3uuargeqz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ivmmyebq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pcrmfipe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gzvkpbnp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ikcygwdu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ejkqjmeg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kqrcjlyo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3youhvrqv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vionkipa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ttbvfbfl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tdkdhjpb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vmujffoq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3szmfdlwu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ffdzdljg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iwjajson.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pfskhyni.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xcugoemp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wcqmvtds.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uyiedvnr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bvoeapiv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gyepkkom.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nryrmkuf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lrxekuad.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kxnojbdp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vbnucgkb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yzarwwsa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qgceeoxj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iatnlowk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fuzvfgcc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aljfauoo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3aewuqbqq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fwkfgabf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bgdxpmis.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xgecbayr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oengmgcu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3epdjtjby.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fopzvgpo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kufipbzx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wfcdihbe.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lcvuewxg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3sbklvqgl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sliagiar.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rugviulo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vjqfvamt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jyirrdml.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ennkoklp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3naqbgunp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3batspiiy.html


<!-- 参考信息 -->