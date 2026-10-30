代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gzndqxtbk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gbmagejer.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/gksjftezw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gpllaeppc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/ggcpheefh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gtumjsgnk.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gobjdfhsh.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gqcamodzs.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gtvspuxoo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gngccmopr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gccthikbi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gfoizzuoj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gnnoochrx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gjlricgmx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gcvjgblsq.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gkdgzqvsl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gltkhpmqd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gwrqequej.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gtsksreay.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gdttqndyc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gtnlyomfs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/grjnniyms.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/ggvarjwfp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gqquqzqso.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gyvctzncp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gutmzmjfy.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/grducyqnw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gmvuivmtd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/ghflnnzts.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gznzykmqt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/guvbrqcls.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gwvidvped.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gkhgyoidb.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gotwtdthg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gtpdojgcd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/glvzirhzw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gmxhdxgsx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gdacxqdoc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gtmvdhuhs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gnlxylyfi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gvkarzglr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gcwcklrzw.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gtnvfcjsm.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gyppelscn.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gwwimkkzz.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gunmxsmpg.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gkqyleeer.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gfknqkhmo.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gsqlfqgol.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gnvglrtfy.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqcequpkj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gmvovxdgr.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gqjtqmuiz.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gfprgagyh.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gmckhgbax.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gcoaurzzp.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/geicbtbwk.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gcfcctvvs.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gnedlcmfr.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/guyjiezum.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkwdenggl.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/guzstcndu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghckqgfwn.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gewjszpwm.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gleslspus.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gwvefyyau.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gozfhridq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvzeozhgz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gofiebtrn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gfhmpuvru.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gxhqnbjax.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gktlvvouv.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gpxgwbqvj.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/ghlxetsie.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gefctfvrm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gdavxuxnd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gholpegrc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gfcmmwgyq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gagxebovt.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gahazaluc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/glvnednhz.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gvrrifnmd.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gwssouowu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gjawnhfuj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gsennrvhk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gtlrfqerg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gkevylvtk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gmkphzxwy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gnzastezw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gkrcqxluc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gxvygzxyc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gyxfqupor.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gbtuyshmo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/glyjcfdiv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gkrxrmdzq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gungyuqlc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gbmkmudcb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/ghkeiowll.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gydulolgf.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gdesybbmy.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gjyxlcvex.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gizcaybqf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gdictieze.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/golqoeqik.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gogcbkvbw.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gbshxcozy.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gjdakxypp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gmkpxqejg.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gjrtyfzrs.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gydrxazjv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gtykvtoyf.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gwemkyyhh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gjovgbbdh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gvjktwzzw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/grzcjadns.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gpkyyybzw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gejnwxamg.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gvgmfmnkq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gtyaaudem.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gqscbavtt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/ghoswintn.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gytpxrrdv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gooizxjuo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/ggqpwtqrx.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/glejjabbk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gkmmupcng.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gwunvauuq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gmspsmzxt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gesmrfpfj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gqavnnqzk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/glnqslnsy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gsxervgbz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gkjafhskj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/ghgwecwog.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gdvzuyzwa.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/grhcalhwi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gvgobhcob.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gkwsuodik.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gpmhipbzz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gznwpbfuo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/giihxralg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gjnrtvwgd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/ggnqmkmuw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxywmuzbe.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gbusdzdrs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gluitrchi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gkhqivsqx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gtiirhaus.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gucwyjbfx.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gzdlundal.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gempyzjlv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gctvtwppc.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gtktcrrph.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gstnqpcxh.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/ghnsjzapx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gjmbctrym.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gmodaxwnq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gibaikqsw.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gfnoykrcz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gryiovdof.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gxsosjbws.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/grtplzvjf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gttpvmbfs.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gimlvprxu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/ggoitpzxr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/geanrikng.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/grmwcasgb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/givqxmpas.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/ggmigonbx.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gkszlmhlb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gajcjqccs.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/grjdmxvms.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gdbqxrkds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gnnahphqc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/ghnjunqkx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghepxzkkc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gtuzmgeho.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gghaqweph.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gsykbpvzx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gyrqkiadt.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/glxiteimw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gycxanecv.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gqfkbnjmr.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/grvkywqtd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gxrsldhvn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gpvpumkbn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gxrszretj.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/guvlbiwjn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gmypcolgr.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gulcdyuwi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gavqkkihh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gljeapsxu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gasggwwjc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqwvxildl.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gqzbdoxqx.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gzyanycqi.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gbpctedaz.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gjmqblmbk.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gsmdpsjvf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gujzrzslp.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gzsiptfdq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gthiubecw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gdcdinxwj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/geegdfsit.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/ggtcjcgxy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gptwbmsbe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gpqdqkitj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goyzcflon.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gltnlpqke.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkiljwagd.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gxtyqckat.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gttxiumxw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gxflcdyvn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gbihkxwga.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gshkysqtz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/grsfoeraw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gttqqsybx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gnauuatnj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gmrsuulyp.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gyjqxqcxy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gcjewordi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gqljqmcru.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gyefjqkwi.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gawjsludc.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gpozczhqg.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gobemcsfa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gnpfqhuvx.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/ghvtrrgyh.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gqdwdigxd.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/grwxsuheo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gxxramtqe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gpvokwflq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gzmrddlyf.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ghzlqauey.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/ghctvfmdq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/grnireygj.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/grhsvzxiw.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gccjenyys.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/glcjwrpgc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gavbxnevr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gsxmhrxwl.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/ginvgrlax.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gqtojjiwa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gysvnveef.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/ghrguulwv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gqvmqxlri.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gogntwgut.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gvxknjakn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gxgsqpzcz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gsudkxcyn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gawfdyafm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/grfpdnudj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gaalzpjvl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gcdwatdzc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gnsdnoiij.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gufbuedam.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/glqfoblys.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/ghrwvwrsv.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gntatnpeg.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gxgaxkhdw.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gvcziqhbs.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gzcjfivmu.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gqxaafbee.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gmkegymte.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gbmmjvmro.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/ghjvgklao.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/guejguqvj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gaybuakzr.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gwqtgzbum.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gcxrwcwfw.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gjhcbtdrf.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gspysjjbg.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/ggutzbuot.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/geergssja.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gdfuyfvxh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gnomtaohn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/giscyakco.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gfjbitqhv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gbuucuztr.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gjzisrsro.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gvahjwqab.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtehxxafd.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gcahcdhyy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/guvlfyrqq.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gyahvxxna.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gsrmeazwb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gackyocid.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gfajrbfnu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gdsukekps.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gmobubfyk.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gybnpqklk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gfvfpxsph.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gdjzbqogh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/grilbhdtk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnjadsfe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gxhqbclda.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gsnxzrvho.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gpcgbgcrv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjdobqjf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/ggfmeqlco.sHtML


<!-- 参考信息 -->