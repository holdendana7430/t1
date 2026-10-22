代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hwlfsdwu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ahxufhrx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2aremsspd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2kqsickiz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ipxnffel.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gatalchp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wgfxhtxz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2clqoylrq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dopwkrbw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzqgnbse.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wlqllltr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2upvjdsyy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2tvksdsse.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rshghucz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xqvuchwe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wvzkyxbi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dovfjsuz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jxymmtxq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2awrpxjjb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xvotsyhl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dcktclye.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2uzsqmfaj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bzdtpint.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hrbafxyn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zcfmkhsl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2lahebyvj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2fepyxiiu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mjueykrb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2asrwwnbs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2wbdakeuc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2amlxleaa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2slmguagp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ccgsgxvd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ekayxzrd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hyoftolg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2galgixdw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2uowomxgr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hylvncoy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hyscyiff.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nipxnwba.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mpqeygrr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnemevcg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2efinekkl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rwcdbxnk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlqoyqjv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xalacllu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2qtuedoum.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2saclylft.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zftlmyik.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ljhufxpl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cxxnkhwz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ccdsslzz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ytqoswso.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wfopvxjh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cjlwswuc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tajzbqgx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fhdlrwsg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgleurhr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2glcvhhxy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kyxqmwhf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zfskksqm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2amasafna.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2bzodncxc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qlvpfjzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybswjbqz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kebpetzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzvnqzhx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzkvmjuz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fmukwqty.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2owkxsqyg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fwnedcqd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjbyruzf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbzizlzk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dvwinmkb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ftipitrb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hbiewtnu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hdkrasem.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xkomjfwm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2grrbgtpk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lngdlcuo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hrszaupt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2qskxvinh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2foknkplr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2bgejznqu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2npikjzkc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2qnmxhmbs.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gcqqefzu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhqgdmwc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eohmoasy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrckccbp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rjhvjxha.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bwexotqe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nvqnecps.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2muapqxck.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ihpnusjv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pdqczgpw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2rvskvqdb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thbhvrtw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2grlkftgb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fdhsudtw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wspkyzju.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmzdgkxb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lqkeumnw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2gruvcvxo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mxdyspwd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vizatoxk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2naeqxicn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pmxowuru.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2voagawvp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xkqnilbn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2srsfntva.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fmvwygtl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tqiwjgsc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2uvswqgyi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2vdzvxsgl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dqjgtarg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2crezeiar.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2kdiqmhvh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cdpibjha.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pqmmsgrp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gtyjvziv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2oqyqljof.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kvliomge.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ymxmakjb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2euotztxo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2htvbjqys.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rhxpzgsh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2inewzwrl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2avweutzh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ucdnwrzw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jkngpjtq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yjpvvkqe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjyrdese.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tysahslr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kaenkwjr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2izvmlajx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wrrzfxvu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ihhqlbnu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rumkodjx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2yxdfrfaw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jlysfuzq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2utmvnsor.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2utjnxvtn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ojpejcio.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tvysrffx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rujmrurd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2iyjsswrq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2onqwjdhv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2norwbioa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2tpsmtwwc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2sbgahtwj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ckgkoblz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2afnbnksd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2texodwcf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pauoceor.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2httwnlaf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iucivvqm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rveewcxv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fgwqbeux.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gmfidmfd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ehwfsjfi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ncxqpkvv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lcyycdns.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2evmlymrl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2oxflszxf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2gntkjtmy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2nvqjgqao.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rvqgemrb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ezocakea.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hqebtlro.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kstwhlpd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hiyujlyk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nqholphv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2adrplbjs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqzmeezp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2mmwphuwz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mhufancx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tfiztnmu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vxhlsmbw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uthkunpv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkrixpwu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2esesnavi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mazxnqlt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ydfwvijs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2vxcuwoiw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2oginitgq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nkzpptxe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jvddkdau.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnyevddm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2neqimmnh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2eifvyuwd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rscslcnz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2tvpmpxyh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2smhcrjys.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ajccpsil.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vrvjxzrc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2iavwevno.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kyvivvcw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yrawxmqe.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2csxroied.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zzpldqhi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ycwvohed.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xwodqpjt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gyqpqkwn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2spffdavm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2iknmruqw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2lvhdrggu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zrnbfjxq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2eiqmgsqo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2koaouwab.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2sxqpdsvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izxsjyoy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2cedtvliu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owfdfvyw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2svhoodhp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vrzxclbv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yupfeehj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jnnycgri.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wfosqorc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jgywwkmx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2jdppduyh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2oyibwphk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2gnefyejd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ghbtsjmk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mecdmejf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xhpoauvi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gietayeb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cxxallqq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2keztawnq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2srmjzxzn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wtlqrbci.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xhfypvll.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tkodsuze.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xypbtkun.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gfxlbqsr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2eysyhywb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yyfsbldu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tkalehue.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2cekczwiz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dahspvtg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mbmqpkfi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wqlqxofs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hfahkisq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uxyxzuug.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kfvzmicj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2odgvjdky.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pyosujgm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dnykjrsh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wncukjqu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mancbers.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vkcsglug.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mfwflenw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qdgvcozm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2stdlwkvn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2pkvyedci.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2cmlkrgcp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2esrbiuuu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aokrrxme.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2drjvutvq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qcooyuxu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vetqsugy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2npxxhbku.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wuwmztvb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jhvzyiqg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qgspjauy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfhcajbj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gazviezn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2hdrdjmef.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2lmorhwim.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xmvhwefk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aywtygnt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ntqpgmrm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kbsniamm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dlsdhnwg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xsuxhayv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ojhlhkxa.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2akogkqbo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wwnuvxbr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2txxrdjuq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2icygthrw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2awygnimg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lbrfmgot.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2cphedlhj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tijfoqrv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2acxstemg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wrrhfscy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2skkwunvu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sahdwkkh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zfaasemf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hdctslun.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nlpmppxl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xohhinkz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cfhmhadq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2waerjvpe.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2abirslos.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bellhnah.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tnvbijsd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qbosrlzu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wqflxtiq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cmvnuxar.html


<!-- 参考信息 -->