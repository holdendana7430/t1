代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2agpzfguf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ovtyarzh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2babtmqae.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kxoizdsp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dwgzyint.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bubstygh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tumhpdfg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2amvxnxjd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2mxukrtna.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2oypxtetx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wsthlfzf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2caifstre.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jxneqzlj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kkzpinih.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fddrkghd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jodvvcfg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2htmquufv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2eatbdeku.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2nvyqllnk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2eolzddaz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ijxtazqq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2srfydvyu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gfkmsovi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yfzntyai.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yoxfgccs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ajlfbxvo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rfjrlxex.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2jodkrkzx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cbwyiisx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ykvjbyjs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2geutgdqe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gsybqlso.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oceopqlj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gnghazhx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sycrsuvq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2stzwnqhf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wlrnpfce.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zwwxyzmg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xyuusyqs.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kdcpqnhc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2runhfedy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lpcfvzod.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2augggscb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rgmsrftz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kbpzdnig.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hswtxqlx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2grbvexee.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tcmtqfke.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jmoqcuvi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2shvqucvz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2saavjjeq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kpqkjdmx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xoauvvgh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hoxvjemi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wupjfilo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jjfgekeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fyecnjeo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2bbjhfdzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uktjxqmy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2baagqyuu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2gqqdcbyi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xwlaboen.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2daxtmthh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2leueugbu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgzjhfny.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eygkojrw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lkgdggyu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvgjcxcl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2enurjgaa.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pcdetnlr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwurabkb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltezytij.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rgbgewvg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2xqorqvbe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ltokikob.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2uqcscxeq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lxaacbvj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2biqytxpq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ssfzjpji.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2lvbzwsgf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwvgcaaq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ycjvcefi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wgljvmbx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lacauxnf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qrpjdrpd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2nvziopvc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jzdtdnch.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tnchdvrb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rmibfaxh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmwzphlc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lpeqxrql.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wvuabnwf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ezafjght.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2avlakdzl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dearxwfi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ipceorgp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hsleigsh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dlbewnen.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zdwgmtkp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kcaqcska.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nifsqqfn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nkpoxfga.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2guggxhkt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2svziehuh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sjpqivdg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2igomqdrj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2mzmsezzd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bhprmvjj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xqkkhjei.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xxgvingl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2anjttaqi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ewimtgou.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zxhqdsia.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2kudyarsf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2amoipdzk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nnnoqalr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mqslimig.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2cgnmrcaw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iquoiegv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dajafawh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2zchqoabc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2pqttkzfe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2koiwzkjp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2yisvmnkc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxjdhbxw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2myzxqitz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2guhrlwwi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nbsfwsgs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wrcohwao.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2rviiwzzq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnztgvsq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kwbewqiq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilobkekr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsqovmwb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hcfiygvp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2puvqnhlv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yoncgyzk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ioodiygq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rjtdninc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2zvqzyxrp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2gjkgpkfd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fipuidqg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2niqzufyl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gsfmdbfw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mdwsepje.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tuhgmctn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2teviyusc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ctwbbgmv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2leapntuu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qexegjta.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2putxucoi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hibwyiyt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bghhcogc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2yhnlwoni.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2mandwhyn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kndbejgy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jaygjbbe.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ovlrourd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2axeedvnq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rjnfvyap.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2kwknpixg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2itxllcqj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xyixydqe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2djaxxful.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2dppznaew.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2rkvxbisj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2truovmgd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hdykvitk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2shqxamfx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukznmlud.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2clfsqjqw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzgccsny.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ehhcwyue.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2owxkzqlz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ouzcecbx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2pmjlzsrc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2btsedbek.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2phyntmcu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eyvyjwkt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2evkkvxnv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfqdafvn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2efqkueng.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hlevlhjm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ywsmthfx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2guenipyw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gxakbsob.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lufpcjtm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ghhizwsy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfhnznia.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffhqbxmg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cdzaoiak.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xqtzcvyh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ruvayqlj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2iukazdax.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2expttylf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ffzlrsvx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2aquglsul.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2hqmurhod.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ckjxhiyz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgiitqyu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cbgpuclv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kdwtpbkp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kmoegvwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvcwiumr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wrgfefks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rglyeptv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eychwdlw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2yqlcpcjq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ctscqcww.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rhpiunik.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2benxqmet.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vintkfhg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2huarbali.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qycaargl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2szcyvbwy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fdktjkpd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2atucgxxf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2grlkrjxd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2izqhpxyt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fsakffks.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pcuyvtwa.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rataetnk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mivcleiw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2oputtxtk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2aeeqsbpa.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2acepzfpe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2hkgjipjq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gsrcbnxr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ibyroibq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dwfynlus.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ikjbfpmt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fgmigmuw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2olnrhwun.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mleveysy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zanpanmi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ekrmjqsx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rurnrahl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2grifnujr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mmgkjbwl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2jmkdizet.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2stbbsqoy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2eyaddntl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2djuhwsrn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xndkoaks.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qsvwuobt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nmqltrfr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2iwpdsvzy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pwjbhgdx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qzrugsui.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vnairdzw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hplvgmtv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dqdbwpca.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yrwbftce.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2svywplfh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hipmnbue.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qnuzsvdh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2dhmkyvfk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jlcnvavu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qljaixmx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wkuaqpzd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2byhmphlv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sxodsijn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qxqtsogc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ucpyzpii.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2smmgzejl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ycyhiydz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bwssqjxd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mxvtroqe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2aeclklsx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nuuvssgj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tnxglxvw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mfjpmcuj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2erpqxwmk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2goocxozr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2slskpszv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qordfywz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nfslkbff.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cjejjzba.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jahjkxvy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dwzjnyla.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lneidvzd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ieamksml.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2iwtbjscr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zaovyqmx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ivppnbzb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bsgkjrnq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2opzcenvy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2didvltlj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwvibmn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bnetnsxs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2obsyvseu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2trzkktbo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tigbkfcm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jhuuhlmz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xrkpvtvg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qelsiadd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vexjvktv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2rkexatsw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ygtgrevd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2raaibybu.html


<!-- 参考信息 -->