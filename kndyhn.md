代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ntztawuw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xsktyvdj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrpyzttj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2mgwgqrvz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sohmbyyf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xlybabnr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bijkumtz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dleqgkmn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ofumsvle.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wxxhwvxk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rioyqplq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fgqmhgwq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fovjzbqw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbthpqls.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hkilzebg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gklyngug.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2itqumgxe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xcdvbbxu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pbooysxk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lugguvap.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xhwhpags.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wykufvbr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2dpsdpkbj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2urywsxjy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dejvpvzu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2saeuhxzk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lttmeqxk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jddufcse.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cuprceii.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2evynitoz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2axdkiopl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ixxnexzm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ggthniai.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2uarnikra.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2bwmkmfvq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xalrdlsk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2obyzgujd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2txqjfvfl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wkquenkj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2kbwxdaoz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ycrjeiea.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xyrnbmrf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nsewnanb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xxypobvs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrjhicx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jgzcefjh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nckbvraw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yrcendqj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jknzuvwa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oktardoy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2tzutkbck.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fdydduvh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2htxyavgy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dvtuogzy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2axxncrzd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uewkgcvt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ehqojyoc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ytyitpao.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2umefcfmr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rrwvamta.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wxvjgnds.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ydkltkow.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hgxumdpv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2auxfgxrr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nzngvvtc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nyjiqhil.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dqyfrnrc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dfhibsll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qafymoms.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pwwvqkad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkmphtuy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pproqstf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lycubtmh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2omujucew.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gblcczlx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wntskflp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mujodxmv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ukkmdxeu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qlrstbkb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2snypsbhh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hvjvuljz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ymdtvaba.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mwyuvglr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rudvidyb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kjwbtrti.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hludzvch.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rzihywnr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2svjbjrrz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wjsqrhgs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2skxtlwzb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2slyrnkvk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dtucjvgd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2npobbnis.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptjwhocj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2umktlsuq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ffcmmgys.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2usfqsfhc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2yjawhccd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jfvkehzv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cldvdpza.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2yxigpvlg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ludkxqqp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mlcpwxqb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2thozawkf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2juhqmcyn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2krmaeixb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aumuejar.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lkzpzrgn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ifssgggt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2nwmzmyyy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yhqijrvh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yrbetuwg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2moswhlpe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ypigypvd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qbnrhhmj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tqnkcvba.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xruodsuv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qnkeqhic.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2agikcjep.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2szftkkxi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2orlptzhl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rjdkmrfo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hbgxadff.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xgxzffrv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wbfhoaqg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pdwmafyo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ewfenjso.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qmmykabn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2wjamtzoh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2oydtdjsb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ytqeqfrm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2txrtqmym.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2veqmjrwi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jodbqsdp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pltlhmeh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rwdqibnq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uymzgksz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rwbzjiws.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2awgifnux.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hwykhejz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xhiiwikw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbjphtib.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2awedihny.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2mqvozjxe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rtshzvpq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2swrgkptp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rmyxjikb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nozezhlp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2psasbksf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2tqhdgrdz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2swecyvan.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2bpesumay.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mweslihz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vbilcrhq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ehlpjdao.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ejwjfrze.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mpfuldum.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jahdmlrv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2emalavul.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qpkwwgks.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rmkedktv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xqekpzgj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vmsoolqt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gtimwjyb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ytimoepa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xkwngplg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zobhnfxc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bisgecpr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2crvozhet.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2suygeywf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2sxilswiz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fysgnlum.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mzkqksqt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nsxcrpen.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jrhkcris.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mjgkyamn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lfvszbyg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dbejoswc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2diongrmr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2pbwateeq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2evmqrllk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuusgaid.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lqlemhzw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ydhdjtif.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrgwwskj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2zqyipymv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zsoxytct.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zkvngpei.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2vztfuyok.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vipnjecz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iyuynlbr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zpfasaza.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hncpruuj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zjczwrhw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zwotyrby.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fnscmrbk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dvzvwsss.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2otlrvdpy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2inhxamtb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ikhmafdj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2khjmyoiu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dszrcime.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kyxcrkay.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ssnshecl.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ajspamsr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ounufvoc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zfvdsxek.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2svhlsouv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bxczsunm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2eqgkbnxq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zdcvjkpy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvqqbhqm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ivgcawdc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kmrklsym.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyijbrrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avpvltjf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2eupbowyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmjiqjnr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ngasdict.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ukdvaksz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pobwsntz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2sjzuwsqo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hqztlltz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gafkrhwt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ecuaifba.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vuhryfpf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2oznixxag.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ocxlbhcv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rjzfekzr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2opuslkbt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fcuzhcqb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vvhwedcs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hsppyjmy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2eiumgxik.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qmemncjs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ywkktjvl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2estvvspm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rfjnmyuf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lpesbzim.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vmswbkfo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fmfjojgy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tkghkgea.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vpehiyta.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2czsmhmnz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2epyprlxj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2iyqisjih.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2wqilgche.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lvmgjpod.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2brsstzjh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2achvtcif.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hovdipxh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zavlozty.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fqdmfpdc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jywejugu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wwsimluv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qxakzgmo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ihdxxvyb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nwzohniv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ubampwpi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ffytntmm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qtstmyyp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2miwblvak.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hgbxmbro.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2htnzwbli.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2egdlsbab.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mpzteifp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2aecagtcv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gzdyqvby.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vkflrjgb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fxnxwrqk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2emdkqphd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vnbbgqan.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bqeolpah.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hrflfgnj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cwnqyhzn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yzxrzcuq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gexkrfwi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yhvlxvhj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wmmnaggx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hstycjzp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2badymrwk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ldgfglcm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pfqxonmv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fgfcfiir.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zrlirjtl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qzekasgj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gjqrioex.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fssfuenb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mymhevtj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2drweqhud.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ipgudkfg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kmveetor.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ggcxpoqp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wldmlgyt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2mapqokab.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2bhytkdjv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jcqbafja.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uiugifts.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2wcfxdsev.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vcwrrmth.html


<!-- 参考信息 -->