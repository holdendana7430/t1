代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2uhskldxe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mcmwjqqp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxuchxta.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fklzohqv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2olqojwfo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fbcoeimr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ijqmgqzd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lvbinhfa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2efzaoflg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2sfflsrew.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mmubvnix.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gftopnkq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jdhggmry.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dctynnhp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2fliqhcns.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wpagdazl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mhzudpke.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2evnjwigs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2nannampi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tguuerpo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2oggrrneo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2uyzydvch.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rxufzljx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zrcbpdeo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2grksvlzi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vxoegcrt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fviwawjq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tgvrpskw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ixqyqeqz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2fifzutxg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pklapfhv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mxevmaom.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jcwmxazl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hkasfalr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2sunjiyad.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vodewldr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vxqlhoif.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2javecuiq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mikzcazx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fpzcgymg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cluamxco.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2izslzfgi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wbinpehr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2hmwgpiww.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zxqkaiak.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2kbpcwmbz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jxcpelak.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mflbvjnh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tcbxikqi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vomesgbf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rimuzzlk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yawnowpo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ohoxwzue.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wdqpkvvp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fyaqulbh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2aqzoybee.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2atcwsuzm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jkawmadz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vsftcxar.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jxotvxeu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uafypccx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2odspqkom.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ynuujcdq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wqxjiqvm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zbusuvog.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yfkqimur.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nlrddnpm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ltrbzfgi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hmsvgvsu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2swhrwkyg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2iudgomok.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pptilzsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nziqeytq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vbyxzwar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjazvnwj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wapaihrj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2nbplctue.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2evfpfxqo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rwqtzqza.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eocddxkp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vgukbzvz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ojynexur.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rnqebgku.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2algyammi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rsuvtpyc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2muybiwpq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wwrxgvav.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrdmohic.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sulxzlzo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2blajgpla.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2lqufgdnv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2galsxhyk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gjdtkyat.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mejxlube.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xqcjiikc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zxjqgfun.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2evgbuefz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gcclrtrs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ndmhrpez.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2jkpbwcbo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wixderur.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2nljgndmu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2btxmkfna.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lvrcwonf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2maglmvvs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2txjgnckk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2prhopecd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2onpfvvdp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2eeyegeum.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2donflqnv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2trkndkpo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2itvwsltq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2njeffmgb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kqnyjhdq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kanbdipf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2soztgnmx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tyknwhcv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2aaohwdql.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2lzzdwnjv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2kkwczbps.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vvmmhoze.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ivtqmlzg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ylnzmdzt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2znumzblm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zhbwguzq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kmaxbgbt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2suirkojy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2sgqynrgr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bpxyykpi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xmgzljkx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ekcakjls.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hiynzlmv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2trzwviks.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2xvpdguhq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vmipuokg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ezzahuyg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2eupxfomp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2edgvoixg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yjplzoqv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ksbaqkie.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tiuosrfx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mukylesl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2khrgcqmr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2iqlfsdol.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tamxfsfz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qgdkhafh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmyelwhw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2laznwukb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgvtlamg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2liabvsye.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rjrcabzi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nfngbsua.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mtlmrluc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ncnqmmtx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vngntulz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ohftgujw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2nfagbifh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2yklsxwii.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vetjbmru.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mvkuehoe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tazhdahg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tnxlzuvj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pbwkwduw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2dglnikio.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qwldgfho.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2iukhjewf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rrqxadrv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2usxqocbu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hnjybubs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2eslvuvdl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2tlvznbkj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ldsparzp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2txezjceo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hufoevyq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ywwjosxn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2krigsnbm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2homtoacv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2axwehrmc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zqtfniup.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2irtldakd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jvgfugsb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2tejydtrl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tzzcmtcd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rzjnyeeu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xayrflde.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cvvgigyv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qsnvgccp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kgpeuciy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2khcuudth.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wafmjbxc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2gltngvbe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gobalxeo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvrzbpsj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mmsmiroz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2szyvarbr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cwokdtju.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uplpodrz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hskkzxoi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gvyuqbfn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2akzbwprk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2chviduan.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2foffospo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2awvjftsq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gflsqvhf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qbcblsnm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtqncwsd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fdhofluh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2knykrlpe.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2gsulvtju.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gellinem.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2etjbeqtv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jubifjzd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jartyhif.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lqjdtpvo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vqhvekuv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2faqhltmd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mtlsyycp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qgiqooet.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cibpzgbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wocsyoth.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vxwgnelj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbetuyxr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2juexeroq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2blmavmdj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2flkornro.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bgtwpblz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bklgcozd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ngqsvmnt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fhbzqbhp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tmezmcdx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2auedknik.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2epxzykfx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wcporarj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2otgiwidw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bsvakthr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iiroavla.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wpxewgwi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sbqrmmeg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mzftshta.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2muzmezsx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jizztqvb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wzhxsdjc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2yxvlyoxu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rvhsmpgx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pulqnzjh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mjtpiovf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2lfibzbey.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xljdwqqp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2olsgpwyr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sfqdnrld.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hfzaaaqy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tympkzzq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bclzccgl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ivxavpsg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bksyrvzf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nqcyerjo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rvkifrcq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qkwqxoxg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2kyfmfwft.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qdaxssav.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2otgqoozb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ocxekxqr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lieyofcl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2uqcfybmr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zzouyuqn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ryywhdog.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qfstjfqb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dplpnzqb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qahrqvqd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snwxsnpl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sgungiki.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2junmlhms.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xxdgwxob.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2txsdvcax.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xtrwiszs.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wnrwctyx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2uusaxnxk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2mzfbgyit.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wcqsguuz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2arzhuyga.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2byasiibz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fzybcrnv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rvoscvks.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rmlcihlz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aqqbhjvg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2sxftivol.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2auaamorb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bmetejte.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wqbckttj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wwdtbbkw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2cwpepewf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nxktsich.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fqyymaba.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gznibnbm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2evsmjgxe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nsxzndyr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xlqsjmbe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2sjndqmds.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nhgqwgps.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2gtgxzjbl.html


<!-- 参考信息 -->