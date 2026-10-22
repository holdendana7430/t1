代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysraglhe.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2vtrgzepj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jprtmujk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2euqxdean.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2yiyjoqhz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nmcgfrvk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2odszuuql.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tiiptdqh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bxhphfbf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2curihrih.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2frujbhod.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nbbfkqcd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zykoqnoc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jabcgxbp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wninehwl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hfuyctwu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2huovhopp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wxyxdypd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rwhcqqau.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ogcmeofr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jdocnxpa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kfmmdpme.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lmtjiulw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ivmhgtut.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qptzkxxv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ujhiztxy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lnekwymz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2jghpwayy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wbmhgdmj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ggfylgen.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2duwywjso.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ppuepvcy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hirxulrd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jnsfejyk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2dqpltuub.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wnnrztaj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ngaalcgx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2nnzczzuj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2huxwxndy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2uvrmovwu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvhhbsbh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tyhpzwab.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aaiygkhr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2izmrpkfn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ozsblplh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyyrfjes.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2aiwhkdwc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ernnltok.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xlwvazzx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2txjtclcs.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hpxbjdod.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2odsawmdn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fawbglgz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nsmquqbs.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2noqzhidh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ivqurdfm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lmfupbwq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpwqrolx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vaqpkrdv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2synxjevj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yqfcakll.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zxhdleki.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vqiipivm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xrnibcqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcvaqvxw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2oaebeffi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqlvacxj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2taixhvfz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2psuqoiox.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjhrhdjb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oytjmuqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydmbbwds.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zuqoqaqp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ldriexxv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2hbszfocb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ersdnxce.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2iupmhhwo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2aotfcwgt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwmhaezx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkpsejvl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kagovfie.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zzspykae.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ketbpoyv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cmwhklcm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2okdqthqv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bednrfcw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gaumtrve.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2gtxlwwqf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2krwdcssb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkssciaf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2txmshgkb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lrbtiqwl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2yerdyybj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gmxiqvec.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hijwkkox.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mdzvzpkb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2czcjnkdd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ickpqzbd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2yjlyldgm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2sevtegxa.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2axsnwyrm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gzjndiil.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sfogqzsi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2irlqkwds.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qcxmwapx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2gjqovaun.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ycxogwdd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iwgywvvr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2whakkcvp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jjodzgho.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rjxxoawj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2avcdjxyo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2santgjju.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2nwahpivb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2jwtqlxmg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dnnvggjj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pafdoctw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ozuewnmd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ycwtprhg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kwkzeixm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rnuwnhsx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2absmejkg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zslbgtri.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hhxjemer.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bduefmxk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hwmushzv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gylwfqwj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2cpoyloci.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2fanorokn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2iggjmtka.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hetvdivs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2dospalrh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2snwzwmah.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2weepjjrv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gicognwn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ltjkxhea.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nopjawve.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mivcmaaq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bpnxpqjv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ltyjkbep.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibtjyxll.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xowqrhmw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2svqkuive.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wuszuneo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vyvcfgfe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yymfxmna.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2epueekoc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qdujlgtt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vkgbtmsx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fsxbztio.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zyjznkyn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2btieahpk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vflmpgzi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wckvegnc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wvmdguwb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ecnlsill.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ctiwpnke.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jttgqfmt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bvsswrll.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2diydspea.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wfrfmrrk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mnaxcxgl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xwvafkhc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2knnjhuzl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wjshrozn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ezmnshrf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2caupgrzg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kbhlyvlg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2flrjkych.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lxsgefyk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zqmzatus.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2arxsnopa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xulklgsa.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2noloiycf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wwonmgbc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jddnkbva.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ksaazpbu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfxszdpa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2laqbpnkj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqboeaiz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nfmlrgsd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mfzqeptb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bjwbvhat.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zrbdvohm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2sdeofcft.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2tnfkomeh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yltfragb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tctmrxly.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ehkiqfvy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnufcuqo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2aflqreqf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vqzbpdcd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2yqvieaki.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2pdvyvugz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xtbmnnkr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2vecffmxx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vlhcpyux.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjcttdau.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fzhlamlc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oeiomxnk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jzxrhhex.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wfycsozc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dijubiur.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2oyvgihoq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rgpersod.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2txhzqnmn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lqqbhoku.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pplxttxa.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cvxzuolv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jruahrbp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmpfokop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsjrktys.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2srawtnrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fejnedbn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ndjvcsmn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tkwlfush.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2whuwwkqw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vphzbzrf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2opjqavhf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ltqiqvvm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vfbkimpj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xbgfslwc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ouxshzwb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2suozznlu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2cljbohom.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2rdxfiqbo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lwdwjbfd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qhfqgosg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xrffdeom.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2szgvudfc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ygktbrph.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fpvswrkd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xxcelwsi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pwoanbct.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nvtnnhlu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vbxfprph.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hspjyacr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2khdfxocl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ygupjfqh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2umukepha.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2htrbqtjl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rdejjstu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2csnhvbfp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rgkbeegp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zxlaever.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bmifuuox.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jntolpai.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dnatnxdk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhzgbnkb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jofdonyd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mqezulwd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oilfxtqa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2esmtifyr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jevtztsg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2cmgamxbv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2fjawofmt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ygcgtnrz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dozajnej.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tvlbpqit.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2riqigssn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fdstqimm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2opgaqohm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lngixuhx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2volkrohs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hemkohum.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijhfqgjp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2brdiajqg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qvszjvna.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ayyltlkn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2oyqiymir.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tscemsfu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ynaohkoa.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ycvpwenh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ojtkutua.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2gzcamxys.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2pzgflsvw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dxvvjhcn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vewbdpba.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mhrwkfxx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qbzrklrs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2aywhknhx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2yevuznnr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iffjvvpq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2hjkeljmm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gxenphqk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ufqpvuit.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2logxlwko.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2giwcsvwn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2eciahqft.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hgzygcbm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vchnspzv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2enonkuij.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ghxxgkpn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bmzrmaxp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ccwzbapf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xasuwixs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wjxcmfqx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xqpdrlsq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xhpfktzd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ubsdouhg.html


<!-- 参考信息 -->