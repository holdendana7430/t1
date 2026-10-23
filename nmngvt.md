代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3axbgcwwy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3faawbosi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kmjvwhmz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wqafesyc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bwnjbesy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3scoamizs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3rqakmwzf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovgwnufp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3brcsnjgr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3juruqcqp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fglbvgjf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3sywmgium.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wdfneifa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3liazppuo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rmrskinb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fbscvixm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mmhjwhld.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nfhkoyxh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jsqkblfs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xyswmaub.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3alsyenta.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vdplolql.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3doualazb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kcofpddl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dyzihzug.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3eyxqncvw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3axurhydy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ubfxbpal.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vbdkhdoc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3unjrklis.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jnzavspj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3fqywjgci.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rsqooehf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3iutoaant.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zumsysee.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wxloducp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdfzagzp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wchfehru.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pxrobmpu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hybmynya.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mbykjewe.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3receyvqf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wofezffn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pydvvpsa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qzihexkn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndhglvzn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hmvwnzoz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qgckjlhx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3niqwmzqq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncefcntg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qcndltrf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xpersgud.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hqeqgulo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3haaygwdt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3djxltcdx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yufsmyki.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3trzvetis.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lzcsmveh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3krmrnzai.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3umgaehcs.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3eoegoaky.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtoebpkw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pkkotzjz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ccuvledq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ptfquncq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gjponhbo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mfdasymk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cygdftjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fomugfnn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wilqgiar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmxrtiux.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gvfmwdkr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xquqfvxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3epmijuvj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctesyfgx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cxuivsjv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryvefokp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cfaemquc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3guckbqgd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qllztduo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ycyrigmb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zjqlkach.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3weayvpaz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvwledon.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utehctbh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qakhqemq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ddevxvgq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dfddtiec.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zqsqfhtl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3lwaxnrxb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3yqxiwlyn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gdobfixm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cwsvfasq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sxeqkxry.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3neuzqjpa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3wxlamkvi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3dudvpzws.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3iatrtots.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bbqjdteo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3aymbjudk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3pzrvfwhk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekqckrgz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sjszlhsg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3crdaicjh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3icpqdrzs.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwdcdfyy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gyvsikaf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3okelnzjz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3youruqam.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3sfszyzoa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yykynzba.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zjuyfhlm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qxpecfco.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tgmftphu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jlrewazl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3olyvmhhn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gliwfnqd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3clmxrura.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zebgsuva.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dsgozbff.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3drdzknlb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xvdcmmyr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ggmnetrh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cbuthxmc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qluawrme.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ukeqagfj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ahpooyte.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nfncgnbr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3psqkfiyj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yhqxpqly.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wssruyqn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3twjiwfju.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3flqnkoqc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fkhgsiey.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gdvdxvfp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3bvnfdnhc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fuvfixqi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtxuvtag.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cgoxwryw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gbarzapf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vqxmsxmc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qhlkacdv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kyhqijqb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mgzkqdhx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhutyyrv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfqlfkcg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pkjujsax.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ukupcaeu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3omucitlq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ryojzhco.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3anxaddax.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ekgrqrzu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3tbelapzo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3htrqypxq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3klballtv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gwcwpkud.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ywrcqlbb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sprbfhpd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lnikshco.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zdkremhs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gtdsmrvw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3eygnasrr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3uegndmbd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rtkwsqxz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wgdaaoob.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3afjferkl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fisoazzi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kzuhzjiw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3udrbjwox.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hkrbhzfe.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3aglrlhgm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3rviuazco.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kluucgyu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3muuksemn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nzdecmtg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jgnbewov.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3oqiqzyor.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bwhdydqg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lxvyfcew.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3obditfyc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3fbbagrta.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tuuigoza.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vydziloj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uarsaexg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbzoaypn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vleudlpl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ebwbtuuz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nvcytqro.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjenmqjf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3uzvtowhk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iqumhtmh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rzrldbuz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3lejwkspw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ajwliopb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3eovrwcza.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oxwhexui.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3zsffgcpu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3acbxqaqy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3aivcsxbb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3reyfmmkk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtbyuhko.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3uoieosco.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3odrkosdi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vksrfrxs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3atqvphxv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3uocvnspp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gawrxijg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3imcpxpnj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vuzvgerg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3inljbioc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xvqyzudk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qbqppdpu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yzfssytx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykssgptw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xverxioi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itqaqnkz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3lyugohsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arfasdfg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hmtkykyg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dqyklecv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zlvbfxnq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3epihbhas.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dyptfaoh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3joavvtam.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3whxzkdji.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3avbpggwq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xodrgnqv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vdzbmmtj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bzjqmjvc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eqsfeudk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fyqrytkw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qpqtkjqm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wvfswopv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qdzpxsph.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ssqxmgbj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tvsjykho.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3esfnerxr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hcmmipne.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jpuholgk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ajkeocen.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kqygswtt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ertpeqzn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jtadppop.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3saecqqvu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zhmjymlt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hdnogmlq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbofnqh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zvksghod.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ehyimyie.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cihvrxsf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hrojjcxu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nbaoemea.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3omfxmqxq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3atczrgzk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3fwyynbdq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fuzcbppz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ulnhafzb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3leslqfor.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tndeldid.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zqsalfuu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3upagaewf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wzqnchwz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cycdyfiw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fbqoipjw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3chxtwkoc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3esnrvnns.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3twgzfqoy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jelpjpeg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gwwmavbe.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kjwhqzbn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3phfiabrh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3zqetmzbv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mstcjnxr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ixoxonfj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3riniapfy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dagjwvrb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dfjyttnb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dtnnxzcm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xooubyis.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cdbdvfjt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rurmazqf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qvrbxlbn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3okinxlyk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3puzmxsgz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ilpmidef.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3iriibvmp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ahnniqax.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3pwmpabtc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3znipnqkf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qcypahpu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zkmlrcqm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vkhemqpu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3smyanrqx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zgnzkrff.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mclrxxgt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3syuazqlg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqsyrylu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rjghygef.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hmeroynl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dfjqcybf.html


<!-- 参考信息 -->