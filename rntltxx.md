代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gnsebjqpm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/glspnkutx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gtxpzpxwh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gqkkzygzr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/guybullew.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gcdprxkir.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gogcvqhzk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/guyzmuhwh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gmsmqplbd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gyigzoamy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/ggapizcgy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gchkvojtu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/grxidtbtc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gqgthvgtc.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gzuvxiiza.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gfuqazwag.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gmckonnxt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/glwiooogx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gqwysbciq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gmjlctzmj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gitsyhkej.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gqxbcelqr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gqisjkxgn.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpqtupbjq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gslutpkwr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gbbsnbefo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gdojqqext.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/ginyocigb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gyyxwdurn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gohndhpow.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gxunvuuwq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/ggqzfdzfb.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gecjtbell.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gwrltwysi.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gkvbjlviv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gdronzxlm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gwxvatwuk.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gvriofwmt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/grbrtwagp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gnywmqxjx.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/glgbwrisv.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gkvehhnko.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/grvbepfsx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gvkqtsvtg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gixiowqdw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gydxyrige.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gnbbwoxwm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gasdnwemp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gkkhwtdqj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/ggjlooxnt.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gfmwgkejb.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gubzlmjmu.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gkbyamxdk.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gdvlltkdl.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gvvfybxbm.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ghhysnsvs.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gmwlgnhfs.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gireuravf.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gglznsnhx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gcfdzmjzd.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gssxjavkd.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/glekniria.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gqtqsyupu.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gmroqvett.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gadhlijty.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gbiwfhydt.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/giqbtqrtc.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gidrisqke.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggdgykfkp.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gcrycflcm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkcdleuvy.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/guguywprc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/giiwdkbem.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gevweixak.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gqkdyebyb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gynkfjfed.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gxodfxjal.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gvmliltqv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzghrteqg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwtmdgnyr.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/ghdfnzqdp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gxdoxixxi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gdqgkmhjd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnlervcas.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gubkfejol.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gykpswwgy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gtgyidluj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gslspfimr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gjejmlhae.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gvmvxpoen.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gabbrgszw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gypkwdejz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gegmmoytr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gnwdfhzyx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gxfjmvskd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/ghjptwmnt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gqrlhkiqk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gvnkayqwc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gvbekpeqt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/glqfjyazw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gzsayplfx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gpyoldppt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gfedunebh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gtuuyqzdw.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gumfestyc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gxdogfysz.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gamirsnvv.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/grrruplwh.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gkcabnjvd.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gkpbybwfl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gjenlwlji.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gxircaedg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gkyqixpei.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gdmanzgvz.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gjnapqcrr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gmpkvvios.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gwakzigde.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gtxjlnepi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gjavmvozc.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gdgmhpmtb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gancxgvav.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/grpnzcrxf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gqaoerhls.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/grdlaqecz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gnktkombn.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gxhqjnnpw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gdmkowdfo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gcjegnovv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gnpozbjpo.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gflyzyxqw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqstcbooo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/goxhvkwpw.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gyhficamy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/ggasxmgat.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/goxvjbfhx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gzmadchng.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gywvahbut.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/glyexxvwi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxqoifss.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gzhprilfv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gszujwhul.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gglxnylnc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gitsrsvaj.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gwvwcnbga.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/guyuttzyn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gkovwlffs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gwyoabszr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gqpdlovty.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gdzfgevsi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gkcrutopu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/ghdvygwoj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gpunfjfgv.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gnqrayjqi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/glhjwkbor.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gtrrxcenj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gppjmyuhe.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gaajcyozi.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gbwncqlzz.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gtotrubqs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gjyapmpwn.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/glsemyywj.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/ghakzwdrk.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gpemqmgqe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/griarkfut.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/ghegfdhqt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/ggljzuklr.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gveohzrgk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gxsrlupfz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/ggmtolukt.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gkyphijpr.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gomihyfki.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gumtsacxw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gnhwifbhm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gbopzsrvq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gyshmszbg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/ggrbjqagi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/glhuijrum.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gwndlvfjq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gsvgvflmi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gjlnarozc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gxfdbnbry.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gignpzndz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gikokqzpi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtgvcfput.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gubersdbd.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gjjvhilgy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gegmspwpk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gtywyxxoe.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gkuwomewo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gxjiptuyd.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/glzlhxakp.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/glkclrnrw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gklqaelxa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gjaddoszl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gngryledr.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gedpfcgvo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gccjedpdp.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gqocchata.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gkgxwnbpp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gdiojaanh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwthvgzba.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gyskutovw.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/grlbvqkeb.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/ggytovsxd.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gyfegmbav.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gxhsafjob.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gezwedbuy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gjtewwxbm.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gvahzkfrt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gmxtnievh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gwihscurs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/giuligapg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gcqtorlnd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gpclpazqs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gmclfjbsb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gygbixjgl.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gzvymbrsk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glfgsxdqb.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gfgsuznpw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gjpqusjdm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gkqzjubrq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/geqqmxgpe.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/glskfiilo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gwbmfyrdo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gzdabauxz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gwsnbofje.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gajfhykjb.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gqhgglpri.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gczscxszy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/ghetaabud.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gtyhwpjtf.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gtpgogegi.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gyownykua.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gnqxkvtzr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gaszyqfdk.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gotuhjpaa.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gyxenflqs.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gdwywitfi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gogylzmii.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gbnofiwhz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gjpkjvqgx.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gimgtxacd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gtakdhzxz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/grgghcmua.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gvsehjbht.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gfkfvwzba.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/ggndeucto.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gshdipekh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gdbvqoxlf.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gemifulza.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/grakcsnom.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gfvzhwxql.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gjxyewgzx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gyrwzxupp.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/ghkrbthof.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gajqjjcfl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gfskovzlj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gquyfhcao.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/grkgoxujc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/ggmdgddjr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gniozqjhk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gwukvmsqi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gqniqracp.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/giiptkvyv.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gyxtsrmhk.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gluaipbeh.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gzwpqbazn.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gclfumesr.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gwaymbbhp.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gubjbomvj.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gpovuhebg.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gjwtwztyu.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gfrwhrvpj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gmdespwlg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gjmjniigt.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/grkmquzhq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gtblugfmn.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ghpffzyir.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gzcqfkaxm.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gcxspfqxp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gulwrznmu.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/ghjrdbwcx.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gvfutehjv.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gklazhxtw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gkmvygaiq.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/ghvakwokg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/grxcbsbth.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gwstjycdx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gxpfiewaf.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gbmysskzx.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gvzceigse.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gjqftzfef.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfkrxsdio.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gpsbeunxz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gqnmfrcyp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/ghbrowebr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gkkefhddo.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gecbcqhjk.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gmszttikm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gewyapqbt.sHtML


<!-- 参考信息 -->