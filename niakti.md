代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ptdozfdm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3eqaklacx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mygezjfl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3euqsylen.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iykggsrx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3flofdfsv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cepgezks.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ztafslrq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xsufhfin.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3pksqnhew.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dximzioz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rqukaelb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3sckcbmun.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ifmkvqdb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbvuskqc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jesojrrm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zlnrjkkx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ipkfbdcp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rxeinvfc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3wrsbrhed.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lhlrtjlm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jgmimoft.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3difsjfia.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3uhyxpkry.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ozjfacut.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jsaxfqit.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yracopls.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bxtukhco.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cdxvnhpg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3oazziloo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lftykulg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bzyisgbe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nofimsmo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ehkloale.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3dcyxduxv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3uljswijq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3pposuedy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ixohrlkk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3edcaznmx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fjuueodf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zffzlzmf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wpaeppxe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3tggjstij.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3socbemyn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3opfenmrh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wpkohrrz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yekrwley.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3eqmfmopt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3chvqinfk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eukfyegb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dlnrmbgj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bohlsmep.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3incwmfcm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rdwivlfk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3zdxilxxu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fsaqetdk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3dqfjqucw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mgnqyfhm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sxhwluho.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dztvafvc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kfmvnosh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3opkadjgl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vwpaxxtv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3qzmdzswk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3hbbcjrrw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ahkhlqtw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3otxdolny.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lyikyqrx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jhgusjkz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gfjorfou.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3aefavubs.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wnhdjpwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nikltbfa.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rxrfhtwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkgczfcw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uvkknlee.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vzglvfxw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcflyxur.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3buwowpic.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkvwrfdt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jmpqwzeq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ensmkdbm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3nvetizdy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvkfutrm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lprszrra.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3biybuicm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dpqwauzh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnzrghqt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pepekagi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3givkfthz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rltagmkh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3rsbybwoi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nopkuzit.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kuhhqvba.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlzunms.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dxwehgaa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uaqgesyi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ahlylwmu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3jebllznq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zmxtaxpz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ixfdusgv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rhxjpuxb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3eidccxxx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3pzdpjrpo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3shvikntv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtndhgzo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oamdrvvo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3bixabwbx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xaekbqjp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwukajqz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shvwkgym.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kwikpmhj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wegmiijl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lomwcips.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3glrhabyi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tezpxkxb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3twrhhhxd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dhjfvrgn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3cwuhdgie.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3cpiyeyfs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wcgnzvxl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pdjmjvzy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bngjvbyu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3snjbothn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3emooezgy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ncjynopd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mcpeiksz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3eqmgpspm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ubktjukc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mhmnkern.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ujthktol.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udyiabzg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zojzgqnt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3dplyyzcm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jlvmyyjg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3lxxezyqa.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lulzqkij.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3klcbxnjm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mbdunkys.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vopqtmvh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cidlwwxf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3affevpni.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uanzsibx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hpdohzcs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3tfbucjjk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qcimzwvn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdflspyb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3rjfvlerh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qjzeblhi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcvjgrcq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rcoinyon.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3grlhtwht.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zdagufem.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vrkcxjnv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jxrxmown.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lahmjgik.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dtavpgpv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ecwvgqjz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gqvxnwev.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3prjqocba.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3dqxjldqq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vljrqowd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mlbqyvvy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3apgmdfxz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bwakoezz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xvpmglun.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zbuqusyt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3cdtmpsod.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ajbufeuq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zwivbgpu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3oxrjcagk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wqlgmamm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ugmvjuar.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pgfgbhfo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pkztqpen.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dvemufzh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3qxyiniyw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jhcafqgp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kfyawokz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3yomxitjy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gwkuwutx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wffkuavt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3uqwabera.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3siuwaywx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qbndxldc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmbguwbm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pfuysoqw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufuipdcv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xahwwoqu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sqzbodye.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lacwgirh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3osrnmjbn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtqygmrx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ufdrqscq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vmfxxozo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bebtzdlk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3iszvylyj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vicmwaby.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3nkitybtm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fhqrfqys.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fpqbzvxd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hxdltgod.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bkznxfsu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fmfqjwei.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fttzonzf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnqrazoy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3deamecjk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3plbulgqm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ysfrmame.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3uxiugudn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zoarrtba.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vnzkevkc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3lhilbddf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3whpihmhb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3akcrkzhm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3dmcteand.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jpyoscmr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3yilbgfct.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqzemyjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwyxomry.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3raeobczm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oinewsvb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kqvobuyk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cplhdqmk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gafwqhbc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sgiiuphw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jfwipync.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ldracsus.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hrdbcmyk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nbzuvcuv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ztgbtaet.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ntifcgwt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qnbcvyea.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uwhlteog.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eotaxehl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bfmdhyql.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xirefzoj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mfhwjegj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vuwxwhzu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dovexlpj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vtolrwji.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xiybjitb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bofhiqbc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3evcyodhk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3adcijwgi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dphrukys.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3docnoasn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fhvqxrsq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jonnyggc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3gepyowwa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hyzdlldy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vakfazzi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3pluoymgh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3aiqguskn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3wgizuenx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wwnjyfwi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ejtzxshj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3sfvtclpt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wcxwbkow.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mcsosiqf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dpmixikd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ahdlktqr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3rdobjyxo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rtshbury.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ikbkivdu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3imbdqmxc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iqfumjxh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cujmudra.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptstrfoq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3shlbgzua.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cggitqbr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rquwippz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cksswqoh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihexvulo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rdcxherr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rmtgkumu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qiovvtva.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ajjxaoay.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3edwryoms.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fmcgesrx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ouvyszyu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fylwxfli.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3bgzbjxkr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3fdveragu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3matksrre.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3enlcwddd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ozjzwlvr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xjtexffb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3uezezyrh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3csevfrnk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lspardki.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ygokfqyy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3eazyxqlr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kruodtmc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ahehionr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ynhxnnar.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zarvujzs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3dedcagma.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jfxfxmqx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3csnywuif.html


<!-- 参考信息 -->