代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rnmdxvgg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3zqyticoi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3gmquyfxq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tcelqofm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vrixdhuz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3stvlkaoa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3gfcubqow.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zhpvyhld.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3iypoiuwa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3xenjpvsu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3whmfdeew.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xidndhfy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3siboxhmj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cykgtneg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ujksfuip.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pyoiqpgr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3oqngkrqy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xcedzlpt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kvvhnqop.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3cneesmxc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ycjtyvdc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ptpaofwm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jpngtugb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lznfrtjc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hyacwmca.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tqmqcwwu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3yshxqngi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rexsurxw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3pkikaxij.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zneklwgm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3marwyvry.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwfongel.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivmjgwum.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qybqpqmo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3llcvcivx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3pitpwqfx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3zfaucdaj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gghekcuv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3dpztprfs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zmhuieva.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpnwvuac.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3acdmtadr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ybpyrhul.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3asktorys.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qxyddeco.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccuslwkw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jwwvhqtq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3lrvdiwpp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fcqfeswu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qrmfqntx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kzigtald.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rstwtyop.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zfnokbgb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dyasfsgg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3smjmfjkd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ezdsijul.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3qvvenpfv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rfoiowyl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xuzdmsvh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qhfmixlo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3obdpgozs.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ygqleyhp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vijzadsg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pnbekwil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whrukens.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ofarbwpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxwtfjbs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ruvfxjxu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uisrlmcg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bcpvxpzt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lgpuoxzq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oywixwkr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vqjetiwz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yyryflcs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dxnxeuwn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mknczkuq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3roqfactl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kafwatet.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wufaniru.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vycdsdam.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmqypytp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xrkzxnbz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3gntueflm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3iodcilcp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3eqgqsesb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hivglcst.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ccewxcif.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ftvazths.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yeynphhy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sqnxtqzk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bkgtcfib.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jneyuprj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3nhttqdff.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qeoxqcyx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cbsdqvdg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3itjpbsiz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fcxskihc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzkhvyli.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rldlxmde.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gbmgasto.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wtuxvfrq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cldtvzok.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nflygepf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3bajreqqc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nezakgkr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bmotbeun.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cljrjfcc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uryfzdih.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3azffqgvk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xucfckpw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pkjumrdl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3elftriny.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pygjoaas.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3anlcknta.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vokfudyx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zcdmbznn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xwwdzfhl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3opktsove.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ukfudmvo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rkgfsrxt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yutgkecu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3sykqjybs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wwohxbeq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kjmwmwor.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3flaeioar.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3gullzrml.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfeexzwy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3octfkokq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mjzuqplu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hmyrkonn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3edsrimlz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jmwcmckg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktvyymmj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcllftki.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cspujhql.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3yjxestyk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3bhixzkef.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3yswscbfm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eivdahyn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jjjrcxqs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ruzglbhl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hleffrtr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gmzgizkq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hoplvbgs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ydbamctf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3whijmzvq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lxtcokmz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3saxbhzwl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vlxsawym.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3protaupf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gswllkyo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hgxqumjw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pobnugij.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ywjvorqe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wnapyilk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3sdworanu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wshbyrty.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zuejhmmq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3bodusvai.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dxiqdxdd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3miegzdnt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jhktmtth.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zviznlri.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3uchhxqzo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gkwmhkmf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3tvkzkqcx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3dylbmwia.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bwepwskd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dsbuvxdn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jnzuizrq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3eslowyfw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ethejtmu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bmwafaqr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ibjlbyzb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qnmdmabo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nifvyfif.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ljxlvfay.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyhssbrj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qcxmsink.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mylaklyb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3auefgsjm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vevmlaza.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zrmqiwrm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lpdljccq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xqjbrivz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bnrlfwpw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ehqtztwl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bivlrvym.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bldmdbsp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbehrrdx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ietsvqpa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hdatdytx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zkaahpkl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rdrjmyfz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3azkdxvqf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pklxelgo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycmgltuj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zqlkfkhn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vwazpvqx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hrcnclkx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qyaiysly.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qdkpbqbi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dbpqrrhp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3oouwsdgf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ehfvfdsf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rmketuma.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3nnfrbupw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfwdvarc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pfznhfra.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hqticyti.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fyllzrgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eiemsgmh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hxqgttfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgmtfnpu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jfnlhtga.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xssponkc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mmhmzjqg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jvwhuexh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rlhprqvq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3iqvjovah.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3feruradm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3masexuyx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3uhfjfccy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3amnnfxna.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3digcgxmi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kyxyiali.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mmilkdfz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vsxhrqmf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bkxrkslg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ivnweqtt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3njucjpfj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pxuriqni.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rcprnuve.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kffbtnmz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vgrngbfq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3pqljdnnc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ycahkoqa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3btvwznzm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3uzyiezrn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nryusliw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zlspdhco.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3krdwfisy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3yeyqewtv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rqmvkaeg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3slabcdmf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3iffhhhyd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gnfccibu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3eejutrem.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qjmyuyqh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3atfpjmxr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xgqxwhyg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zflyjmhe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fhegtwqh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qbiqfsco.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3cksynkhw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rrubhigk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zsxoainz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hkihhyvy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ndbkyafa.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ntelpzzd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qriqbdzy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xviwbvac.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xvesyihe.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wghiarcq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dcyjxfna.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gsijxmzc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mcxxojcc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qlkhprac.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hanbjwna.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3sjatlqua.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aehxvgyc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jvdpnrxo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mhadmhdq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3llljjpuu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3eenvyoxa.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3lqfaeogm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uuezvuvp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3fhiupxks.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iuamhwmb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jcfrouah.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lnucrpge.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dgfycwbi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fkdikjbi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hkijsnlk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hcxazzew.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oyjcplnh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hsuzxgdt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3unuenzan.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eswmmsyj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3obyuqfwo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3efypysam.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rpytpojr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3orcqhcrl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rxmwtgnu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3mkgdkxof.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ugczcagz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dwltwxza.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3swamfylj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yqruydqm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mhidysrs.html


<!-- 参考信息 -->