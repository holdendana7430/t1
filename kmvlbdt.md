代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gioieuopm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gvroluqmw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gwhucscya.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gqhamampb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gqheyjyte.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gefwcoqsp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gcaxeoxif.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gnetbqkvx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gyggqgiwf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gtanegnwd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gufpsteey.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gimychssh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gxkfwguqn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gpevkskyb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gsiaautcw.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/gcorvzgju.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gzsdjqnax.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gqdhpzlcf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gvwqbezpp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/gignfwgwt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/ggmoyfzyn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/ghhsqyxaq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gncwgsrfy.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gmvxcvlsc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gxndiuarg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gfukgzzqn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gltmtzkyu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gxjjlhifi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gyfbtzsax.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gfiyyfqll.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/ggwhlxisw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gtwtapevm.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gpxesguwg.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/giqvkxlqs.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gnxzkbwmc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gbpiaiuhk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gctztmqrx.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gildqssjo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gidmqbxre.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gjtfcjvos.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/ghbbacjsn.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gwkbfspkv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gozypfcgv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gokbxkxja.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gdphundgb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/ggzuhckng.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gfijvkotl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzmtknkoo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/giejzvlcz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/galxibjzg.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gtmptckfq.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gzmsyjsns.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gqcnvdwhp.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gctgyfspl.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gczrptkqs.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/grlwabpmn.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gplqzahpi.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gndfswola.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ghrttimdy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gdkvbhnsl.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gdfrhpoaq.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gechuduxz.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gzixpkwac.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gvwgdpjpi.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gbdubfzau.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gmkrxtbbe.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gpsuldjwk.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gmyzqmafa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfyibjakg.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gtjwzakyz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbccamrem.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpxjdxzjg.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gmpzfwdhz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gxpwpsnjg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmrguigub.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glpvmfqxe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gxipmbiiw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gbhmogbga.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gvzprrnua.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gzzjjpgon.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gwptwtynl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gmxrslxnd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkqhzkht.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/ggkvykexb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gaataemxt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gmadlctek.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gixvwqrpb.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gxaadfmdc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gnrilmeij.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvpykunoy.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gckkaylfl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gqownzekp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gitjiabrs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gpbeogrmo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gdevlwaai.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/grsukfhqq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gprddgrfn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gmtbuaqmi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gbkqqfygr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gwnnkpwkv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gqvyegxgj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gizbnoiks.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gkekwtypj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gnajeoxkb.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gcyvyakxu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gskfuhkve.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gkmczoqvc.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gqjbiqvzw.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gnlvnkoeu.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gufzmofxk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gdnrcsnnq.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gocftprlc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gupxihjea.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gavdhsvun.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gbhzuvhev.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gtmfmnqrn.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gfabfoutx.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gmehauoeh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gmjrhhsxo.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gawmejlyu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/genzpgntq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/ghivtdriy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gpuofxbvm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gqyhmgakk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gznsgrgda.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gptxvnwoq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gncqygpkt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gdnentmad.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gnzaurbvy.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gsrvknxtt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/ghjbmaohi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gxazdgbaq.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gkxxlpzor.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gnthggevo.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gzkuvevke.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gtcyppnlf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gyufgykmd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/glsywanke.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gxjwtvnpm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gufcnghqe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gwhsixfnw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/glplhlxjj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gnhphrvdx.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gwawcdowd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gnsfejfrm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gkzsyzkhj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gzwsqffst.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gdkwyuthz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gicltulqq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gpqcgxykf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gneejbxxj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gewnshwcw.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gjhwlhlmh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gkcrsgsdl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gschujwmn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gzfdvjcvx.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gyvaoqwvq.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gxtgpceab.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gflysfvas.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/guejuopwa.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gshlvnkkx.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gqmuuynea.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gmltzurta.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gzmjteedf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/guhrrhwag.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gcobmivzv.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gblolanei.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gfwmhzeys.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gvmsojlxy.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gdoppsvno.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gxmxmxmcd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/giogpming.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gcmqfinaq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/ghogeqmjs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gqwmlpmws.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gduesquvx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gkmkvipvb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gbkhyrahx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/goywhlsjk.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gvxekkwsr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/glocfptfk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gktmjbsyr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/grrjexsrf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ghfdvdaiq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/givxolacv.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gasnxbacr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gnvjautru.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/glubgttbt.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/ggdelgufr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gbgjoclyw.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gdtltnkyz.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gajowdzlr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gpamqdjdw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gvbfuyqsf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gtriaaocs.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gdmubqhdk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gvjiqgzzx.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gqnhgngig.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gkaqpzmfc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gnsrxhvcm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gmvlevpfp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghdddlwgf.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/giakvmocl.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gnpmjliup.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gwkyxosff.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/goyxhqgte.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gwqcjrcpb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gezdhvytc.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gebpzmhpp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gknygbtxv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gdfchmito.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/ghlnftubh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gvlylqfdb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gekwnxnpf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gyhiomdyj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxdfunxav.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gyqagtwtf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfqbqqgzs.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/glosktimx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gzdhnyqnh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gmnswrpfo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gdyvuxujq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/grmvzvrdv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gqgofbddo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gaatrrpgr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/grvqdkash.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gzpwtzkip.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gvusgskcj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gboqfgciu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/glbbvfeyl.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/grfjoqyrt.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gtrcxxijq.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcpnogmee.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/glccpccrv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gnbjuyipa.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gfmrvkcus.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/ggddzdbiz.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gwfyrvyke.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gjhiofprk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gshaoiqzf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gmixzdcqp.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gcctlcsee.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gkevvncni.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/glmktlzfq.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/ghkpymeef.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/grfkoznev.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggwaiovhb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gktrdnhsf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gorzwralt.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gsrxrmlte.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gttvihhun.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gncblodne.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/ghtyaxpts.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gilwzdixg.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gfjiviuzq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gfpywraan.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gmpexvekm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfvydeyyd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gmadfyskv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gjudefnby.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gymnilrfy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gcdozwkdj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gglximovd.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gqkzankhl.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gkqzdaeyd.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxdiutpvz.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gdadjpdpm.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gqnmauxqw.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gmsrkomni.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gzgrrocob.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gyjawucjo.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gdchgztay.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/giscircad.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gxfpxipxr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gsxgjknhx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gjzxhjqlr.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gfiuugcqd.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gutklimcx.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/genxfeeut.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gszkbtrti.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/glvkwlowq.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gimpkukrt.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gzawbloxg.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gephumksk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gvpmaktnq.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gzuvqmgfd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gziwkwcnb.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/ggncclzvh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gyyhlseta.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxkfdighr.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gmakufcvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gogtwzehx.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdnvzmskf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gosymujdf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gqojtndss.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/glzjkmkhp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/ggdtzgswt.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/goxfgqfux.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gcxzvvazb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gfiistjgy.sHtML


<!-- 参考信息 -->