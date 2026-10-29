代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gbcmtcexx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gagnggjzb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gttwktmfm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gttkhhlco.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gufqbskbp.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gjticoyuy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gxefcbdde.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gccuoavhf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gqzandrvw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gjhvlcmmq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gpsuogyyl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/grtrazspt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gelivvcni.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gksrrdfen.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gchmvabpl.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gkzndzyzd.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gbfilqnww.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gusgdzkeq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gqwmcldie.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/grxwoizqj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gmsmjuoth.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gtfkaxgtz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gzuxldgam.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/goawxckix.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gxcqjasjx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gbczkezms.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gcsvtmztw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gxnuuykuw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gexqvwlsc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gcjrftsoi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gaikvdicv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gafkjvzut.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gwjxeitah.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/grpaocqdl.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/glhmwbpaq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gcwfvuyjq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/glkessizv.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gnedpehgm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gcpumdtju.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gfdkavsjw.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gkigagosx.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gqkamxstt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gcsrfunsz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gylnsvrdp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gauzveicj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/ggnrcjhyy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/govcigdgo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gezftznra.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gxdgamalx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/ggqfopsxq.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gyapacfvk.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gbuvexkew.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gnbvfsuod.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/giigwfzen.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/guogbjcvh.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gzcyfpagv.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjvrbaptt.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gijqmfnge.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gvqbihttv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gvpzqwtvs.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gavoazjlo.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/ganmhbxzg.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gsfzrbspn.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gzfilixvm.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/ggkhgsaze.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gkvvaflrw.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gnimwaywh.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/golagpfkm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gltoxlrcx.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/ghnmbqodp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtdxsgqda.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gmslmrjwa.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gqpxlczqs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gnfacrsis.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gtydaianw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gqpuncilh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gsfuvlgcz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/grlaeydwy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gijqhrgpk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gjimshmsc.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gokbwmtnq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gwqpwtosa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/giywtmfig.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gzpctfugr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gwsivforf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gygnjcsex.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gfkfqnagb.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gbmwbxyjk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gyxpldwjr.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gqmhhttre.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gcpdescmq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/giyeggdgz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gukfczhxm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gwaxrcolq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gdmssaacj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/goynqlqbd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/guwrjksfm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/ggyjkqpjj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/groutoson.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gnhsaearr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gbqqkbvwe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gpktrkofj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/glpxnokzd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gwjsodegy.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gpmqieyel.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gesfsnrlq.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gsskpwfmo.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gxzlrpzie.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gxkzleyeb.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gpbvinuyi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gkkosrait.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gjbqhnehi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gxctkseqn.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gacuxjlig.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gxycshyjq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gfswgzrfx.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/ggdvvnezp.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gjecqowws.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gxhoqowrq.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gheifvsnj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gskutbblp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gcvivdksl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/guiqcldli.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gcobxipdg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gpansxdgw.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gpdxlxjmr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gnnnsdoqy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/ghtpahtry.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/ggxhosoad.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gfxbhntep.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gumxgscjz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gximcxqpv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gicacdtyf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gulwpdplu.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gpbzdgvxx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gfuohklnv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gxsrtjjbp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/guylscipr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gtsdtpffx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gnufntofi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/grlompfth.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/ggxfftdhs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gbaqzeguw.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gclhzrpvj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gypjqknlk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gfmhtjdnv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gcjlvuiln.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gokxwesau.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gouzbbpmk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gpqllztzc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gpbyipliz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/ggumxunyn.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gihnbfzsk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gedatzpak.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/guogrmmlp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gvuqdllvy.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/ggeofggkk.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gegmfapov.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gdivjndas.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gbfqqimfr.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gvgkwawfz.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gfcqylhef.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gyliobiqk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gbxdavzez.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gcdlzzilv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gsbdjcksc.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gyvwopbft.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gdxvdodbl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gpvbcuitl.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gfyadxztp.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gqcbtwfpu.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gfguxdrzr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gwluqnley.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gkxnyollq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gggmhxrrc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gtyjwdcuy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gqpcpevqw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gxpwfwilo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gdlrokasd.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gdjjmnafv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gkkikeyqp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gmintubuj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/guxnswlql.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glzbpzjfr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnnuallou.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gwytokkux.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gbbjmhymo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gppedrulr.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gftlqrzfx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gmtesorao.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gsifbkpel.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gttolkfhc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gcscdhifl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gjinocwaf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gebjsdgxn.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/grnayukdw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gnvxpyfwn.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gsywilsgg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gshaboejx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gvxwqlgjc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/graqlitnm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gpzndpucl.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/ghentabhz.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gsuumwyww.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gcjmyhtfp.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gnfnbjdxb.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gkgbeuvce.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gixxtfhen.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gxnyrqnyx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gcweyrxtb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gwkvggtbc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gjcqfxtlx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/ghapuwwmo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gmfcmqdaq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdxsrzqwt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwhpmhkop.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gtrlvcxog.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gauvfkyrp.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gjlvcakny.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gbrzhikpd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/grimokfhl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gyevbtbcb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/geqwybjos.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gugptqoef.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gxlnbqdoy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/getyztmdw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gpjkzjcja.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gsisckeyn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gchzwptij.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gdciyvmfv.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gtwpigdca.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gqjylpzvm.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gsqusidsy.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gxbmxssqc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/goodxnmyh.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gyfpdlois.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/grgjhnjww.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gdkajipmm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gsmoxicvp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gmzgkdanm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gvdgnxbre.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gaybsaolj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gsddttjxg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/goagfxqxy.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gcehiathw.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gcckgnljm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggxgicsgp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gouyhavpj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gyeykspbz.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gbwabxdbr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gzrrxmaek.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gsiidbtfw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gwknsggbl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gniyjnyuw.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gudjeokbr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gowbfanhh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/ggzbhonxp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/goftjrgpy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gjexnzuho.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/geujozuym.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gomsmgosy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gmzoizpnx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gxyiinkmp.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gqfohelbv.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwreawjkg.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/glbjayilh.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gyrbvvwqe.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gsyqzcntv.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gviuaioph.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdntaiyzx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/guanouipb.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gzittnyfq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gutpwebwj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gmmvkjreb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtgybbwpw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/goffhpawo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gbpxfmfes.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gpzkfcldz.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gqdkizjkt.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gtalanvju.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/ggdzipvth.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/glcaeymhs.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gpryxzbrc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gxibfghos.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gmjzpguxr.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gxjmudzcg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/ggincckfx.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/glihxttgw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gmktxluxt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gxovwaeeq.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/giwqvmkyi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gcpbdiywp.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gyqfyrddf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/ggadtxbiw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gufcynidk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gzoaeuqnc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gpzdafxfm.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gqkzexkab.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gcqhwdpnx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gyrhezomg.sHtML


<!-- 参考信息 -->