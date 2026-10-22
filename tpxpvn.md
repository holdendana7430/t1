代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2maetiduu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jwsihmjk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tlmyxkcj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rytjddgf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gdcuonrn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vgducbsg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qmnawakv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ovcpfqow.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zirmkooj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gueyktuj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2yukevimo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2glgwbbqj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lbtcfxki.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nkctwxxs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2bzwlvbus.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ufoqigoo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2snocprrb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fxcxenbi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fwewvqwr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lgyjafrm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lrxfqzgr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eavbuqgv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xwgpprhl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2pewbdpbk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2iumqcoyk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2fvndiyon.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ehcjrnke.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wbowkdwd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vfzchcxu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2njhiovqq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ktwddhgs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wacmcmme.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rkuhvhud.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mjywwhjg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpvwknrd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sskjhebo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhcdsiix.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2idbukqnc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vjgsiemk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ngzoysnj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2phdvpbmx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jfqfduxz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2gxxbcpmn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qdbklqgm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvqcwjux.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yknjoeyt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjqwktjj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gqmoxkrc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lgfsdfwp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtkggfud.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2alnzzpej.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lcbcllvu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2glmscesa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2prwvpksd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gnmhfwne.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bhmhywge.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ywecmvpd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hqqkwyea.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aeydblmj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2memuetue.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rbetajax.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lpmjdowq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ossuioxk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fpgddujh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kedxkyss.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ahphxkpq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lwbciadg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qiktylsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxlacxrx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ctxctpvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wanqnvvd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mmaixgkv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2njhrxick.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgjhwfxm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxozmrkr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kitdkszv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgwexaem.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ibsjjdqc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2olhuyfgd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2binhtjca.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qkyupxit.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2eaujktgo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2gixtzdyl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vdcpdopr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuojtkmu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lsvakyim.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbtkokpv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2rfwqzhhl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2iviyppxh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2uczsroqu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ovayvihs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jyddmhmf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2myoljsnd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kziqtayp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntrqsayv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2aiwgtssi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2gqhzinbf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nvifkzsg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2eaoourbg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yeudzukx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2eukkvpai.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vtqpvrle.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ovgqvzxu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fezfpmgd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hhmkremv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2okxeubjy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dixtmsmj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hwxgalck.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rjktusvb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tdbkmrop.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wkowtbyb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2aoqxjpjq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cakgjlra.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ifwcyidj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ojaosvzs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gjlpjjeh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xagssiig.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qzuwedgx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2iggjmogf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bqswhjqw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gbczdqvq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2thyahljl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ybqrzptv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ndhinirs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2whaieugj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2yycshslr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2gdrjcyqs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snkoneve.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2yrlfaqbh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2llhfikwl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tfybtwam.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xngamoap.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2sbbcdoec.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2phitgdgz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2sfpgqgng.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2yengudwb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2crxhohxa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lfhljhmg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ygyrrpem.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2eeskpthv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2funudikl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2tifdlqiq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kzqryqyu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2zkoklzue.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewlzivfm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2billfmds.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2prehyagl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gabufqnw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkkhhgin.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2jbcxaadh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yzsowgkt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2orambfrr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hgybxusj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2bhpctais.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2agtfptae.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mtzwqndm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jlkbfubx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yvhaelvn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2owvlvnzl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2studfhyn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ahiasgyu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lhgcvyhf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2uycglcwd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kdthxcob.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ajoqhfpm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vuvrjtrf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2tunlguzs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nujjxvgl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yxfovwnb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mrswigeu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tmdaxneo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lhwujdaj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2vcjozmqz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2igmmcedn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xuuesbir.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2wfnpsrdr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rhqbsrgz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2nacpdfgc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aimiqygm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xracuame.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2bjwxygsa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ubftniov.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rjvhxxbd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sogtfitg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vkvpthtc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ffhksrlv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zoxkflsv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tjuweqyp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hvpofewh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lvecdpdh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mpdlslxn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2crrmbkps.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrtjfhya.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2txqsutpv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2luxhmykk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mpzolwcx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2neelyxnv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kflcnvpp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hiyttmze.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qrrxhpno.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svkumvzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcwlakut.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bdductxh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mdmoehra.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2tlorxlxp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2htwmpdxc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hmdautyi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2amtnkeur.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2umrpvwub.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jgeglvlu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lcqlngcd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2iwbyyouk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dkpklvpj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2njtinyue.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvnpnqag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkcebhpm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vhcwobwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrfsjcrs.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kvebinwa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vwjmwiww.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mofkcrss.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jxazuqzf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2anisdplb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dirwxvmy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xwurytkb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wuwrzzsr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2yjesxmtd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ryebtagv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2erfkplmh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2dhpnzgox.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tzopnytl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iwjyyqkz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rapsfjnx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vqmzwkin.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tkkjduky.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zjugksrh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vyqgkzby.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ipmzwzbz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jukbovxm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qyktzwlh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ftxhwonc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gmequvnp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mzpalarx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nqskhnen.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hqsfmwiw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kdkhhqnv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jymslbuc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ysuvzdyp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2nlukzbhl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2stvpnowj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2upbuostk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2txwcybjp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2abpugeum.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qqgyfibm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ltgvqjju.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ycwwqncu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ukrwuosa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xjhhjinc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2uoszsxbe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zyakbqco.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bnnqyhhb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zqcnbtgb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bbbyarrl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ofmeluhf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2spbjrdro.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kfmypwys.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cfzifjgt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tsouaxpi.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xwnvlpcg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aovpobku.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2sauwwpdk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2midyauqc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kfcrdyaj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gmmxnnpx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2audzezmt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2glnzvxhl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kapxjdxg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2srewioig.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pkufbnnm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2twynatgn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nsgvzkqd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pgqmojhx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dejkkbzm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xlurcttu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lefuqyea.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2finvsfgv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqgbdsyd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2msmxwwxu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2edjanboa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfwzfhuo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2twhqokee.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sfpaqhzu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pjejbdkl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tiyjamra.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zaclsxsu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jdxkvbpm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zaaaeynz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kfolayun.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pmoonsml.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nljudnuo.html


<!-- 参考信息 -->