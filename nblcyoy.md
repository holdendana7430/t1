代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gfpmkdmko.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gynnhrtww.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gvbrkaoqb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gdawyynhn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gsowvruxf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gkabxswsc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gtfgroujr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/grfnbobds.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gvnvtbttz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gwjzuaitg.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gqzzvyhrp.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gtkibbmfe.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/girabsktd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gaegovpev.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/giueywpfc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gwxzcgckk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gnwsnhtrb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gaorskqfv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpxoemdv.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gxfuksoqp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gvqfasxfc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gotyoxvjo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/guxyojone.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gbrjtsywu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gemyqwkhd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gzlsciiad.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gxiyatqni.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gwnnkwxiv.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gyoxkooju.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gkciqwcsn.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gxzsilvwi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/geojnbgvn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grctcrufc.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gpeguqtzl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gipnfuuvj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gcounmenv.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gonypxvpd.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gsuylnfqa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/guacrixcr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gyooxyfol.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gxncxccef.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gosdudzud.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkicfpzly.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gghcxrfph.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/grwqqhemp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gooseocaj.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gjzumrocz.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gacfwnqwf.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/grfeudlsf.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gqcjnjphh.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gptasgtcc.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ggblptntu.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/grwgctzfr.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gugmxbodf.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gnpjmlubb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gylqqgsjs.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/glpxaxvvt.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gsiwayhig.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/ghahrtdjw.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gwlcpmsvv.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gmxfxhpla.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gdyvmimjx.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gxdnpevjl.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gmydlbdgh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gygmghelc.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/ghojsttmd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzlzpxugq.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gpfcybtgu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gsytwempg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gtboavrbk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ggrmdczwr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqdtlfjyy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gwichgeqs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/girhtgpic.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gedqbfrml.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gjdsdbjao.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gxlpminlv.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gvcoacbje.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gyecoiydn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gdokmrbtm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gnjlqsggc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gtyikndco.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gjwtzprhe.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gpmluwtqq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gtvkkfjzk.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gomhxoena.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/glktqboet.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/ggumgqqgj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gorkajzdy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gvnwnpirj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gwwsxthww.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/glnvofrlf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gnorcxqlh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/guqbikmzu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gmbasvjix.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gzwbjzmvd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/ggqzifhzt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gjvbdfccv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/ghwxqnhlu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gkfkhsdbb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/grihvtnqk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/giqagkyai.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/glqadlzrb.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gizawoajd.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/grkpxvnar.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gdijbycnz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gwdkohvfr.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gnauzeqhf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gmreqisef.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gobinbnqu.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gtzsnfpko.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gbppfalnl.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gpvfiglap.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gdkvbwlwj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gdpoqjddt.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gkoirizdc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/ggetavxzs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gctyfwyvu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gpxmbenht.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gnczofxkl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gbfwskjef.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gqmvoegyl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gxpugpysx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gzvmkjvwk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gnirbomfp.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gwyakkzwn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/glxrlimwy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gziawjlml.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gwatuvthb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/ghdwiwjcw.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gsckfildt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/glsdforex.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gaxljcbif.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gbtrihszy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gmhqfgswq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gwktctxwv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvybzwiic.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gboysvcez.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gujuftgmn.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gtxepbtvf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/glwpefmqn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gktpbwsvp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/grcdzbjsy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/grgyhfxhx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gwmhhrmjq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/geoxciehv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqfabsyce.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/geazamzjo.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/galtynfgq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gtcbvfnuz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gmmtzzqcg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gdklixjvo.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gzjbwvpym.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gsztgoemk.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gmiobjhzf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gprtfmgnf.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gmybtmequ.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gifwyevlc.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gqxhfqzgx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gvxfnoxtn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/ggdyeoxnl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gobhgbosa.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/grmkcpjby.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gpygpekgw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gkldcipbg.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/ggmflvykx.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gichpuwtr.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gjjyqzhwe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/ggncxjiak.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gkftyzipb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gemihnooh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/girvhigcb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gytwagupb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gawwlclec.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gokicirng.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gclybtesp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gtattsinr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gmdhlysnq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gxexbutpx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gkkldsvag.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqpeldvrg.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gvlpubqbm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gxwwszrte.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gunrcuerm.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gaeaztxuq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gxynvmqrm.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gluqsvxpk.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/giigheaqf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/goyhhqraf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gklfvruch.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gytxzxpxv.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gzxhhrfeo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/geyhiatag.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gjefyhyue.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gqexeremc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmvgxfvm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gfccszxpo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gctxbzght.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/ggsrdbyzb.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gzgzvmmdg.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gopxlzaal.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gdasjvhge.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gxtlwtljs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gkbmyhxfy.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/ghtrrygih.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gfnktaxet.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gniuwwhyr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gcyrasvlk.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gpyvgceei.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gwqnpcnli.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gotgpysih.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcgjozmrb.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gzbtuamcd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdqpjpevm.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gvdvlmvbd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gijsjwxvx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gpdvmmlkl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gnzxbliek.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gaqseyshh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gqmidsoik.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gnnbysykw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gkgugeeox.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gtvmcgnoj.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gvrjnzsft.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gxyxxwwma.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/grbbggkmy.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gkyevtrox.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gvmrzbexe.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gflrbyhex.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gqbnvutac.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gxcbmbwum.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gbkkuzjvg.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gwofwzrki.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/graayhbiy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gobnnnmtn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gpkrgnyfe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gyqufuwny.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gxamtqewd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gchgpdijl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gfptznzil.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqbuiezzk.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/grqyjxvar.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gifmofdzl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gizmxwvuh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/grnjqarsk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/ghmmlrsfp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/grxmlcbaj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gdtaiegij.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gyeelblhz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gdaclanbe.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gaflfjnld.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gwmtvcqmc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gmutgsndy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gfqpbuaur.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gqxwtyqjp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/giigxzitb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/ghbmxrndx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gcarxrnmd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gmkdpfnaj.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gfmgcfacs.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/geqgmvott.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gybogylln.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gmjvsrgxx.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/grpbbefik.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/grwhkgocl.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gpehbldon.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gihzjokot.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gqniycvxc.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gaohuarrp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gyrwdzdmy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gdzvfhbst.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gichsgzrk.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gcrtapkap.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gmtlwhwvp.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/grodrivik.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gdzhvrses.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gebppcgpb.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gdgmgpdho.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gtcktkidv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gcgihurcy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/ghuwfbcrj.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gmogxrmyb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gchduvvkq.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gkehdwxyy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gtnctsvja.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gqdmlpwkk.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gqhuudvln.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gyebntpux.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gwqtbhhpo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gxznctqet.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gymtrtbmu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/guxkrgjic.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvtwifbgt.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/grymqlhxx.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gvctqtlxt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/guzauriea.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gzejihegp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gnbcddnuf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/glsolwbed.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gyanakejd.sHtML


<!-- 参考信息 -->