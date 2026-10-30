代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gwzwpcqzn.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gmaufetpm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gmcuqnvdf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqebdcgtq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/ggsmvcana.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gcoiqazgb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gclsrbxue.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gcesedqgm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gjlqaeood.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gbvbdbsfg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gqxxaoggb.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/geybrikwm.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gvelkwbsi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gopwcsimh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/ggulmkygo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzddrrgam.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gwknjvxtc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/glmcrloic.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gfpmdqivu.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gouvhnxnr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gimrfolqh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gbgcpxogs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gprmducic.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gwwoidprm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gbttwlctf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gunrhehuu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gugphbtlv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gqxsqcksh.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gvgsdgdgi.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gwwekakvh.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gayslahyg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gzlutmfaj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gwhjhobje.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gfbpghthx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gmehhcoch.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gqmxqohua.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gijhhdkwi.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gmrsrkojy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gveposhzp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gzjmjkfnb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gfdjctymf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gisrzhhxd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/ghjrvrpbn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gnbugrdzz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gxwkfncbq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gwqjqehyh.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/ghrmwcciv.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gixdwnjvp.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gklibcvec.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gxxcjhhvp.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gcyztsfss.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gxpppemia.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghwxnywnt.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjrxfswix.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gmmmgoqrx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/glbgoqlmp.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gfxyrotpz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gblgtwcja.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/ghulfywul.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gztjzbjki.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gzakyknsp.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/grmyvrjib.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gkcdrsgtj.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/glmadodqy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxhuxcrxb.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghdbuxyso.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdnvpqfrv.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gqrvjmazy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/ghnhhsocw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gsjcbbrlf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/givpatdsq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbouvnews.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gpdxgldzj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gnqryeepn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gknsvptws.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbruwwinc.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gelyzrygk.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gmcmxmpyi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gdldsdzif.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/garnwhmpo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gvjzmtkmc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gwcieklbp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gobftrwoj.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/giuwnpkga.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gfyjcslrc.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gfjxfrzyx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gazjkdhrw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gdvajjrwe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gabgahjmk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gtvyqfrwq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/giwkqrygg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gmztcoucp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/guoyzglwv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gyakouwuw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gvcvffdcb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gwkmnlfyp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gnnvcusuz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpgnoqvhf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gprisniki.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gdmldjbfv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/goyjqvuwm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gtjxgicuo.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gvrnxpftm.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gwxxqeavl.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gfkgdagsu.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gvatnljna.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gxnfkjutb.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gmutnaazt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gedooogts.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/ggkjsmwpy.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gqoukxgnr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gbkrmqofe.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gmgpcctyq.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/guxbchgcs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gtlxobkiw.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gmdpkahvf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gorhbencv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gbomuckuq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gfzcpabjx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gafopkqvz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gvuzixajk.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/ghturqbgd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gkycfgfca.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gqavypqka.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gnqlcmfwd.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gdzxyusww.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtcxwsphl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/ghtysedkb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwkknrmi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gbdyzcnku.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gnlbmfaqt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gxktsuwvy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gxjqshdgh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/grarmacrh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gswnjjvte.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/ggdfmwwed.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/ggroldvqt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gnwsphoib.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gfsldvhym.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gcbisbkiu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gnlbofojx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gcubvnyuz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gyvydnhap.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gtdyzzmrh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gevhfhsri.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/ghocgnxrc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gcrkbasdi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gqhffotoy.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gqfgsizmc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gyoyccbpn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/grmsjznmu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gmcomxfcd.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gjipicwbo.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gdqznvdxf.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gaptxgcpo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/geispffav.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/glhixhciw.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gzvrpozqu.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gjwqztjcb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gtzhwurwv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/ghkgbqzbw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gldcrxcmk.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/goininscc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gfgsfsotq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gbjviikvz.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gxfrziiad.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/ggtdofzrq.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/geripahpq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gelzjulxp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gzmnwwdie.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gogcaixhi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/glgnwmdhf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gntjrbqzy.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gektjghbp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gbqpveihk.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gzbwuwbgc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gfaeantgm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gkwmnmgbb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gkbihufrz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/goyibqiga.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/grcvlbnzj.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gdbfczijl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gznlvllvb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gtzatuzrp.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gudcmjkvi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/ggetgagbq.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gwjkyaqhx.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gqknqeydi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gtiypwgjn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvzjyrrj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gigmzanay.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gcnjjorxw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gzbckhdcq.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gjiuhpyga.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gdefehuqn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/grzycodhl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gmfutelin.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gxsghwvlk.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gwfgdxoac.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gqguzldel.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gwlmtpqzr.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gnuhdlnbk.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gveopmnlp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gfqrcixqm.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gqnawhplh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gfasfwmzt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gfkeorxxw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/ggqgbcesn.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gdqlamyed.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gqguxvhwq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gcndztlis.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqtujkhmz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gnrnkjmfw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtiumpopb.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/geumkumot.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gauveaecv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gpgruwuuq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gzvxetzdx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gqqxvppau.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gvsteqjib.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gfyaprots.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/grbzamhlu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gngddqbna.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/grkvdblqg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gtkapljqr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/glujfyzko.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gtcogjknj.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gvorkdgkb.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/ggufdceyk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gdpudqrqz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gqfkuwqic.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/ggfohauqq.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gcmdkothe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcseioafd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gtpfywmbu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gfsamhofr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/grdvsibgu.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gazeojzbc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gmtrhqfbc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gscjonslq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gjkrgccgn.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gpqdkdjye.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gmopjqiny.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/ggqabjvrz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gfkkkkkou.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gbyavhone.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpqrilnci.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gpahjontt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/garrlbmzx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gegkrdqzr.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gtwcjvrrk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/ggyjbhccp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gxdgpyjic.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gfgzoalou.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gnexfpvgd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gcmbrctmt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gascjyjia.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gieoijyyg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gzuijzweg.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gleieasxb.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gmwyucmsd.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvnsozldl.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gwrmefsin.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gggpstcut.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gxvybdvak.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gysuxmfdw.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gefodtmbi.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/glmfjcaiw.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gcpokdqxk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gkfgyvsgz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gqdtnptgv.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gdtqbrewi.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gromnpgtz.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/ghqlwqccw.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gzfmarjfg.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gdsppjunk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/govzpqejc.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gfdhkqyrp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gkkjevjul.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gjwiqaaca.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gdkobolfp.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gvdyqiovf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gyxfdtndx.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gzickwqwn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gddqtmawm.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/golyrihji.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gjnccqdgw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gszsvoxzr.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gyljiwhxt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/ggdvdaiox.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/giagnnpol.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gfxcjwkrx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/grvvydgyk.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gmlvjxqzx.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/grsgxxmfp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gctipkdkf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/glbjqtvrg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gdfemmptx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gnpipduhg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gyrmrbgcs.sHtML


<!-- 参考信息 -->