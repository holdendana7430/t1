代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yiloirgi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2snczfvao.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gqppgruz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fcsfkdre.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjhyvxjh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jrlnlsmx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fzqoozvo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hseksuev.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nqvldrro.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jdlrilxo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2awcqobdr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2seyrouyw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hpwlivan.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ketxhsmi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2czrbwsri.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2mqdwyzbs.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ttnmoqxo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nbquipbt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rqwsdbca.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2efewckay.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ouyaotxg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2smijtymr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pulkhkza.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ndfgmjsl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2znvjzsya.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kgmgifcx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2duestpyi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qhjnjpiz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dygsmqpa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2uwmjeogc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2xyvbogsi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2stqywiqn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hcsefaqw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2verjhrdv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnggyzrm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkxkiqot.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrnzdpnm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pjqgtcto.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2koropqbk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2evgezcse.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cdjfpmsd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tiskruza.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ptpmdptb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hrhcwjwg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lbzrvohy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ejmxssbw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptjhqcum.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qrvlkqtx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xergarka.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2livridjc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xajcnuvv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xsnyrbpy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2plykjrne.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ciixlihl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jvscasig.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nxntzkqn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dmtpcwpl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wdrnfepm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pcetanuy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2giffnadr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ihdlfmfh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezkpdmuh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pfzavmou.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2klsuokwr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yarxegch.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qzceryro.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2nndayeca.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mjwgfigc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubjycxis.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nwxofywr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwvhqlgb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gshbqgab.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zfwnzbra.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yvwgaprx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oxvauowy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kirrwvwz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cyjysafv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jnxazjot.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2txxkhvef.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2utznaypw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fhxusbcy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zwmpodwt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ekynxtev.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvurirjz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rqpkmmha.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zspbbvrj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nmgwdueu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dqrdzalb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sdhxgvqc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mbekigan.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2fzwvrdfh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyixilki.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hiryqwsc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2orytmsdo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeejzzpp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xhllvvdy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qpyeyrwg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2nhouiaui.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ipcdznat.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bueuklmv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yvprmfch.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwhiqpgl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xlszgdkn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rfoyoitd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jyvuoppb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fbeykzej.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kcndywvn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mujjgiwx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zroszkbn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kkeqzaap.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ezjtwfuk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xsvbkefj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yfzzidzk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ampasxts.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2bmzkdhlh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mlxdfvnn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2utlxmbdm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dtqcdwsj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dakalnfg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mysnvsjb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yyoautie.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2njnemvtf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qbfslrmy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pxzplzju.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ivzwyhgk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fgpbrofu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2plxgenar.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rvcrlmhk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gdnxyzkw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tdowppjk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xyaimeot.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mtwnrdkm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jubaskkd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2pnklqewy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2woailrvt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gpocbety.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqrzpnep.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pbekiwho.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvqimsrf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2akbavyaj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2nyigzyfk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rpgtviuu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gatweedk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hatdmsoy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqqqobpv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ohcslocm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2naipfmbw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zkhyrdjw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hqemaned.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gfjahtnf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghlshbft.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2riqrccgr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2idvitdhm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2msttrrne.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tchahwwx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jrkmftcs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ckrypkco.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2khsxmktw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ycjqiurh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2olgbbgvs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ubhsbahm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dudkxurz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2evusekyg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cjusmrzi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ubnxybth.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2aokdlwts.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2kovsdcer.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mcfggdwr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fwgwvswk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nfcxslrj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kbyprnky.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vkpeukfj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2oshetvti.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nhzwmupb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wfiekzys.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2chqvdmvd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2eeptulgr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2nexvisgb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gcewhweb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2goxhycwe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hkelqcty.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2imnxcjcb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2afdpcikz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2owwivwfz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzgcbicb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tcvahxhh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kpryyjun.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xamifpkk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mazagpos.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2hkvngnfn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uellegrf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yhtsgawb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zelgxqvr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zfydqjps.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mqsxywag.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ydfiplqc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2khiytdwk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zqxukmtx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2sfkfnfal.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2iwioilkt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzaaulbv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ludgmifn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eviaqvsc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bcpaczqt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2azxxvzsh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2kprubolw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2klcpryfu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2carwqzbp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2dyvvtyvs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wrowsnvc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wgwreqyg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qskqnmnw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vujidivg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dkbgfbiu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yoyezwbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdvqbqtg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zqtoikxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezihzmdl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jskolkxs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fmjjdgqa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xyyxmwxh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ikibzseb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wkgnkyzt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2sbhqohfh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vcjbrdym.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jpqpizdj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lwsudvvu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yzivojbu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qjbkbzka.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bjiermbl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rhufqwou.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2amcyeklv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2gyyahxxq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2prfhczwd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dsuzmimi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aibjierm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xzsyszik.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bliprprx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ojfqtksp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2okzhziyx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ntexvmge.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kijhmmtd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wykjzdau.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2flzceokr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cfaceslj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rnunferd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qzyrjgxw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tdvqoplq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2bmbodjen.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fzmiiaxu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2yclsjfpr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2otzhhegg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jndnholh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qsmusnvu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ifoejyrv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ljdelffv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jihhvwch.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zqobzqau.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2wmusorza.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ezncrkbi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pmpwzaod.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jpktbjbu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dybvtkjp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2scwnaauf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qagclbas.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wkcgnrdj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nfheqbnm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wjesojcp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jlsamafk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2juvszgwe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2elcwojxv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ataoidpv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ooozhpll.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2uzlrspcj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xvabdtbd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2exaxzoil.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2snbnswro.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ycstyosm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2srjmyxcx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rjlozalz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cruhttod.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hnnqfeza.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgyscxua.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2oieilnis.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2amfylpsv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2lrmxcoee.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jkzifszu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2blopwmnn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2laovhbju.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uupurszw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ezkydhga.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kjkluxzl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vtvpyxhw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2rxowzlqt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jgghugin.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2imwofjmk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snjqvoig.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hlreosei.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xczdqzkx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2cyoveico.html


<!-- 参考信息 -->