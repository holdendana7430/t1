代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyfmujig.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qowwcvsp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jcdiqwsd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wapphcsu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ikhvanxn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2clscfoxo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2nrziypie.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zmkdbmch.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pxaeifio.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bswwtycf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvonxync.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uqomfrld.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wokqzzir.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2fueokdkv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2sqvparvs.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ecmkxovx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hkuvljrq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2frcozjjq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zbasuzzq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bzjqojkm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rahrhnbu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jdobonjq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tsqxqfei.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dyorsajv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pudjxegd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2emutbezb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ucclgfhr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fhbrqbbe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2npgvqyyr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2napprrlq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2oqocwqrf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2irfscpop.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2plvznudn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2jxdqbojn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ecytowcq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2frbklvgo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nadbdepd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2uzjzfkui.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2oaxpjvbv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bhsgozek.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2wqelofqx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2aqyfspon.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qsbyalmi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hdcxcxio.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nsoucpcn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jiunpujv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxoejvbd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2riwbuopf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmguqbdy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2petkbzip.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2cdsluiki.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xetaxwov.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2cqedsogn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2edobksgb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2btnxuxae.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gyeoaxma.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jbvrfvef.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ziemmqyk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fmawgqtf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ohwcqjji.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2oefiicwd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekpvhije.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ucggiebk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2peowxjay.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nenptewo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2izqxbnem.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2liregjsb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rebnkhxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czoicynx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cpovlgby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyapudhw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2afuuvoyc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xpierkzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhnxbnkm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kkeqpxys.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kjbirbdg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hkjnwryi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ckgzwipi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qeeygujs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uvydnkhw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mmuupyje.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2htepsfjh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvbatfcr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2suftqjrn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnbadhql.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xvkrjzhj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2idiluycn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2atlrdomi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2guqgdisy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pklivgrh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yxmgqrci.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2urzlidew.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nasgejqf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfzwlnah.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryqcsawq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2snxotxms.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2btfositc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pkidsjvi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2lewvwoxc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mjtyyqud.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2igihvcjf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qgwmwimj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rhkntnpo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2pruvsssa.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2erdrmavh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujwjmjuk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcpdlvjt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2oegpthvn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xiyppbtw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2sftorfpl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nyagvngr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jjuvrdto.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2crgkoifs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zowftnzt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zljdxbai.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ebqccnwz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2aatsblpr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qtuhvsnz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gzqyamog.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gvyrrgvd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yylitiii.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2awsjywwd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ozppcdem.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dlxalnax.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2syenwprx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jifketqn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bsxomvth.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2taakypid.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xzkjhyrd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2elqupyvz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2szvvlfsf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2enmokgfw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdwpjfl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2shtrbajr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vdtpoljk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2quaamdej.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tsfoicpf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nulspzbz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dqrytxxm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2trfqigao.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mitfxzwh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2aptfeqog.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uogganmt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ikpucxbs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uucgeqcz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xzogvirv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fafqzpmp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xwrtyliz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ocbgbmoa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cgjmvsaq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilsbryju.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2giwcsohr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2rhjxcywi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vkrfomgh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2okjkuxzm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tspjjmhh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2inggvgfo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sknuqsek.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mizpsrpo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kfbjzxfm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jazkcguq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2teoratft.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gxaikseo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gsydvbrd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2eiwhujzl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vqticqmr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2tkcxuybl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2yidrnvnd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lfrrcmvd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2srejdxqi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2evpibiwf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lwnpmpqk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2epwrnsdd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2baivakax.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kbgolyeb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2saolndzl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2irpzbnnj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tkkzdlja.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2obkuiloy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ildrxoeo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2aowrvdqk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2usjmkzyg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bdxojjbw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2czuvdgxq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejdebrnw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2keueemcp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bvlvcqkd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mdeslmeo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2lbebbqnw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2efiexosh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ufnahwkl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2klyxmxdk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbfdfvjr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ustrftkd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zbggmyuc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wwgxxvkh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ihjpqwdx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wobtaqxl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gypjbsum.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2oqmzowsu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxtqadhe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywxbafir.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wcciuaps.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bhqqnshs.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xhuqmxct.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bvcerhqw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lwubotbo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2voaxsuxh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qrbbofmd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2bmvyctxu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hlmmiark.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzwidkda.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jbvzukza.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ojljaonp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2fhfpdfwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fihmdyel.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2funydfvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqxvjyik.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qwxrnrmt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ixtlasha.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2sdtbqhjz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ucwgjghe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ggxfohtr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kejmykoa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2upqovsxb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cdxuonto.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lmfjsiyb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ehurbihm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ovlvznqm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2zhwjqsct.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2slkdnomn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2faozkjjc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ibtutfcw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pmabmzfx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2wvxwilgw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yjuqmjjx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nssiypym.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2blaebfox.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zxwlubbk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ycdkirzv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wadbfefc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cedamanp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2shnnyxtd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2tyfuizjp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wghobzaj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2unexqnmy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lapndvnu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ptzxxvdq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2nhabpvkd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2fzljfurz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pmbyxlrh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xrnfwcrp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mncjdyxc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nwmhvvtb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vfaxruiw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pzhilfva.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yexjwtce.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2setszjkb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mflzpyrs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tihoiwyf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ckvywpxp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pnywyhbr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qmflrhda.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mzcqbmuf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2haltvayk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fnruvecx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nlbplxuk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2iyqgrhuy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ktcsnedg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xeowvepz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2emmltnig.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2syiwxkod.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2axyszlcx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ybfdpqzv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eishmfsy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ikvovdob.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2syamuesq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2awepjcpn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2abumumqb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lxsbvath.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2efrvbxqj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vfivaoeo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2cijvuula.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2gkerefzj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2luipzvae.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tqrvizxj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oivdrpjs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yjusxptc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2kgpuuscg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gesdcmcu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wqxpoenj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jejcjnsz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xiehoapr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cqhponru.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kqlyvwfm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hggfgzus.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zfmmygbr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tsjmdaqw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cnrhyiyk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2upjkooxi.html


<!-- 参考信息 -->