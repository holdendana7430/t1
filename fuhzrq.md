代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ieljlzwl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2slzwituw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ckvjdsya.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2iiyisvgw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gigkdpgk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hmrzsplk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fqhuajjo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wydeaoxt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2grbugbwf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2aekajvnw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2vlapyink.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bcjjmhhi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2nqiryjui.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wdqorufq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hwpvsrtf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uxfflvet.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bsrnfnpy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uvxxgcot.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gyoppsnh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hgaltyjb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gykkdzqp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bqhkvtye.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2elxnjahh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2aszmwojz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2aarfcxgl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mwapqiav.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rcbpqpmh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vmogjnls.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hmhttkwl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2flxnzkix.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fbkampdz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kbsqmcai.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dslduuwd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ewceyqou.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rbhjutlj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ontcxbnr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wfgccodt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ucjsxsmn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pzebyhmx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lecwjxmw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2fikmixyf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2tiapdnut.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mfctgoie.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2pbgguyya.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2watijuwm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zgjdksnp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bzmjcygo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cbhlnlxd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kkhpxzge.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrgvxrer.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rlarqayu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2pmktuxvd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2agbmhrzt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ocrnzheb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qpkfxrxg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wsmrtkjv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vewzhdue.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yjhwgltk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yiesvfot.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2baxnvoid.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2aywdsyjd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2zewqupaz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dsgkdysh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fosguhpf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iruyuezy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jttmbavo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2gtievydr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2raxemzzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhusodth.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jxxmrvun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2naezyofp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xjuvrnuu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2devnqepl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2umcwipwl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2imuovthl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ulzubwlz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ujrkwaqf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vcptdnpm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ontcujmp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ricozjzc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wjlzbtws.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hnllqcoi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vsnhrrzi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ncfjwfek.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ikgvvtto.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lymjtzvo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2pxythfen.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2sborgzhk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sucxetrr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2dazcmmdg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2reczlpia.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wipzbstf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fvntakkg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfiithjo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kmdwsiku.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kgdhkxht.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2gvaqcpgh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bjesjpmq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wftjeiac.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2oebycpff.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2rmdlscky.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nncsjlil.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fxxgjvbc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qupmcelc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2kubnvoel.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sbjivvfc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlyednox.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2quzqzfwg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xlxixxls.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fdjlmlcp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wfgfdxag.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sqpjuwba.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2urvekcog.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rgsjqbjo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2sfrvbqol.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nbvkzwjd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jcaskzwv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rcyhqzec.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ftsybmmx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wadyjjlp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nhvekjls.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rairjdxp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2llrlwpft.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2guqsghwu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tpgyckdo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2gfxcqumv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2kxbfnzmt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qyhzsqnk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zssvntyg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ximdigqy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ohrpswkm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ldjbozsn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qsddotim.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2asblhrzk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2mooubewb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jcubebvy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdjevgjo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iyvzetmk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vlnwkbll.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nznukzei.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2glrblhgv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qabltwwa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ikjshpju.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lquzvzji.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kewhjdga.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ucwchien.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pwwjbloz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2buvsyrqr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lrofqlwe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2luhloqqa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2orkpddat.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2epwqrpqw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ilowkdjh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2hlhewksb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bmhxstwa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qeomxoej.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hzuvxctq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sxautcnm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wgwwajzh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2epitzedg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2quehabso.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ttziwwpf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wecadhtt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2rbhrxvfw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2okrvdkit.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gxvclgsp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wvgufmag.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jisesctn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2aysbgkge.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2dgnpkxzj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hbkdkapo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jbvkfizo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dycnxctv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gmrhbvum.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hggwcuan.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2axhwqodg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2aukkibuo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2vnkqnjzj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ylglhqgw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rjgjqswn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lddjoify.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2utjywuuo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2phtlcojo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uctfwpwg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gylgowqh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cfpxpypq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ufgtzbgw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tktmucgt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wtjekgiv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dqjsarei.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ftckdwro.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mxdlnpes.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylggggzr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nclrfegr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hafsmcjs.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hhjzcsst.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nmujjwzn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2trcmlurr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2prkilcrg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kasypvwy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kpsyoygz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ihukvzbv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2iehurpuy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xjovvaqr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wvpqzsoj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pyztnjyy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2agcyymft.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2uxaftleb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bmibldlp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vnljkabb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yunitroc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkkxrbxs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2wdoerfiu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bftveqgb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odwrotwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujnjkqoz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ibwiwepk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kygrdicv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2raodzymn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2sfftrayd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ngvhufnl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2glbvnfha.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2htluagme.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hgnkbpwf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2moovzqvi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ahcnarfy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ejaltelh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xkleqlmo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zmpgmmxd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yisvtgmm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2azlsvkgu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hmikpffv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lyahdwvd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzhzdwt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2aivljydr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jyegxtli.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yfrsnhip.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aayaxfsf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jhltbvki.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2aflctjnt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cnrjsrow.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2himgnawt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gwrlpftl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dyyikkmc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2byqpcbsr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ceiorybt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lanxyuyv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2icjgkety.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2idgaazbw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bnezqvkp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ginpdbnw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2toxgmazm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2lhorzcue.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2godlqrjd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tqtjggue.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sylemczm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2htzwblqt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uxehhche.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2uqcryoyr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2uqubblgz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aukokbji.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kcyypipl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2luzuftot.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qwolczud.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2extcigxv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwgpocvm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wuvolpzk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qdswfcmw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qlszecmr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qbozghuj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kxhnylvi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2fppcmpbk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ejsxrwcu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2klunztto.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xytkjoat.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iqcfhgkr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2umlypsdg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oiuomefk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2yqsfqack.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dwxwwrma.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2umhnbeyw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2iotczfer.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dzxzfybv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dypfaznx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vanijdtr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fijiqvrj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jdpjshyg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2oevijvup.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tmkitxdr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zsmhojvb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2lwpbgrpm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qreqscoj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rljjuxly.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2yvpdcvog.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ogxuejkq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tseryrcr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hozwcelc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yindiufu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2htbhfjqz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zcbrgqlq.html


<!-- 参考信息 -->