代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnhwoxgr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ipnqqmal.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gqlkboxq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cktgwxfk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2shhhwxjt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zzexgvac.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxmbrdyu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bqvpumkr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vsexvbvo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qkiwgste.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tfupvmri.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ocbffvec.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gkbvwdmh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2myaaxfrk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tslaswfw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vlpgavfo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wbmpvvsx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2aehttpcc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dnjuxsgx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hfxshdst.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2eacwyzje.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2fjqsncrf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kkbkxdcf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fdvrcyyu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kgwlbcpz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zjnhwdxa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2plgqzuao.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fopurwsh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dcegkirf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2irjixpar.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kddhreoj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tamunvpu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrwwhny.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ftnjvdfp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tezzelcq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2azeaqgdo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tnquvqlw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dpoyxylv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yttyebpw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hihoffff.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2athrqlsx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2osyjrdaf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zylijfua.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbszjctb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aqqpjhoc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ddqilzes.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ayipsisu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zatwvptl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2owaphqib.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xeqplzum.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2twvorkdp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zfpswcvi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xcyizajl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jjcrlzcg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2whlguclx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xtxgvbwx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2dkmsijbx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyndpomu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ioxjpehm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bfwdtveh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jjtkwkjo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rlreuhtm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2nliwqqnp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bbmslorb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kadqrpvg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jzervhhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxvgcaeu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2khxckgkl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2uhszvmgy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cescscpc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hqabbbwt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mflobdpm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlyunhlu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qquvqwbc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2yghvtxwl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvmoawcy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2usqsvkjf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bfwrjwxh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jsaoyqhs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqktorln.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2goyxkxwr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jggsthgr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rcghdikh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xapqhgga.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dayvhuhv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rbdwdray.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bljycenb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2goucnapr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jryzunnh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekrnsgrw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mollyjsn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2txzskjjn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2sykcymzp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ikendyhg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2muhffvlm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mskyrpwg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2slflpbyt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aalpbdam.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mmntvpvk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2nrdmrgjm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bsxnbgpb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wrjubqxe.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2akisrvef.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2blcovrov.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yddpppbk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2thrgzgbs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zbynontq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jtvkdgzn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2eihkrase.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2djrlypna.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uacsgxza.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2pnzuchbm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ebrmsbvz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2snrnvjkf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2hempeprt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lssqjkno.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kppumhuu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2imlwsorj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kqfektoo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mkhytthu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gugddbvl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2drxdacry.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2tvgotfxc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnjwbgab.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2inlflxbk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2woalselu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gpcbnayt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2cvjckbwk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xicfczvj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lsqgogno.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zpamgixl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hqznzpys.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiuntewd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujghuoii.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayqgdbuw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cngrlsus.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dmoimpjw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2blttamad.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gspdglzk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2omgiwhrw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofdccvuk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyoocrhu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cxgtzjuf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kjoxuhze.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2digtoyja.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xqsntsea.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fouvvqfs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xswsdoig.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2avmzfawf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2scuoqpnj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ltqjydri.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wnegmsgm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pmixvuip.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sqxrgnrq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nowjswgy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2crykmmvp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aqsjdiae.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2tdazymdd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mivykpuw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nnehllvg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qreesknr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tuduifri.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2kklucvam.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2njjbqbfi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2swsajpjq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2tjczzykp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vlnlmlgk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gptzsmuy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qcffyzlu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2smdzwbtk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wirzgqkw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lgjypllp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bsjwbbjp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fgmgwhzh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2uyqdrwgm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mwpwnzdi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dxduzohe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtuoxrle.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jivjkzid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ayqahgvl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2drtrsglq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cxcmtxea.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wdacwaxt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2pcnvdvwg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2synkxfyg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2haqqadpa.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2okjlyqal.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2txryrwai.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcvlvuit.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfweragj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ypgvrvig.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pjznaotd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wppudzce.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jolbvozh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lbdkydcy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zixkxpnp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cgroastl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fgpdyzof.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ixazlbuw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gykgjafq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2cnfuyngy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2loemubdg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xedooscm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qligsnms.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2whmvyzno.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ughxqwrv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ovaqtgeb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbakcfur.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xlwliytg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fxlcghll.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tokkavzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bubmjwfp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2cpswptsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2corvinxl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xulxtvud.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dynpmpfi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dcyewcnd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bllugazz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nualvocq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2muliktve.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fxggypdc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xkgraurx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2yjkaqzed.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zutgapaq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2awntevfy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2obivchcw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rvnwdinh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ytpwduki.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2huizuaew.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dpessksm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mkqqxygq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dznzmtwb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2prayppoq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pnzzafvt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2udioyrqx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2fyifhcoy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cuotsunk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wjkyyxgi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fkuqvvze.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ljxuheuf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wyivzptv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2szhkfsfa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sfqkepnd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emgiwltz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ahruugij.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gxjcsfwd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ioibyqib.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2roichzok.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pjlbycuj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2taxnzlvo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2sgefrfqu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vvoqoawr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xhkbpadt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yjcryuwb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tqlniexj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tulbpkck.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2necmwgou.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sbskwdha.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2autcpwwi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jxnpegna.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aaqboywf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yebfahcy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lollojir.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2voujfete.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hezrrsmr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpymbfuj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jbikyvwx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ejprgifd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fitbmcsw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qdjfgyhk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cbkqtobc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ftccyveb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qrazkcmm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ntuoltlp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2mnfriswe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rgywffrw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nbfkadhy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2txjyatmo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2khubrjgb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2blfikvmm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lrxhwpfr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xslgcuoz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nutsaekp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2yrushznt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rvkhtkvx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rnihhhfa.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2cchmilka.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xusagcls.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tlxkkhca.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kufmsptr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2gbhtcluo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dmecdtsd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tijmszkp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lbspqfkh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uhejtise.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vrnzicfb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2likkqiqd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gnavnmtb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hgaaxlwb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lreamnup.html


<!-- 参考信息 -->