代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhetadgj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cjpdrrhl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uzbbsryd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ozecexbf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kljxixjo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3elruutyp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3gisdfeum.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqguyfyo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ydjhyccr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lxbzduum.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3rynvtsbl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hlfllfcx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ilpvijyg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3iapusjmj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3rwbaounp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nuakxyhi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3lxxosiqx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mxzmaaxm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fixeqpvd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qcmrbjdj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3epvvnykc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3caqvdnzo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xjjywaog.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zsehmmwr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ejxcfymn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ujcpqlwe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gvwjzian.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3emotmoit.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rsceipiv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3trzssaik.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3apoxywhg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jwxybuuy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3biysmgft.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3oyacrloe.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3lfxjixlc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3tdgcoxnf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmafpjij.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3upiyycrd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bbhprgoe.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3akaatvhq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fuomhhod.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ylpgknzb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bwucsmra.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zutuxhjr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wewmcqty.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzmtrcna.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjbcekec.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkstltze.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxohzgxr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsaqhxcf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qqvsuneo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zapwugit.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wqtcllbw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lzchtjdn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3neyfckby.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vmqauwfh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qbcfolrw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sljzbitr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sscenucu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xezjpald.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3sdoycqmg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3vaifxkkb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aahayqhz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xdftthdd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tphzjeua.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jzdfctpt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3admfxxhh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bqxhixlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbfqzlkz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yqcwamzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ummefjzq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vpywdwrl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3urjccnfh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nkbrayjy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nejqbvlo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cwvqbxva.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gldwcxkk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qywtqgdw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jufwqqyy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gdermeae.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ffncvvnq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3srzgdcmd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjakakic.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eqwbbqpe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoobxlaf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3aehgzqtl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kbofuogr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kogtovix.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rlhmmffg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zatriibd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qqocfcub.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkfjqqnx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bapgmjxy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sqyelikx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3skhejnsw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3thxyxluu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ocfqdrhm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3rjzbrvem.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3maypqqtg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3kgnlatws.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vzilwqxg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nzkpxuzc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tubzvvfx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fotjmqqm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ttxwjbzv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tocklppw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyvrdtjf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xfwrtsus.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ybmqivnz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3wqouamza.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tkgpyvaf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yupxxkcp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qbddhmwe.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tnyqvsxa.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zeiirkqs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3yjbewtji.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3xhawlozh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bzpjmdbx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zjglyrrp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3avnucuah.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nevazrez.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3psbrrbxv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3znskvdsx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3czorpgef.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uwlcmcrb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3cgijcaec.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3askijcwq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hspnuqqw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zfinocri.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ojmfthlj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hvhjzgjk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3lobprsyl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hbtocvor.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bdobonrc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3folqpndd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3evrntbep.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3iytnzzbp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eheshbee.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hsdhrcqe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ugufhaoz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hmjzurvn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmllproe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kjrkfddo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lhqfxtor.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3karlsjsf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gqokjmkb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3snqsaxlh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uuvydawh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rbtlvdoc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3piaunwip.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jncffdnw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3babjqyiq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rptupbhg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3nbetwcor.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fcqavbsb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xqjepyth.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qsfimflr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3licxwxfm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sdrybqwi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3pylqfdhg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cxohamjg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3qjgkofyf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wvlxplcm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3niqfoqgc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3sbnviier.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zwxbwyra.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ljambxfi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3iplqwnzy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3maharlqf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vvdiscog.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zbvkchyd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3zzpfunoq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xdackejx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rqtvwzur.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kwiqjewg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3delwphgh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gazgnqfs.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3govsqaxk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gvxrbtwr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3yrpmbbav.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nxevkavy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pgurqwoy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pjgjxnrm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sjvdciae.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bcdzztli.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ughxxeuc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pmetyjxd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fzfigvpv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ympodqmx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3atdvdfkp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hnhkhazc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ofmkkfog.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvptsvxe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zodttpon.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wdwrxezd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gakvguyp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tgbgheve.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ttxnkvqc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3lesebefh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ooqqjbsu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpagdvcq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ylormjvv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yjurxloz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zlwtolot.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ichypzzf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bvrabdza.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wvhcijfe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3frucchsz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3gsewqood.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3iqtnwnho.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vzvddmjq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmrakeua.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rtdogefe.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3icczoymn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3swdyrrkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfhrtoqd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hrmcfxwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwebbihx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wxlrpixc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3uqkfxbsw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bpujgsgc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bckylurx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yexkpzis.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3malfrwtq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jxecxfiv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ehwujwuj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3sqzvukmi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3welyjrmv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wpuvntxw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rxnpsjuv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hmmhwuax.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tkixdssj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zwrnhiyn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3alsmcnfn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3yvbmyehc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3eivgkeyn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bjffqbmo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3raynfpga.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ezopbddy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fcymlbjf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wqsgehwh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jtwixacx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hqvpisyk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3swwmbtdm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3baqeutjh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pemsvskl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fpiiczdh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vrxboedl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yqpgfeme.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cnibrblb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fdhktrzz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvfkpcc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gqwrdviv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fnevpaii.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ripiusjt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uogtedyy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kjzbjwrn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rwrrwoss.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zrcrvudr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3dbiwleuq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wgfyfqkj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xwpsymry.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tdfrmxss.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sitfpvhf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3itbpfron.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekndfsmx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fvwbkpsy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dnqwpejg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3mynzifyd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bqeihzir.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3cmavmbju.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3whqptngs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mmuvrfsb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rjswdbfg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nyuenluj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vmcmtzky.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cdxxucwx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xmwijicq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3sqplkdxo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ipwtfpsm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ktmghpov.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3yzrtoxfa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tuydbkgm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fulvlbcn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vptwpnin.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ptqakjil.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pjnnzbvc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oivdjdsk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3viiarnov.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3orclnpjc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qusgejok.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mtueijma.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3upcwkrje.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3agzaxymu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jacflcbi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3imuhhnkk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hrdwbjof.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xieqobne.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jkhcqcfh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ldplpele.html


<!-- 参考信息 -->