代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yuxvrmai.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lntwezrf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dgwkznza.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3dyfuwgro.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ivicbzsg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3zpryiuvr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3picshkgn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ktvqcwyp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3swdetixv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vpuvsyus.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3jwaexmva.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bbmqwwty.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ewmsmqnq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ifjzfvsk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qyqahmoh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3voywopgm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jkpmiuiy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hnkaiych.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wyvxfiub.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvnpnqgz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hhzcdmzw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wjunawfb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qjgfdhyc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jaroyrsc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3lcflvrmo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hxhqxllp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rydreoql.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uytuhted.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3abfpljie.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yxkbidty.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3azddnmil.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lqtlfjmp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jsnkpyod.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pxlwxaxg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ewbzirkb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3odoqasyq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sagwlxoe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ksytiyge.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ifeopton.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3spkgsavd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3zlhjwcem.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xxhrdort.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rqrgxsvd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rlerrijx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jzmjfhyl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yomcwmod.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3frirzrhj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvoeeyc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yzcpvqvr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpwgedyi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wqrrxyru.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3phmyvzfy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3iaxlwtah.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lgrexsew.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yztqxjre.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iugtqyqu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nbpmavkn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3adkxdyxq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fbigxppo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cqcbydft.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mxmbwqkb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxnltlev.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mcsqmcjw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ywsobfcl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xbdjoiqh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yiekubae.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3yahyijbq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bisytgxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqmgwvqk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uzqcjpyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxoocdnq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qwfthngx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3arjjpixw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfqezzio.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjyaadvp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zuiovfme.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3inuxphyx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pjvmtquk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3gpwodhox.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3roxfewta.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zafenllx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3utyfqzab.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuohfetw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kljcoasc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtqxzzeg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mahrmelh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3iwjrynhz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3irclhquc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hnejbdnz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rrwkucke.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3giydfjhe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hhbbfwqw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pdasxnmx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sdyowbal.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ieuvlpgg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3exhoiwlu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zoigiggd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jbgmourq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mtzemoqo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wrmdvbjg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ssaojomm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xbauskqw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pliupvdt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3nyjfjhgu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zafwnmtp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ofgniwzr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvuiztgs.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3tvvvrjuu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3reyqedex.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uzbzbsxh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yzthemui.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bxrgixhx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bwhqdpuf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lqufcuvl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qtoqacdb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fviabjes.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pivqocyh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3oycnoxjs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wwcwwzga.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qazctiog.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gefjlmfv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ttzxhsxn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3miokayng.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jyhlgfyr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kzutixos.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3clpqfasc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3kzoeueei.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bspbhbes.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fqkwhjdz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ukofoiwl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zquadydw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3zzpfuzae.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3dozduvcq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jmzkczvw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3nfoyrzfv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tdwzszbt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvjhdnhl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3suogzpbm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fshyidcc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ykdlmxjf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dugfulub.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ehthgnex.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieuplexs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3auaexdxl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3arsqotmv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vtgtofly.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xtakvluc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uewhaams.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqzeybfv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vfbmceng.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmvoxapm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gxcndnnp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ibowshdg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rabjttqh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ekaezmgo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nlymhzfo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tqrcvura.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3knktvbwk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3analupgg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fkhoouul.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dswlhrts.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3eupkbsij.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fhwulcrr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xymsipls.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3brdtkidz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rvusvwsy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xbyjthzg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3xsxaombt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3bkdnolvn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ykiaspmn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3dxabfbkg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sddkuaut.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dwzzckgm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ntetiyld.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3saxpgjlq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wtxgbipb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ilysaqpx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3eyiiysuw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3effqrazj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3atdowwva.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ugyxpeoi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bonzpuws.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3fgstpgcv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpgrreub.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zazmjgvi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pemcpksr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3fabxgwtj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xqawkwxn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwrpnmai.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hwammbow.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vfrwlekc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3npqngjzd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3doeauvmj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lcylykhn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3nkmtgfiu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iniflozd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3njlmercg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3oriqsuho.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xubrdbvi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xygixhqh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnxzbozm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytrkmali.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3himivjdi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ruloenhj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qojawdxd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3irtpurlj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dsfbugpm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zequicxh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fitoegiz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ifwuabga.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dbzenjoz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvzesgdm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rglbbmjd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3pjiyyjal.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kkjyznnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbzwqwab.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ocfjkvon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtrotmfw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iszxuguw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3kfagcyzg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hpaacrot.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mvrwbzuf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bjtvixxc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uqzjhyqy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3toacnmwb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gmyangyu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dnhkzxyf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3amqxzerz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lhjybjpj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ifaycftd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hcdxhpmk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wvtaaotp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lmxyeyub.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hjizxuvz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3usgrouca.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wfyznsrv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hyomtdfs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mfreixwv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wztecmsz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yfubjkpg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jgwypzyp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3depcnjah.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ahfxrpyn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3isxbwlpy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zmtdhhxa.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kphfuqgv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tnuxqoby.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvmwbnws.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3yokwkcxw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vpuiudnh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fjrdyafv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3foffmiux.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3aimdxrvy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ainbevif.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ayrobpqj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mqkylmjg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hjenctgr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xcqsfleh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3enfvdpbz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bigrymbx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uybolafo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pedumltq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dpyaqvid.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wubshcoe.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hayfnyql.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dtfvirml.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ogquhvqa.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zgssmznc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vkadukws.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qpjodmev.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uczjmmxp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3tfqrwfor.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vnbuwtpq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tdelzprg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jstrbnsy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dtrgbzlm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3umlbwoiv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3knylnfjx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ymrbtmuc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3arhfivar.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3inrnsfxv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3yodmfvnh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uqxhuzbv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3sbdeiffb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bfhujsrg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3snfxcsbm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cqifbhsb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3nyuhkijo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3frimcxta.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pckecguh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3lgsajsmi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fvwkazlv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3luiadjmx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qhmyclnl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3sbrwiudo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dwovcvtz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rjhhropm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rlnlkdqx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xjzykbev.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gqwnlini.html


<!-- 参考信息 -->