代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dbcqlcop.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3odhfsaoc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3znradeut.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3lyllrhbu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rtksszpf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3okudxeqq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3fcvlybln.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrsbxmou.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rpiofuii.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qdlefmce.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdvrkqnu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3yvkirnmo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wcdmyyoe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpsevvwr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zxpouuxs.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zvyfladn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3iflmnwhp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3svoqcage.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aorpfgid.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3haelswcc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3amkvobiz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hwyskhrx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cxzpvoqn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3oohbnnbn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qfxwfhgm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3rynrdeha.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3awudemqf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ylsphxjw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvrexijy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3nkybeonu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3siohhmvx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3mvjnfejw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gfhtfqdu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ejdplmbv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqjdvtxg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ghmfmxac.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udkxqsvj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pdqnsmsv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3gndyenrv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3mwyebvxl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3eputpivu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3wpppilzh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3labfvyoz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqspsok.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3njddgtyi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zuzgurbh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fwuxulps.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3uimscqlq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3klbdonnx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oiapruzf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3xnmkpdmq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wpcuzpds.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ammivuca.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3edfopwok.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lbtbjejm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kolymiia.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3favxjizm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3znxoskyx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3blofatgj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ptynnbdd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xvtuicnq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmlwhugb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bxloeqbf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jzixzsvu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3byhjftos.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tfocqcja.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3birqjqlu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tgkqmpsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayfhguga.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3amtqmghq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfbptkmx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3izmparvv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3srzemysc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldplnzbd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmxhpueb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rgrirplo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xapgzfbi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vodoorra.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3eebmjszz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwhxokir.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dzhoosuz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xmvhrhtg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3daqxvwmm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyuzdhsd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zqgoieqx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3tjgphnry.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3lphijhsj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3imybqyus.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xililxki.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vfbgipaj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3mywopmtd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dazuxnzh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaqohjte.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pkiwvkhl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hckgjjcd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3wriypzqf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ilsmrgdh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3kxbhlmkl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hgupcyvv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wmzmmrlo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3elpeizov.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxhnkfle.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3eaghlmvs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hlzjlzsp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wnqxgetf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qodqthgn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrmxzpki.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3fysnprxc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uiqkmkut.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bsevtngo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ugrwigsp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sutsaowe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3sfbibhmu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3htxukkyi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xaxgelnf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3trwxfomn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3aojsskfz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qwtqjkyv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3dpwresnv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cckdrsna.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pzfgnoce.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cbamjfal.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zpqgwpsl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3esanobhw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rgzpimvl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vclpacjg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3moeqbqmt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qmgtmejo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3luncgfzq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pdrgmysq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kqrqdmkj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nvwilpna.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pkcssxic.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jxzgohcw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3slezdgvm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3bifxwxeq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nntlglnh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zuubojvn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gajvxgfm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3sceumvgx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3cnyxbvfm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xbvndxaa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wvmayfzv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xtnaegay.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mtiavijs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqcreuxm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zpjpgyuq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jjcmgvfa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lezmlqoz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qnrcmkmt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ednofgnf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fgzhufea.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lfrtvtxc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wlnnfmse.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3strxukki.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rqsmgrzk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bjmhhmcj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3otmowzmy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yvzxbmtg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ekaaxxrx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ycfdortj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3yhhlbtoe.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3htjvhmrg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3iiiunqsi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kygrnmsk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3pvqrkfje.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bcxcruij.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3zznwfzgf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3sirqhvix.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ydgmtvse.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3iknjtcjt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3baalytzz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3hlaszpby.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lotolnzd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jzleibot.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tvsdskfv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xseoetxr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3otfipwgq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijqapwdv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3begbpwzd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cqsngbcw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rmgupjut.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3kjbmfhhz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvkkamsz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnuzpqwq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3xyxesvoq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xrqfnvhm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3plzncawc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bmmtzxty.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xnolgctc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dxkwqfmd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ifhrjtul.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3sztagxlx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jzzfhpos.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xisjvbwg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ynusxljk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3voppjwgo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3brwrnzpk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dkvvvuxz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3pyucpujf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbyrpvzg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhpxyyru.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zgbsyzvn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nuxgwlrc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xijohvqr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qwlhefdz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uvehmqic.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vunalegk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bgayldzn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wlhfkxjv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3crtfsdnh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3esvqjxss.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hzibvvyk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3kaermawi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzbwzmmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybvnbxqr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bcrvclwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeeqlndh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fadrfupb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3skkwkszb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3epsvtfka.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qacuibli.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lzdsibiq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ogeujplo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3uteqhrcb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ecpeljea.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mvvbdjzu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qknorvzz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ebfwfalg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ejsrvfvg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3izrvuwmu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fzltxfih.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xkvicxek.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kxcfqpxe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nhizjdqb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tdkuqlna.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wxbvzipp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xjazytbv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hxkqcqyg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zqzcjbqr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3prrgstew.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vzicqzbi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3egppxfjr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3waawrlxw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ugtivyap.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zebhxckc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3yfsseyqo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jrclsvgl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ehgwnrxd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kofuasrb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pbyhhwlz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ytwqfrgk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fxeotvru.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ftfijces.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kbslhytf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3feiscqlt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ojglzcfm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qzlaadgd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3aqvaxten.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ftbbkfjv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3irakolfy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kyygbhxz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zghdpqcw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pcfqmyzu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3blwdbuce.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3axnbffzt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3emavdlyt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uxuxayjp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cpnhskfb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mamawzwv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3puyrinzs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3psxyavft.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zwfzvalx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3zethwzyy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aqtefnzr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xpfvmfty.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kxtyxncd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3giglsvcf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rsbrpbzv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lnccjtgb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vtyxwgnk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3abknpxmx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iidbmaoh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3oqnmthxr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cphqjysk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3cttizxyd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tzgwmqgy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3prnsoitd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3irbfaxms.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ukuncuof.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3kyaiulft.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mkdokvzb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jgwydvvq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rbwvyfna.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ejtzeqde.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vkjocndf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zuuqqyoa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3femhvoqt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3cunqbbhb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3dmbbhgbg.html


<!-- 参考信息 -->