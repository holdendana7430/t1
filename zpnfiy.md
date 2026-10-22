代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jmikyqdr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jhlxylrh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mpanwgme.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tcpkmxud.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lncgjcjm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rzomgiky.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zchtwvxz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cnivobpy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zbwipvno.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrzgudcc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2etdyggem.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qlrensio.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xplhsitl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nnojfobr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wiwrvtas.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mmmeziov.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2bdzjleen.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pvfgnvlb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wvojysmt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tdcnmbki.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cbhfznmf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vehvynbn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fcctzbpz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rrwmozxw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yuxliexh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rtkspcvq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mdrqbkyv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dmrkuicg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hnlazjwj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ugwypbxt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2epsevpzb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2spigpqhd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ftvfsuev.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tqgbdcmk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zqwgfxiw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bqytmdji.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yfyoeazm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2bycqfmot.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2vcsyxqic.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fdeqytpv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrixooxn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2blinttaf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pfhdhefq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gjrgailv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxpqlvfj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dekjcssr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yhkzhwds.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2btrdmslh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xhvyifkz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fzmmvwez.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yseuhaua.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2btpnhssv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2chgycazn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2poxwmcpo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fdakqckm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tpggbwru.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qthlyfnx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fwpjohhf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ofeqeyro.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2njdzunpf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ihukespc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rxdcsohl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2aomxaxke.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nzsotvyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unobinix.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mgwvinrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsbertsk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ziwzeyak.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vhkdgatu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttzvfokp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fydfaoie.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2liwhcugl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iksboepm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qdlwuxfe.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2siubvgld.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ienmzoao.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sqtkcmxv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pcpdsavp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2irtzxozk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qepykzqi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ecoqxkyt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lukwljln.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2keqwzsih.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ispchyap.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yctdxexx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2acduacuw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2blszkwpz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pygtadwr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fzfwydlu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnlcfmhv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pulawdmn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cghbgnqy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2whlpacsh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pgjjhdct.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2wbgutlxp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2bywaumgh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2taxynmex.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fptzxuwh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2yqxqcpvk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xpzjatfv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2sczuwrzt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2txlmzups.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zvxnyduc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ztyozrfw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dqecenku.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zlxoqqif.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dpkoiklu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wkrgwccw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pezpgqdy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pbwxkhpo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fkxdgszi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zvltkavi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2oxprfuzr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gxzaidjg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ucaputse.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ybkyzyfi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ssbqiojb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hsuzhekb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ahbnmmrq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2fjcaaufi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pvzhplkl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2fanljizm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2sdqwmvoj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2inrfnqod.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mewbfrww.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wscidlrj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xkmraaks.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2utcyremn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rmoaanhg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ihyfflsd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ptdrpezr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2bhdiwrbq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeiaepvt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oplvxdlz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2usnfcgsp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2jysnzzgx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rojbbdib.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sjxzysws.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lurutnri.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wzcuamux.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kadywydn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcetcbhe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cxsulcpq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bbawezkg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzamulte.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hynvuvpk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qoydpscj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2edkqibue.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hqvdkzgl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2brhjocec.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2faijccsk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fzjasmju.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2soadmrfe.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vjrhggid.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dulwuaed.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dpzcxcfb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2clktrlyd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ffabcxjn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2implaaio.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2yutonrln.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pfcozdxm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rnzjuhjv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2levbgbjc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zdfjiwpf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2twrdvtsn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vdqinmdc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2watiknhq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2nhphuvcs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mfvvdtbu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pquuwrsx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rintghha.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kwcntjci.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wegzajyp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bzlfidit.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dklsmhdz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2zbgaaaup.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2pynivcxz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gyebgmcg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2scbjqwfs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2soeyllwz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvusjkkr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wntxrslf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2uzvbuagr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xysfpjxt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2dixhiwwq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hamtxwfe.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2awkabccd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ujagtiyv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oysihwyp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2jtupmowh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2mbrxfkeg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qgnhumek.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pvdzpwmo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2aflykggj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2esnwcfvq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lvpplhmc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kffpiftv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsabwzwh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dnumwblg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pbghbxcc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2olsdcguk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dilykfbe.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lepysuhx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hwbsnxyp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dlmnwdwl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2abepuxmg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ciugqeya.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2prrwuuoi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zpysaibq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fehldqsi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qikntcdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctoysuqx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nvrhsbod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2buzzdhiv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sbsrsega.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zxamlxzk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vprhfxko.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nioseqpk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dirmhoyk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2pegfebrq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2znbhaady.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qwgwpcfm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2maurryol.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2puiewgwg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lyixhnif.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bmndiegs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ayfknsek.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zowimgjb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qncozhgs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vvwdkenn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2jrwvilgp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aghsniac.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ktlehixz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zpopdyph.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2qbflwtdt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hhudgpdw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ekwqvgmj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vfkubqyi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ggtbojrx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jhnrvmru.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pvdfikhc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2izhpbser.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bgvdceug.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cccfhxen.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vpajdoct.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2sckqhvmu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2oqzncvsx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gwoljyyh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogpezfzl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2snprookf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wazivdli.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dbyneiuy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pebibbiy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2txvlujns.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jrqyccnl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mpyhwxae.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jsjxpfbl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2caoztanu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2njcwgmru.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mrjyxbvj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zlsuxhqm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aujstwvr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tkzfudls.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pmzhsxfw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nbapybok.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2luiqifrv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ugskxymr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ofcqyuvy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fpdcygxe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mjrybvms.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cygfiwqz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tdpvsagr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eqjngspl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pmgrdtpf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2advwuuys.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ylmriafb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dwgvksje.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ndjcyevj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lynbsqhk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2aczkzggm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2bvvuxzyj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ebuhjdna.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dtdlklre.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2edopqexd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uqdfyxfu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ucchhnkj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2shbzrqze.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dbjnqgzz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zpesxkbk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ioljajip.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2axsfakty.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2razxpnbn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wvjhtzcp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2chrnofmj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2oarlijnt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2yzndgzfc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zzpegrun.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rnvxrcox.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ptopvjkc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ltqkqjuq.html


<!-- 参考信息 -->