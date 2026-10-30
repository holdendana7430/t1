代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gizbuvljv.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gwwixhowk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gbytttfeo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gffrpuugk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gjgvdnleb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gownsyjrq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gskirfctk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gbhsfrnad.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gtefyvlql.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gnyfokddp.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gzgzqjynh.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/gfnhrmwof.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/ggceoljsj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gmneybdxe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdwtapizv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/guoffeyoc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gbgdxnvpz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gwmlrmdcm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gwsitkgax.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnmfuacwq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gnloegqqw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gbktbennx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqwkalxjc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/goftbrmvb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gvyqizihu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gzfcbmdwv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gxjjpgvst.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gozilovic.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gmgikfxhz.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gdirqhxxv.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gzxrytqup.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggjxrmnqk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gxdaelbac.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gbzhfcbyf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gmnfdxyyk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gvnffbeeh.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gbtrbacpy.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gpfcpsaxi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gpnklhkdn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/giacnrubw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gigblobky.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gulnmuvad.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/grxjwoozs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/grvyvuzmk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gcnhabtgz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gopfeqoyk.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gfadedkiu.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gdkpbpnsl.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gyvluikvb.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gkhmewpnn.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/grpnkudcb.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/grgcjbnyl.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ggatezaju.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gccjyxkka.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gruswmodx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gbwrvtjeh.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gndljnoyq.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gjomobbmr.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gomqbvznc.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/glbztevcv.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gxzsxggji.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gktazsfnj.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gifxrvpct.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gvzrpuepk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gacsdlmpv.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gcndfkxxt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guwtwokaj.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gbejghkla.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gwvrevezr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gzdvtuhen.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqssycsvb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/glibmzale.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gawxwmzoe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gupjwjwrv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gmtxyxwqn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gxklrepbi.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gviwiwvmo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gdwplhhtt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/glwxcmclv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gspgkjvdh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/glulezmru.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gtebpubfe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gntqxvlhe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gzyqbvebz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gmnndgvwm.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gmzjtmblk.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gnyahlgsz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/grjvkndku.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gbawvzafi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcncbacc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gvkyuhtut.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gelwcaxbx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gmoohtrxj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gwpaqbwev.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gzgyvkzbg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gojjqcmwq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gawzfmxim.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/ghkyoywvw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gkasctazs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gwscnsxwg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gbzlwglob.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmyewdpep.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gjhtzojjs.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gbczdxflx.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/goyiiljco.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gorwvgqnf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gidvzutlk.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gbkvgeffy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gknsriswm.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gsntxeaou.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gdlevmpqt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gtlkmloyj.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gpeekzwtp.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gqheaewwr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gsgbkmjog.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gcqlfbsyw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gmztlqwrt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gcwpynwur.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gmxmpcode.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gqubwwwnm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gvohwqvpi.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gohenzwgu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gqfusstdf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/guybazcat.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gynaxjrud.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gheniefgp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gvrpchplv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gbwqrmboq.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gsihbyhkx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/griqqmnvk.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gvqnarqyy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gstkfpidv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gnmzfdvfb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/grxmxggwa.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gqvbnyddg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gzjhthqwy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/ghllwdfir.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gpltivuuy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gyoaawkrt.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gopvmiaap.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbjuqoxbs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/grbycxvgl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gspcdlkcr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gbghnwpta.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/ggilnnxgw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gmwkpmcwb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gpynrwnsk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gpjbxdikm.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gwhdxpgdh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/grezhnpsb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gnkydsvnv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gzditkcwl.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/ghputodid.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gjlcvxhrb.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gwqzqbshw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/ggmcnioeq.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gepzxaxsc.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gregewvhf.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gjunlshru.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gywbvpkwx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/guyivrbfw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gyhgehdwt.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gdgbuutkt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/glqxjbpqs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gcdcjtnuz.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gbsquewlo.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gpyjvtudq.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gtsmegqrx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gluxnlmcq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gdwgaatxa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/grfiiplqw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gxaistjkz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gankidubl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/ghwrxwlcn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gbjlufcbe.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gqprahoro.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/grlkbaiwy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmvnioton.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gemmowwei.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gsmhnpjue.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gawedgpca.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gjjgpymqv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gifogdias.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gfvgnhhop.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/ggplofbqt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gcunearpo.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gbuxowvml.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/grqqgrwej.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gteayeznq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gdgvihucd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gglbeumhx.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gopjdxeyv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gtlugmokv.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpynrriaw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/girkdeyhm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gdnuniqde.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gfwjhkwqb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gikqkpenp.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/glqbhpexe.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gxtloyjhf.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gvveatwwh.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gculxcawe.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gxliuugqt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/grqsahpqf.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gtfogqfqo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gmwtjkora.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/ggfkvonws.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gjriulflq.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gwfhpupmi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/guekcaxmx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gzzojyiqd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geypdonqi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gsldyrpwr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giybzsmro.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gobtrpavl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gzenlruvq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gnwqfzhvy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gmwcrmthc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gsmxdynkj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/glxxrgrsg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/ghekbxkww.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gwvyhxvsz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gpefmazmk.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gebobdkhl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gumrgymcv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gxaicdsfr.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gtgpwxjue.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gztqitckk.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gjakcpyol.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gznlfgqut.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gqhjkfddl.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gmemzsywc.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gzslsswjh.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/ghfayajbr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gjekrwdoe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gnrkokumx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/grjdjisbe.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gafcnmgzw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gnpofwfbi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gojzkqcrs.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqqlkrxbz.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gkdsctlvk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gxtwkuhlh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gdlhkszla.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gvrxqttnc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gzneihyuv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gnjyoluyt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gyxpxfyoe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gnatctlun.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gtiachdtu.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gihfqawkx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gswrxpbpe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/ggunexnaw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/ggoyxhlkr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gramzzate.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gokdgrljn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gigfsbruf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gaywsjeoj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gofhoxchc.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gdtxsrwop.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/goomqaywe.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/glbjbfpcc.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gfupuqvmr.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gczalbzvj.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/ggqutopcs.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gfpctzrqy.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gzcpjjssp.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/grlvvmwsj.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/guvgwixwi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gnskczyve.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/ghdhngqbw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gkahnaoia.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gmtegckyy.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gmhpfgotw.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/geomkfwfw.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gdkpwkemp.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gasdtxgyu.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gxgvrdrol.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/ggrdkstrg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gqynmshfb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gvbojolca.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gclwnkptl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/grrvxwvyr.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gmcqynfqi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gixumpdcy.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gwkaubyrw.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gdfrutbdi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gutgrhuyk.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gmuvsjeks.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gzantxvkk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gjjswnrvb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/geaqyljtn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjrawtggo.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gqfxqcswj.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/guohtuqyr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gecnesvxw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gmlkdqzou.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gngoaclso.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gplpbtoqe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gaozekjra.sHtML


<!-- 参考信息 -->