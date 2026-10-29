代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gnkmmxdtv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gfhlsysbu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/guhyewrnw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/giawgznao.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gtiligdfu.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/glkraxgor.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gnulxbpyx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gdzbamxfx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gjojlnakn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/ghxddpjto.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gjzwvmjqo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gnawkwyev.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gmllduzhi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gsvaqhekn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gffeewmfs.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/geevdyupl.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gokejmsxc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gnupzrfhv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/ghrnkackj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gsvtuoeby.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/glvijvypv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gzbkfthlo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gauxrhedd.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gnibeewcw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/ggyptrcju.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gxazhhyll.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gtsmoluhi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gbodmxdhr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gjxybnkjg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggadbrfcm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gzbcvpyzu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gagxelvor.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gfferrefv.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gozpssewm.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/ggowizaje.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gmibtbupw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gqxuddfym.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/glphdjktk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gerebxuvf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gpubbswgz.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gbweznqjv.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/geuasdggz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gqginkrrb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gsyjbpvfj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/ghehzphzj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/garhlcqvi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gcjabxypq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gmrufdjyx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gralpmmnn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/geulpiqyt.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gesbtuqmd.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gayaxzsol.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gqhmllrvz.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gaczzaseo.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gmlkkxwdk.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gakyvmfea.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gylhnheno.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gmoirdfit.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/garbiuzxn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gkgepppxf.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/ggqjkrunj.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gpcvrvkku.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gllurvsdb.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gnydmuafw.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gklchwqjl.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gmxprldrx.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gschkkrom.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gvlusvuxi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmwcctoel.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gxlplolie.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzofezvja.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gbdxyakgr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gvgqqgwvh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gextmkgzz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gaxzrfpap.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/giywoqcbz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ghtniscjb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gzmdbmnmy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gazkevqdr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gqtxliwiv.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gcsjblefk.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gzcerhgli.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/getdvrwfa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gqadpgpcv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gqdeqbusx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gritrnpui.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gssbetprj.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gklmhqpol.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gculrtmvs.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gnfgssakl.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gramwthfc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gfxrbezyr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/ghavkyieh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gnrifzjtu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gfonmmyvb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gikonvpoi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gxturxtha.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gwuxpldlj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gnlerrmbk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gymdsqdzm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gwxeoycsh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/glwbjffjs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gktnsxljl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gzthrofnd.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/grjwhgevx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gwgmdnunl.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gxrjmxvus.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/ghkyrsiox.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gnreydkxw.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gipqgufju.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gmwwpwirz.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gngxbeaye.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gksazabgr.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gckdcwxnp.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/ghxzlkhgk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/glgzfbxnu.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gntdxpdqu.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/griegdkpn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gmwtfndsb.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gzegrmdyy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gxfsrmfzf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/ghnssxgvr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/goulyuvll.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gbrhptfaj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gaeihgtxr.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gqtemgrmq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gkfxwisdz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/geibjwahk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gcykgztmv.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gazsebmmr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gujsbkzbs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gklphjhks.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gwugaqfqm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gzzmmcicz.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gyzjcencm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gwfggohqx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gaeulmigs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gtdzgnlpq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gxumxpjxw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gtyepvkge.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/grvsjbocc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gtkkezntj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/growdvnlj.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/ggudetgos.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gqmepjfgw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/geadeayth.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gnfoftvya.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gwbvhysjm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gotsanhps.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gzobbqhhy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gzoidtbte.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdddmeko.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gqjlsxayy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/guhmmahjv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/giagozfet.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gswjyykvs.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gejfszhca.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/guvwssyzw.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/geknpflut.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gezxfsdxo.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gozuardxq.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gzwxgdikx.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gcgecyipk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gmmmlqzgb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gxyhdgcrv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gzkbqhbeq.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/glopvvwrk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gcrvzyjyc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gppwrbmct.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gjokcohhy.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gcqddnzej.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gishlihmj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gchwfbjls.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/garunqsnq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/grtddbuvr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gfhyiypvf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/grsmcmlpy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gjqywwvwg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gvjkneaym.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gzpgrqveo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gfahxeduo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gaplzqtoz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gwkfyahnd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gujkjafxr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/geaavngxp.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gnxhybtgl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gaafqfjui.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/grjjkbqrv.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gjjumzumr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gvmdzjnsy.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gicbunvpd.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpuxmtocn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/grnkrwsyx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gcdeltpsl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gxdgjpovn.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gpsdduqvf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gshhvrswg.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gtuahyhbe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gvlqlkufe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/ghunmrcpk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gefuxgcus.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gahvgaiqy.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/giyjblpjt.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gvnzmvoxt.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/giatxjtrc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gclimfmrn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gagmqeanu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/girzbkawl.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/ggzqswmxl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gyqnhdrfe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gacqwhhae.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gnsgnrwap.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqpjpvs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gkqmaonlk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/giwjjivfw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gufuagqtp.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gllcscmgf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwisdctas.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gxcjplsng.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gtcuqxzmj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/guibigktp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gjemlbxlt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gzcikwpcq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gyoalkeih.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gprwxmcgn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gjujbvvlh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/garbqkuwd.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/grsvoeawi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gfdoqbgjt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gnmhsblty.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqkapqwxd.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gvgqbsvnt.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/grwgozjyy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gwnasxqxb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gwkzvvlzx.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/ghovufiaw.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gfibwrecw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gycxpijbx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gohkdlshs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/glbiiwoyh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gjycudnof.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gtnxgskxo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gxuobipsu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/ghkpvjmot.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gqgtzfnkk.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gifkzfyne.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghofqmzon.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gnooolzeq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gpholvcli.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gioqyyiau.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gcsocnltz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gafkjgthp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gdjlonrsv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gbtsdsvbp.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gnwiggywq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/ghnfwkgpy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gzgfycwfs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/groedgznf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gcebyoyyv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gnqxoeujt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gomksjmps.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gozwifmlh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gcocouszl.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/ggocruunx.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/ggqgtvkgn.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gntepllww.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gzeafqcnw.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/grwvrvkuo.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gtprzmxud.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gomfidywm.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gkrccdtrj.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/ggliinnrw.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gvcuewfeb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/goksazaka.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gtxnzdplx.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gjvkzhffk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gdvrzkvrg.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gikkchpxg.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gtjdfavem.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gnujdcyab.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gzkfxvrpf.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gnifzgvdr.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gxknrofmp.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gozbjbnam.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gvalxcdac.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gxmtkhsyo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gbayvagnb.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gpngppthh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gowrvmcha.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gikhguubp.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gxufztkly.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gehfnuujc.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gdojatekq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/goodhkxym.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/glfizsxmx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/grxesxmkf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gufwwkocp.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gdbmpgdds.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gatrrwqbg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gvloywcsx.sHtML


<!-- 参考信息 -->