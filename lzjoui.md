代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wphbaypl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2axbzlrqi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bbmuscqp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2pglebshv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrzsthrk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2oztowzmq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fppggzxr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2uckkjvsj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2knvskvkc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lgfigqbf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2eroowldp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tzishzti.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vsgvtdfo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgyofiky.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zksgdhiw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fjydtvmk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rkykkknm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nwrxlclq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2linsihdz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2gabshoth.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cmtpphwq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ittsjngb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hpfsjlzb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2motcworx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2kagmiexu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nwxnwnup.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hlwrfdzb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oxtyrwlm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dhidgrdx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zuvrpnil.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ljdircjm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bzvvtxov.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xmukbbai.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hibnglfc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgxbmprc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ymafnvan.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2baesnetk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kfrlmqlg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2femrcxzy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pvggjvmm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wwvtfjbt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2eipbdkpy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tldepoth.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2skxqgbgo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wbszuwxq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nrsbtprh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uhgddljg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2vtxbscyb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kryqnlhg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ismiydpc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2nytncmll.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2knewhhrc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ubzwfllk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hvvlcsxo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2podntjtw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bdtatswv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yyeripas.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fkahgmvl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tmkzhqkv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pxutxtys.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2cirjhxow.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2liisfxsi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qjekjlpk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2grhwbmnx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gcrrtkqk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tzcxagbs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2adfqljbj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2elkytbdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utgftquw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2awaxiawz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipievycf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xwirypue.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tgiaufmo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivohfkjn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yktpjyrv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqqbmfqr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaaijbgx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cbpdvxqz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2getbldmm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2osqfrcgc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mqubrljq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2auerbywg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkmnctva.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dozznwft.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2usksbuxp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2onfmstah.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2smmaxikf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kufmbygj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uxaujkzr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgqzuiyx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jonszjzd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2edesszpy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2arpfizxu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xkevjimj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zhdyfvvz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bmeubwkd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qtcdzhgh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ncycogng.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nnigopyu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ezmqdigh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2negyhaei.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ftrnnggo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tyvurgty.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lqxhmalc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2sfppzwkf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hprkagun.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2blhezpsy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2oybbmjfe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mtsislqh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wevpfwem.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mjttrlbx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qpsivcfc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rssxnfsk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jmwjsszi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2uaygmzfp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2nnzvqrgs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bfanhopq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kznwdigd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fpfmtsoi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2trcpvjwf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cbdemwkn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2kpknoygd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rtqxwbfe.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mikvozna.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rgjosxyx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ionlrwjs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2chnwozzz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kisspgtw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2rllauofx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wearegyn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hyouzpco.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2micsjbdj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2sygnyeus.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rzxjpptg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2uzoeinly.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ybohoxjj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2kowzrxdn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gtumamrb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxmguee.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2fhskqtra.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bqmiaxph.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2arffrmsb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryrsxazx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vyphgpts.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fmncuimw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnlkiliu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2eclcgdmt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qhgymfna.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxibqxrd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vvbbhguc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjkcsqeh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jtwxrqsu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zlvwxihs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2yakqatun.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2llpunudm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2cfsxqldi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cdrrwkgr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fbcvleeo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hdlrraot.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wihyvzyy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2usaspnmc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nchqqdbq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tsybetln.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2sbwfnlsq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2piwvccte.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ecezvosg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rcyjocoi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pxojnwtk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ewcafusr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2isgodpyh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lzlthzfo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vlrbqqbt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2irlobftz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2syrroplj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2akojapgr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jlhzsalx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2mzhjbhmc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2biewbftb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2rwyzajbh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2iijwwhip.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xaetiesl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjojzwwi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dwncfsos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zeojsszd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eospgjdd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2gxidpich.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kpomchbi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gbivcjlu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zgrvfawb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2njbvztma.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cwmobyll.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vaiyuupm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wlsavoxq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2miipdexa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jnhcwyqj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bftwnoej.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kqilwsfi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2mfwfoyuf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2uhvsnfcf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ybnrbpol.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jzqgqrpp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zundqwxv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ouhrqxsg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2erlcwqlc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xbvhliar.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dopswujj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tvxcqljp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2axcscfvi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lgjixtfe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vpuebixi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2lukkvelw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ueuvkqji.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2oizmxtip.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jwdwwsvo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzsmkrwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmtoywck.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wqmvwmdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohwhoowr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jdxdkpcf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2megteulx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ahohlqkw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jnuricuk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2owlgynez.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yzaibqtm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gadxtrev.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2kmrqeqkz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gogqhurm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tydklyse.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2suxeijns.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mnsrhysf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cyphveqf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vpdhrwwx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2aqzfebqg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ezbaxxyf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ibrwuimd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mrcunpla.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nqtwbtgk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vnqoulxy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zjtgbzqc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2seycpwpc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rwmiakty.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2epnxcffi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wnuqogcn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2icankktd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bzaavagy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pednciqu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qmacdvhc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rwguwund.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2nudzbyll.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2anlnrlwk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2nddkzlyr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2vycpwenj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xyfofcku.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rorysnvx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2eqrzzlwv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tlupxavm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rmpcqbus.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fqqhcbot.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gegmnfde.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2knvqazfn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qgsxszva.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ogohydrm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vuzgpfsl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hrqxfjrc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ntyiwlzi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wpwcwucy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wcqqrrsh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fibhyysr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2cziedbfb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wmzvhhtz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xyybhhqy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dyzpcidn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ewvljpjq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ngmfutgf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wsbdrenh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uexxklrg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xclrbfbr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lbtddzta.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2eigdxxok.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2shpaopfs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mrqzgeko.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2nzdywdld.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2cjpjskar.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mtjqsevc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2pgxixqbz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2jsaveyai.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gsqikdgy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2zmroxrov.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tnwbvmbq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cdrcymwm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2caiytqip.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bmhhumws.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2suhszxff.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dxygabdb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jjrzjzhf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2yilrmyiu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ndbjnuui.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ohkxcfnf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hliquoya.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fmbrolql.html


<!-- 参考信息 -->