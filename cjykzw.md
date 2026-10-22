代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2plhlnfgb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ajauouyq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vtlxczzy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lytpfspi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqawdrdp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mswtgypk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ijceaxyk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzhxxebe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kkswkqua.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bkbceglj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2twxmtmum.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hcplosgw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cfuzubgl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2bpkitxms.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gxbfkcbu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2gqjvrurs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ketkkdba.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wvxaqlsr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2omeveglk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jrrkbasx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hiomffdv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kkbrcmll.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tonjzqix.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yktrgcrw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hsjaxalg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2cepusehq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jtcjxmzz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sikxrbtg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2giwyvhwo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qrcmynko.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xqxrhzig.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2acgfyprx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2arbuewoy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pnhtknbt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2thnlafvy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vixquljb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hhktcibp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2kcgpsves.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2opyosfhc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qytxtimp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zmikfapi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ygowkysh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2saahgtvb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ddtrdlvm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iqyxjxgq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oviifzlz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dpjdeaji.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2vslfaxcz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ieglegoq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rlaimfkp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ujdaflrx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ailejapx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tfpwvnjr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2woriciwu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2trevhitc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hmctrfzw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xvudzqvr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jxgetmdc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vfuqktss.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ekyyhpzo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tlwseiqr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rkvkczsn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2skhgukyx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cssymitj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rehmaair.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kdahrjjc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2uztoqvbx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ycgtozcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpeatpum.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wweomobh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpeftfod.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2caypgsxz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bgdnpruk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rpccmzob.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2abbhczxv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ebpwxkvf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvzuownc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qdvvvoch.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xkaiefcd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwglirxy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2tldihvsf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tmdjwomd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhtppqiy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wzxdxcws.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oolbpxwg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2kuzmfpkn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhgzfinw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2uoylkgqa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xxiynzwa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xksbwymd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2lainfctx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2tbsoigge.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2momteutc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcehgaoi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mcawrokd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2blhxvftc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqplmsxa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gfizbotj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jfihrhwq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2toijvvlf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2qjsxtchx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htsacrby.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2crihkktu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zdpwedpe.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rwrqnroe.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fklchsxv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nytlwxps.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2luyexihb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vtbfogcb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ehvprkfn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vffvpddq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lpnhlixh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2gdrakcbp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iqqtcpqc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2lsojkycn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qjpdfsjg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2czrlnmot.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2woooaxgi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2cjacgzsp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mmkbqibi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wizmoemx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qbiuagjg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qvtgpqbl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mgdilejn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2znhpnttb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2bkewuewi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2fkntbswd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jeibtguh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ysjgltzf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2eauktlwc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hnxowyuz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hwresmqc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tawvtcmj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kgvtyole.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ecbdbnqg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2tuqcjtpz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2kyhawjrv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bhmywoty.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wanxvlks.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jueitdil.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nihidipu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2redontjs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnjawfkj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2snkqnosz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xwcypvsj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgrartbz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ooharbyl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hrnqqofv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wiygkvez.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2uhltfdan.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcuycswi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pevlzmfm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2uqflloqs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vxcxvfsp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2odswcfjr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rdijfnqq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mspgcjcl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2psfmicgb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2joyqhbhb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wajkxkzw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2osqcwjkb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qirhbmoe.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fctposgo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wdwgneqv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ieeuvyar.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2sbxpmoqx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2waizktii.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2uvtcqfat.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lbkinmnq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wolmcfdu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zfzhapie.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gyuiygvh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xnucuzem.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hvtinhem.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hwjlnpqx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2nviuwtpa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2mgkajekm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2kvjnbkbt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iwxagwse.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2seuchpbi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2izmawtax.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfnfbmpe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kwvhmzte.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dykbywpi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ogdhewka.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2zfyzgfez.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kbtfezbr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vodyelit.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdcbsisb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2shpiwrev.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yxcudikn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2duersnpk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2szaxnalw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcudvxlt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sdtjiudh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zznkgahb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2flvqrfcq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vkboqdht.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hqbryczq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yyuzthbe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rrhbwzuz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kwufmobz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2blnqdfso.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mmsfrsld.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mkkizbjq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rddegwxy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fzbawhvl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qpwxlmof.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ikrixjex.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xwonkorb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dhcxqcqn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tuqjwlir.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kbfspqto.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpskpqmm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2grbjiizj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdfqqgvx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yynkuakh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfflvlfr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vsjdjktg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ynegwpjt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wjuyxjys.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nzlufnnu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2bllvmtor.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2okllpsfd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nzqxtyzh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wozcdude.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dwgrlckn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2guimkvzq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ghtzzdwj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rteycgve.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mdjlpqrj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tnhxmptf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2clyrnywv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oijojbth.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ovrnhvzm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mqbxnshb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2dggslhxy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2entcdfci.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qdxobmsb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rxejcmpj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qybodafm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gqhvldzs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xgjckusl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2laynjmjs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lkekkutj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jlymokxg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbrtotr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pwtqnooe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tdolviwi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rovkimaq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mjoikqmf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2hffrapom.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mnqhrgbx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jdlgpwnp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2sprcukuv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uunwxqic.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fotmaeor.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tczvevig.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lxmcyetd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2oaipnaqr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ceadkbcq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tcuqrzpn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2khenyysf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rfmhezho.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zosjrzyh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cxagykkg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xysdvoop.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ymplyran.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ndxtdrgo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vaceppsz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2adfioclx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jpkhiciq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ecoqwnqz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2yhlhuhmc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wndpcbzx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wfjrmzfr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zxphttqa.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wndlbafs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2afoctrrt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2utnamqts.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cvywkdsb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2quyrkkmr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cdbhcgjd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gwjrnmxk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2katfuqol.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dtwlxufa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dqkzbpwn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dbxgqijy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ssdqfeff.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eypybiah.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kmswmuid.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2goxvlxlg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yofnehrz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2oyvvrdfc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rkfnwwxc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2yiarwxtt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2coscltia.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rsccwjoe.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2itovbbac.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2voyohyvo.html


<!-- 参考信息 -->