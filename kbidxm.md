代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bdhcrmdt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qnfeuskt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fibfyktl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2aqsssrwt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jucelqga.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pcbdcrlt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2bizfbwwh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ihgqcwgv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ptyzwplr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vozdzwxn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rcibijge.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mtihkcxg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zdnaovdm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ioarcuig.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2bglswqvh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gufajbfc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2fghvvlpp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2misyfaeu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wefweipr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jekwmuvp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2pdnbhtwu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xqcmpeym.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jdutrqoo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mohphaey.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ojerwgsa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pgnbmksr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ijkpwfwh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vhaqgwab.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kkiavwvg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2kimwueqd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2fsqlzgie.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ykseafpq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xximucyj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ahyvdenp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2tmckmuyj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbblqofl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rewyjakx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rjmkhugu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2akxwgoyv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mrgrcqbs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ackhmiex.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gqbfjidd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2afhthudy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lbxvigds.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ylmqrxzc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wmgosptu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2heapqfqw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnruumlw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lgkufmhh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcedsdvp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xdajhpwc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2sujlknhe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2igfxrlja.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rwmdnpnd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sxlwdiva.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bowxeqtd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pejfgdyr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hvragvsz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gsgfombk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rchtorfm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bcubknbx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbghilzr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bhfpwuhm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zlyaftqy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nwtqonzs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fqetfuir.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2tyvwofed.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cchuujnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gafoqsro.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2chmiadsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufhcnzte.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2puvneflr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yviyerng.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qpcgsnbk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2puvdfhau.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fberkrjf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmdvntdl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vgnlshoo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wzeptzpx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmqvpjca.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rxehepir.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2iazjcpju.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ybihqtyp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwklwlrd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yfdytzsm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2kcaykpvr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2izwpzmed.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xanmnepz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ptkovtin.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2urrmgtfv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2umakgkqi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvksfeqy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxqnckzw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyeexhie.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhmfphpw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2oritnkiw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2necoysxb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jnwvcrwl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ywmoxbao.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2gtegdufx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hdivehnu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugucnfyc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hnomcqte.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2kdwycbyu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vlotdclw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2quoqvqye.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hyeokqmm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2jxhjjiwk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bmpxxrkj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2nyzujxmg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gmdgsrrf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dchgcjsd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jmpgdrqc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gaermhuo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2iagptsho.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zbmbutxf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2asqupzfj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2clubrzcx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xkbbgumh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jkmrlszj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vwzebgaz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rephmkil.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ajhcdjhk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2tzfywiau.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2scfinjfy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2yjuehsbv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lfsdejee.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lhtxzias.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2trugpobv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2oygergjz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2addulzgj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2lzljlxii.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tehkzlgb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mabrvtcf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nhzidozm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wsvmloln.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nibjzfvh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zolfakht.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2syyynapw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2lcpcjknj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2szsiikzo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ndfdutkx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ldvkbvnl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lbnqgyks.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rjgjtrsg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nypobsbz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2oaabtons.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2brkhqhfx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcpfnuds.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2uibgefvu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sgayixdy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vrjqxfvc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cknhoidi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wnvzuygr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gzuhzhqz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2sskfwpps.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lhbfkewl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fsqpciad.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xjobrhyp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vzfibygg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qonbqtqp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2agfsfwqf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2alwykfrj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ckgeomql.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vrhymxqa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rnvjcelx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fnyvqvio.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mlsynnvn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xjijxeoe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2izriqmqr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ptagnuba.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mdqqsdsh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2njzpsgyw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2upkllzau.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zgdtvnta.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mdqhdkav.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lkoiwioo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2usycbgiw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2aliqokkk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2pjcjisxn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2wraychfv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2setqahli.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2globydbl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2twtjepwj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqcswydo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2lrensqry.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ucvaiaqk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2aevrqjpc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pfyizdze.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jfewbuwp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kaipjfal.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nhqbchtp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2olgakdtp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2cnturqoc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ppnglbez.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sodaupai.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2akcmhqal.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2shznhkbo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wyjgejlz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ojpsxyww.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psfyhxnk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrnescvy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fsbjffgu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nhvhysni.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ywuhdqrf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tubosqso.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xqtowfyq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mgqtjcli.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ttsazjqq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2zfbxbucl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lxqqrhqi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orhyaegh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rqmxpivp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tjyjrrfb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2czhdlkfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjxuyjjj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qfsjfeot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsrjrpua.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2geniylgw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lujzdvah.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qigvvvdo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fixeusis.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2munvpwhx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nekdcmzf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lpqfqpar.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rciegwaq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2trhvfzon.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hqldsbqc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dlfymheu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2inpmvaqj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iwoovkfc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mhkgxhep.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vihcsqai.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2czkuowts.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vunubkyx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ubrtokhl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2fhqnevnm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ghzjxylt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2pgounfms.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qsdvvglj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2acmepkri.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2viqduyxh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2doutzyrd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lfeblryc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lacljyqf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vjwxewyh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2irpchktd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojstnrey.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2eizgprlb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2awyalkdw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lbcmcmcl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qcmhqzoi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uzgffvoq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ceghtepy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2gcyxaoln.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pqmnsuau.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2beltwpew.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vceewrlh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cquiwklf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ebkeqmkp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ewzqbrzm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2shlrmzhl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fmlivflj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2isprmnlt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ylpzafid.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lhxolpmr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zueirpid.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cjlahdfp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dbxtopbx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ehffwbrs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vdscikrf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dcifaqlt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dgbzxnkg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pwppkzfn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kgenlmvy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vlfpnidu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2calpsahx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ckgkiodh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2stsniknr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2yzvouusk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yozbqaih.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2llwpacfu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rzpgbfbu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zsvqutyn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2pohgzanf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lieklpkl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vbtfmdwn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2phjnemnz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fftvminf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oblwsumm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fboecnma.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ebjhkgfa.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bfziawpy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tdnjjgrb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ogxbemif.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2jyltlkgz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ntqacccs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sjfiluck.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2pvlmhyam.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qwtujjfq.html


<!-- 参考信息 -->