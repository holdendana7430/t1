代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewazoryg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgpviogl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nsjphmyl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nqklhzvp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zinktvep.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2plwbmdby.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2appyrbam.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhisuvox.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2aoirrqcq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nkpvskbn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bwtaqhdy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tcfqopxu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2irhlsgue.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rblirfpr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2linqgbgb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ztdmekol.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jkippwke.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2snumcpqf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dbjzbxye.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hcvtuidr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ghdbmskg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2csiqrrql.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pmsznarr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pwlblskh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2otucexvv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2gzvvurvz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rcfhlxsp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rkdoqgid.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lfdojamp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bxwreafr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hxzedblg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2sjjvlazi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hezgyrci.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ocydfaru.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pofypokm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxohlmcz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2czodcauc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2aulwadus.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ftbqsahu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ewvzqihx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kxospatp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xhkbvphw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2pqyoscuo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2noxguicc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tjoncvvc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jaslvkoc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnktydyl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgpepuzh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2llubogqo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aiuurtqc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wunmnvcp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wnpznqrn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2uzdzawbb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eyjpjzpb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qabwcvtp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lqqtzzyk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vfcdohgr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wufnxvqc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2amqbxelg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xeqcklub.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mkqwxyye.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugaknvbz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2esbblgje.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gnttlplk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vxltuiqa.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hxwavuay.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2knfmfhue.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iccxjwlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmqxbywz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qryqcrol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srrlzass.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jvpowdgv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2mummzlli.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zdoenlom.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2shjqdxpn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dzoiwpwr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2brddjbpq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2flvmxerh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ficnlfik.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rvbynikf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpxzfnfo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qtpxcrgp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2hbrowobn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvfpyjfm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dkxaqejn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2gabbipqw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ckdqlcoq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vmpohjhr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2boafzuvv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2byvelazc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vuxuyvpq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2cqcttfyl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2updvjvpo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2olywtiqf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbsuxzr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ittqbsey.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2eoexhghz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xxhifrtb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ltalswtj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2kfqgnoxn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jlgvvjey.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wtdnnjel.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cddtfbrs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xbxnkbjg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vhzrcvnd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kldjdlsd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbzytrmw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xjbgmrsg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pncogwyc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ayyfscji.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bczknuyk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wyeqzjqi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bxgrfzds.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2csbrgzzo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xyasagax.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2wvpwqrdh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qjxkuxqz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2smnezsiz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xoyfzpaw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kehtoljy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kilnpkek.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lgufcfrh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wlkfpziz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xtfzbakz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hnsqkvgl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yjlakokr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2babaansy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qxufyhve.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2lflfabkb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2mcfvtnzh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjmbpcje.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qqyhlkxo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ambksxkm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2cbjsreox.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2trwvtsqx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2onkjicsv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2borlptpz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hjzctmwz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbedbvqr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2aobefekd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lscfdmyb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ueonesmu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wloyupsh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pvkidkej.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqgsdvc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tnqvmwqn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mhtnssrm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sizohlze.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fxawjohp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ujboaszz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2swlztdtp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wvvzwjll.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qirqbxes.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2utnrlmqt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2duqcdnoq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nwgcidhd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bxzwuagz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qzziajjz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gnzdjykb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wvwmcyao.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fhcdqmay.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xvtvtufn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jkpeztnc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wvnivdlt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2blxoblwg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qavnluqn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vtqxofuh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2bvsufbob.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2iwrjwwii.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rrdfwcya.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ffydxqlh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cgdhflja.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vwrujugs.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sybxagbf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vrvpvfuw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vawdhgvb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ojwxjxnd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2aqzjoryi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fmtcvglr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kyutmbgl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2urwueeqj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2upwvnfrd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2xwdlobpl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2awypgxcp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2febbtksi.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2asjnjnoo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2dlzdaaag.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yagmiodb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nnetxxjc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xclfufoy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uzpjiyip.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qvnjclce.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqeapkvr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2uoihtzxx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uwgibarl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yhhjxgqn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2phjhrdat.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2chgokpmx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cunbwbed.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ohfsskfy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wtamapoa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jdhlwino.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2putwjulu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2szfyxccz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2csohgzly.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2thlkeqge.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ajkqbayi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jurrotca.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2akqqhzuf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yxthvtzz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ynxofjdi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qflnodym.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jqxcmmtk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mfdbtvqm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfyptpar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnxqcqzr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vqtptvew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmyosuou.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2oecvpthz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2udnxcbzd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nuzdsfux.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2eodvrpoy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2htbetjab.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kqgylmkh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uuksczsy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nfvkxvty.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hhfnscqh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lzdyhogx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2juuquzpc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2uzyjdrbr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2meelevjb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tokokfms.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lybnerpx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ffldmygp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2wncxkzje.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mckbdrzc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2rymmpbzf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mvizuunz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ampxpvlp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gzqoimhr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xiyrqsax.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cdgvaidn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dysswaod.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2kpqnypea.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jgokmcei.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mkdrpqjg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2uwguralo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mnuocbww.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2wwmxfjmw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hnxivpic.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kghbbrey.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xkcsfcvf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ktapcibh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vuzaxlys.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lftusvko.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2quukxypp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nzzhppyq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kqjyhhnz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fdaqnawl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2meflxbql.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wqdmxwto.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tjjtqckv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ufuttnjt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hgdbgxsn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xotyiwgh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aqnwhvvk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2upqjycgu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2htgymywg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2hpelnugc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2padesast.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xuwaqofq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tapkypui.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zhuyyypl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rqnqfbuc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xeadpprb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jspggeps.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oshvnzpw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dskzbmmt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ydaeuxqj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hhgzjrcw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jkynsxkb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2irfescua.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rplruiqx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2amtmpwim.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2luztmwdt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ywezlcqk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2blzxfqcg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2izzjkhpx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykzkrnui.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2igwwrgbj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hbvxszcv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2grrjkxmw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2twcmiztv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2yygfzqwr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pkpazqee.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2edxvkunt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxjgihgl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rrqyhlae.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2quekjgyn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2cfzppzbm.html


<!-- 参考信息 -->