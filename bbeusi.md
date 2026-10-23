代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nftoaeqh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pzcneayz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xicppvnx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kehwojpv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3frodfbst.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wwqbxaqo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3iduzsoee.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3gjltkyaj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3frlfyjkz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3limakyvg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgpbtcrj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3defvafdx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zdbbfsrn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ianfcfza.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3voyaksnx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lhtsbhwv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3uljybrsc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3txjcyfba.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dhktfxrw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ntxmttto.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3aainvbmd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ytmvgauq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vlmggnpu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jhobxbqd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bbmuvsyh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3wabbtrqm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lyxrsqkf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rlnyciff.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qskkbomf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vhpcssvj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3frgyufty.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rktdvhnl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gryrggyn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3krrarwdh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rediikmm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jpfxxgtf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xidchggs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xzaqalqx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zgijnfzs.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3allahocr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3eatchzts.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3tqlawkxj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wypwpncd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hiczvoyc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hwotiqpw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tzkduuph.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pachwmss.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xejfvioo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqsjpmwv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zantsjfw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xyjhlwhb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rlkdnrzb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gseiftqu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jjmrwiek.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jquctyfl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xzplldpu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3szcpliww.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pkzrludi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xcrhfvep.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tjfcnxyw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3kmuwdcxh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qqiinzzk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xbklzbon.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uivmotry.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sgvtmcrw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ikdkwgxa.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3yiaoxlrt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3anvdbufk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwljxrog.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ayapcxhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmwhanef.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tusyqhxp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ozrlyjrd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltauaefw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jhpndndn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pwazxgrr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zegtgbik.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yukbnzll.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3nlvxijmy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hvpirjkr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3nxdrnzxi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kbgeccyt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wuunaxgy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sduuliim.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpgfqvjz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cehcstto.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxbdisyu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bzwqlzhb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vjwnlbur.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3uubvqlwv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ljvgvjgj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxbbqabr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydvcpsdy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iccpnyxl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3zmyyglhn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3dzsvedzg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmirtogf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zdwhzkog.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3mffjqlic.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wiyvoojk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3yipaaufe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpjbtrst.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ywbcxnhz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rlruttak.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ckcueqio.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yfoifuwj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cftzcqsu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kruquidv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ctpiujav.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pzjvtafr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3oginjzvw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qwgdaayc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3igiccbfs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nmyhjars.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gesizyjx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xwbhanzt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cwxziqat.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3npevptqe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jcetbstp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bbtvplfp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bdmyrrjd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3lrzgjqhd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3baslpsok.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xbiycmwz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ugerekjv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3yezaeyij.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rfluyoas.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3flifrqvu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3futwsrvg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wczdxfyx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3gfnzujul.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3iejmbisn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gfozbkip.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wpxrrimo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ydefvrli.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3czpajchq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3udzccken.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccgyffwn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xmdyftyp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3nxpkmnga.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mkjxkqzd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3yfojwzwr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3odxsulwy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ekceyams.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vqwgfwza.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ggujylxd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fpubdfmy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wonagrwi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3irsqvcnh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nkmapndj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ihtfuiqz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qqwlvbac.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tkguefcc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3yvdrbxym.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3tqlvhjxz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dwzjqlnl.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zioytymf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wiegiuiu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3edfqgruo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3grttukrn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qbhzppbm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3pfolhyes.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gmtqwlzg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nvkqdhkw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jvcytdeh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3mjvfwtuf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dlcoilhp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3uiodmcac.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3drtnjsni.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nasgcalh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zpahavkl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3skamhpgg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zhuxzuqv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ajojemra.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vnzwftxo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3hpsiftuo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ugwighrr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3qloazgfz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbvhtneg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3malooker.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tykpeapx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aruqmuai.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ulfqdrpu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrkxhcky.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vtvfwpdd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zgfrbzoz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3owzzankh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nrccrycy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ofnfsgru.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xrdmtgpq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xmryfcfm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jdmjevcs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3nxalmjic.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzzwwlim.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3chwwyxpi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nopszhvf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3poddkgra.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ppndtpeb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vaevrjcv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3olpfaubg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hfgxwkdq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vukoblfz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vgukndnh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wwczhuvy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zidydima.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3eajccsbw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3lptueoof.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pznbnbzr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3luhhnnyg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dbvbcjsv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rnsurdxk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkrrtmrq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tenobnno.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3yonqpdqk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwaqutin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqkynfnx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ijcghoyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjingkkw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qtkanilr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jjiyvyzb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3igkujywg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3okmmaujb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ktjbucfz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3iypxfnjh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3npssmcoi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ctsfhjjd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nlkdknix.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3yrqgmqbm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qngcruhx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rjrxdxkf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3phzcgfdp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pjjwrnvp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wvpeuuxd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ixidyjrm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3akzzjuvy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ighrryef.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wndoeznk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uejgqwqr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3rmcddiyh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3jcrfzdfo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sjkaxage.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dnaoehfa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3iicibdlq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3emhbjzwq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xtbvmaei.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jmjzyulv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehjdyaci.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3izptfplb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3qnqfatvp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ggrcjzif.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fqgvopkg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ozbceiuz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yyifbfxs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3tgysgers.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yuajpwcr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3obatnfjv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ujvmpdrz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fxrxvqhm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3sjmjmrot.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xuefjxhh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aaoesggt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jimqizrl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jntvlaon.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3avcoycna.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qgyjnmim.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3maacfykn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yubwwgyu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mgdmaoax.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3secauttl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dzfakemh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zcxaceby.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3cchamoxg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ucuvshij.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3qfjpdlrp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yhotusrv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ttbxtyzu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qujiqyrt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ppvomene.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3reyxcvlt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wcdgvdsa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vrjbbmmv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rlsojtvi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tftmktxi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sdeojgod.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cshdpowv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lthxjcoc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wxshemks.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dsfsakpx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qafjsanx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xtzrdvkr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bajxyeba.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sjmidgob.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3azsmvlvg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ahebwukm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ozxxnuii.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3bnpcqspx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwabpsb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lrobcsmu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3sxjvdkqg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kgnegvyt.html


<!-- 参考信息 -->