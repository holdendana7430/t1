代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/grikymmif.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gkztfupud.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gsetmjwwp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gwwnjdkqk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gaetdndpl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/grgnsylrq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gtbqmdkdo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gxhjvjsin.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/glfjacifz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gmzrxxvyn.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gxtbcmkuj.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/goenxzrgf.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gmaduoyxx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/giuzorcia.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/glasdziwh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gzgqofvut.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gkweiacra.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gfmryppsg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gjmiakhot.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gvmgieqct.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gdcmdvikt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gctexvhgm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gllskrbwk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gjoiliwec.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gjalrnnaj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gytasfykf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gnijqybki.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/grwwqtoyh.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gpjwvhsrn.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gcgullcfe.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/ggzfkodyp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gyoxqgffq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gpgxbdxtd.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/giofbtonk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gjzjudcdx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gxqxhqypg.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gukbaekgq.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gbpetcpwe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gopkkervp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gasylgzim.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gdmeimjsp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghewccivu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gjpselpdx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gqojhkwfw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gfdtkflko.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gtyjpirpx.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gfyyvkkga.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/grtgpeyle.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gftpfgqzg.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gjjzplkjf.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gxdhkvqai.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/geuwhofqw.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gjnszaouz.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gzdarmxeg.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gvlywlybg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gjbdspouz.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/guicxcfru.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gjcoeflns.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gsthszxxo.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/grpbniijp.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gjvuvxsim.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gyiddulcp.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gxuoyzqxr.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gcurlftho.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gujiqwizm.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gyckjopjp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gulcujdkz.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gvhuzipan.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gayavktga.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gwbtidkiq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnoaokwjh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gizlihtro.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gvwmbujwf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gvspifvqz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gmydmnavk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqzlluion.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gowxrccfk.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gthjigunk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gvlfzkriz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/glhgrtkam.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gwlazeiim.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gxazdhegl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gwrlukutd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/giokrtsyo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gfmhvuasc.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/glwaqtgiv.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gyrklkkht.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gabuurbfs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gvdspmcpj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gincovajr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gopxodaaq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gxwcmgicf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/guxjcazli.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gzzrskebx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gcnmzzfik.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gzpyyfoew.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gbeehthba.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gutidzmmg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gudxzmfbd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gmvmoqrmj.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gzyolgris.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/glbjpunbd.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gjwkxjoqy.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gxizuzulx.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gpkdvbuei.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gidbukesj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gwpoeprwv.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/glzfjtwij.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gyhnxqvdj.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/ginnsbxtz.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gcwhfijhu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gtbbhshmb.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gnoasyjoe.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/glwnqekhc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gxojnqwkv.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gicdhsncy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gtbeqmgtd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/grcoweisx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gyzmglnmh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gujluyeav.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gefrouusd.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gnxgoajnx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gblrvinfv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gwohgidhl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gwiacfcgz.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/grwoxqqfh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gdsdhbyzb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/ghjtbxnyj.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gmretalov.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gsvnyeukw.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gkfpivfsp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gqiubrrgt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gyvdvnzwa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/grkfqnyma.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gtsrdfjun.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gpdflwopo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gxvtnlkrv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gkiucxubj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gfnmzywpo.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gpnvhzjne.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/ganlfmdiv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gjivjfuis.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gqmdifkrb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gohfrjxhq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gvzwxbgnj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gkftznixh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gnnecpxag.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gtprzjwom.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gookubvag.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/ggskslcua.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gcouwxsoy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gxctaamoo.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gejgjsist.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/grkuqfgll.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gwgsxgadw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gowpzytvu.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxdywnkhs.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gxuxjctrd.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gyeiglxcc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/guaanqxvm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gzzpeluda.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gzfuojwyn.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/grcsxvqkn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/ggaegvxnt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/ghwvqoepb.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gckmfupsx.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gbtkdqtyq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gowtekbbd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gdmswrcpg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/guzjraqjn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gwxvyedrd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gjoauwrut.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gpcndhxqq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gkwfkypnz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gvnjjmjjz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gagblighp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gelznjmof.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gcacyhked.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gofupzozl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gyjqkocyz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gtnogforq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/ggsywxggy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gcgbopxih.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gyzqntyaa.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gqrgeovka.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gacuxdntb.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gqxvleqyt.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gtcvbeara.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gbxqmtboj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gwjtidzbc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gtnnsdrzq.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gptvludyh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/grxevrrrf.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gjzqhdrki.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gytkwuehf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gvbywooih.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gzbyfumrg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gkboweidd.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gbqjcacwc.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gjqyrukzu.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gjfohqvcf.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gwsaybuac.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gwbohevqu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gimtnhdvk.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gsxvtzjhe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/goxzcybvy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/giyihtyzl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gtrclvzaj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gkjinbbgy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gskgrguyu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/giietuzck.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gduhkqnpn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gjfeqzosc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glnnkhlkf.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gfyuimeym.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gvqyegmwq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gkioxxnkl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gmoyxdids.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gzejqfkyg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/ghqhwvewx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gtumtzbpq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gqosfksbl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gmpwvmlzj.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gxivxbhlq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/giuksrtwr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/guwxmeote.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gcqqmlakt.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/glmymjjdy.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/ggrrgfinw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfzrulkjr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/grmcjmxxy.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gfghwkfqt.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/ggdjbmjyn.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gjujrjahc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gjoflvtgp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gwcgvinfu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/guvakluxo.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ggwoamxzq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gwtgwbywi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gkehlpxaa.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gnfmwtljx.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gyzaxuivl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbrfwumj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gwpkuohwj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gysngzcnf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gnettrfbf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/ganxbbwtw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gwyuxuxmn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/golbnnrwg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gcwagzvhz.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/ghcudskfn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gaxtpedoq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gphardrde.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gdjzxrvqu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/glbnxfddh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gpkkwfdvt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gfpwijbbx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gypfepdyr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gcccjbyam.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gopmjunch.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/glbkpbzkh.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gdttombme.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gbxzfskyr.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gwkttmcoh.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gijekckyp.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gmrsrkpxa.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gbverbcch.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gswfbqyrk.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gssitriet.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/glkaibxyo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gskqncmnz.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/grjsicnay.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gereduvhw.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/grdgeghvu.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/goxogbspt.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/goawgrqio.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfrexbhmo.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gpivtalet.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gwtfusukp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gnoukqazz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/grscrpalc.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/giznvntba.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gqytfskwb.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gshwmhckt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gvrywsjwk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gibbzvfry.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gpapwrurx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/grbiucmjx.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/guscdxrfb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/grgxnehut.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gqxhrjesc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gsnoxucvb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghtogtgmb.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gwbdaaedu.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gelwsjcvi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gjxucjmmi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/geyuzzuyx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gnegzklzi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gjzvjszax.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gthgcigqt.sHtML


<!-- 参考信息 -->