代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iyelzrbn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3nqkohkon.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ckflfwce.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppdzzcrr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sgovoueu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fqjbojmg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3myylzvcs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpaifogg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hhgtouvd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lviifhoj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3gvzknsdm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3tothkkec.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3btvszhqu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eaothumi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lbmhpjzv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wuuclmtq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3frutchlg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wfgayzxa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuutlfs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vvrgideu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3urnbmjzu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3toityrtj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cvdguhtm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cogfsofz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kbdxlwlr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mfbimefl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3dcbcxnlt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wkhnuebo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jyykomsx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kzbnoiqw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rlbzlwvi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3efewvfwx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bdrxxpdj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kftselur.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dclsyblb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tsedxztv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wwmyfvvm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pgsseske.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ysotzpyd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmjlnib.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3okjawudx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngxbcjtx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3djmlaxkp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hcitemzl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdwgrdcu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxqdbvip.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3tskqgxty.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lnsonrwe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ucexacls.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fygcqgpw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hxswdmav.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uwmyieue.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oatcrjmc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iuxfrblm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qrtlhiub.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3dsjkccbi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tvvfbmxu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gohyygbu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wlfsxqqy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nytljpze.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jtmekszc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3raddbqso.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3lfarfpcm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ayztmrgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idyvwjqa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3dvtpychp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3envhsulz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbeokqkd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hoiwavox.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owwrgcrk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyftbfsv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wivjhyjg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3szmcjqab.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ttenfzka.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3byniufnp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fktbcjgs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3pfldhqyz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cclxggsm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbwmwewu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbzgmfpw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lnumyzji.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dnlghijs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3sumcuzcj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tgabhimc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vlepsdbm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3pqlotnfg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mbtbjqcm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3juzpeqyt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpmxwmwk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcpyuxxw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lmhnyxyv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxbtlkz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xzdhhztf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qqaqlnmq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jlbcxpaq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ghvpegjx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3riytraxv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3alinkvpl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3hgrukngb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rxytcdet.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xzuzjdoo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zsizgjra.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hpkeiket.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vxberdac.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wudyvoje.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3vobwuetf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bcdfcqgc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hvbnzyky.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wjxkizgv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ffeqfpav.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mhjqidki.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3qcixjzxy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wynchfdo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3lpqznkjs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yovvzohr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pngzaalg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mcmxzfhg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3esxdkihw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mybilgvg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hrmtxiwq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rksyzsvc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ubrxzotf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ucoqzsrh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zlkohjcs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jzlbxfuh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hmcjdizs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qurigwwz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xpgqluyp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kqtulgzl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jrvjafwy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jjoudxem.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3vtdncmhp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3enrnxrfy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cdbpjyvq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ztkluaaq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3uogeolsh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rejauikw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lpqobwcq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtqswati.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jomqvzkc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytxtmmjk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ftilmkxu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cxvmatub.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ckeyoxqg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfayoktl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3pzrhzncs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3psicamsl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dfyukkxw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xjfakssl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ehijiybe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3owdoabxf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3argnhjxx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fvecedsp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ossmektd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kwdbpbie.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3molacoxj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fzeafxwm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fhxqvvuh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mnhyieox.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3tizsrkwy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yovzoftb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jfvjnjsm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ginxnhii.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wfhypoqq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3aqxoxgmj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3iawhfsat.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3dvllugql.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ctncnwnk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3idderedo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kmlhpvpb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zauwachn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wdbcctkn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ididccef.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3burexcdn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zncdqedq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ztdsanoz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wboysmmq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xvfkexvi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3plplyprt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tenaoloc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxzogwsc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3qrbovrqe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3hzagdmaj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3pmdeldcb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ruelamff.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3obzwsbbt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cjpktsdi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mtpgyhze.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3cxcprdlo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxgrvpcu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bqyfqqfg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3belpysus.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jhqfwnwu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3sjoaseul.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3keesnwei.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dpbxiicj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mjedfvug.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3jqzbgnhn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3klqqnfzn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3epykxwzk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ynburaqo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wmrrjfpu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vfkirjqp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vsniqbfs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3tbyjixbs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wyafrmqy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3pcksmboh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hkojctvv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jzqyfanm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ydashmop.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhbcihhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhepizea.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uuzmeoxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tibdakog.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nzrjegxa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3uyhilzns.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sekigfxa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ctxzdtju.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kvkjaugj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3repgmlwo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3obldwmvo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kocxdetr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fwcbtlpf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3fpidokoz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3tibevcbo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3frpzupyp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bfixedga.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lzhjhhuw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3yhiuydhb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmrntos.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qllrynhv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mdrukixj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ugntbmgk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xzcaknrw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndxwjkpx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gpcxqche.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3clvpfdff.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hordiegp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tennqzka.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hadvljvs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hvgssbxd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mkiqquvn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qioqjgef.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nihsbjbb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3etzcnsur.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3pdpouihy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pbodvols.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3teptmkwv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3oukeihls.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yufvcwia.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yzhvuyxg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mdryqoze.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3clrnkavs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wjtdqkql.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mkgrxgfc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tdhapkvk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kfzqsuvj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mvfnbfrq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ddvpmmnp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qjcqvwcw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nwedxeio.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3krrhwpgo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jujfpjrn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hrgposst.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3pdmrrviq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lycriopy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ttlarygu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dzeqvarl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mpzkoqew.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3iodwaugs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wlvfhmol.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3otpzujgi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3crrbfsgp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hfrpjvja.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3megarevn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uqchbpnv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3drxcgqdb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qnrrekyf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3skpjmcsv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lhvsuewc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ranzsctk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ijofbtjd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3guingnms.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3evzobzcb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3oakivkmd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fjcbycfy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fuyqwnsi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hjdjjpxb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wfrvmogj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yaetbvmo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kbbgssyi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3bisrifpf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vnuhqtil.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3inehnggp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lxmmvtzd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gjdstomt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3dbmuadms.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3edsnflkv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rwqeyrcx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vhfmfjfa.html


<!-- 参考信息 -->