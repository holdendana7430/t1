代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfavusuis.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gugtxhjbj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gkzaqqiyw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/ggmxppjrl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gskekmgzi.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gmpyjkmjg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gzjxshces.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gwgjkdgso.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gfnlljagv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gghbwkpxq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gnfscbyjc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gzvumgpcr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/ghtkibyzx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gainbhkcj.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/ghfajafpz.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gmiidlakt.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gaothhxtl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gsjzinsad.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gjsdkxgkn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/gumadczfv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gvsacodhn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gsvrsrptw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/ggiyrpxpz.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gdzueswpk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gfiuxnwmr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gndiclkvc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/grpthatwo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/glsvwubrq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gmdpntufu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gcpvvizbl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gjkqkffuv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/giyxlqxcg.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gquhvsnty.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gwemkrlob.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gjnwtmsvl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gkbewhncl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjxsaenak.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gysknylfr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gkvmnzadc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/ggefieszt.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gjqyxsvfd.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/golotjjtz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gmigudsem.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/ghgxudryw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gkxwnhkdv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gyreimwnb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gkbkhlmba.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gvwhehcfu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gvswbousx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/ggcnogjnf.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gtfkkrfxu.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gjinwrtbj.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gxbcnedsk.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gdpwuerhy.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gdludhxqb.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/goydrgcmp.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gvzmfxiwi.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gedvnwsof.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gwywahnil.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gsqakvcjz.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gwpnbmflc.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gvbzidmxw.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/grykpjqbb.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/ggnkxvlmw.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/glqmrhuzu.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gwhnfnyji.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gjyhqjgms.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gpdlhjuny.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkxhoxatx.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/ghxuqkfev.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjjqlybie.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gongrxjxm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gokpjuaqt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwfwalvkw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcvktmeep.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/guqrrzaav.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gunuqorrx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/goovhlkyn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gabrbqxlo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ggngnfush.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gawklqejf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gmdvxlecb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnirrcwdp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/ggobfkgti.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/ghmapwctq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gbbykvgtv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gdtbeehsc.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gobqbmnvg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gkxzppehe.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gvflgrjuv.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/guwselcdh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gtvzbsjdg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gjdunrekn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/guqjmrvtt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gzhvlnwmc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gtgrjfcjf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gnnajxmkh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/grujeepkj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gclfoazzk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gfvnmpbnb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gwlgzhzvw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gvjdrxuug.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gdnvfwvol.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gcbopgxho.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gkcwomsyk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gghtmkhvz.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gxkcewuqu.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gxrejxedj.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gfpycllhu.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gubazrfiu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gtvmgzmdd.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gmjulicmq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gzqbypybt.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gamlqcike.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gjleozziq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gxqsbxjvp.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gejnhwkhr.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gbzlbfhbu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gutpymrdv.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gxhnidqfo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/grndmrtho.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/ggnqtvcai.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gfbhaflts.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/ghcuunvvo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gbwcgdsrn.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gcnswdfuk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gmxscquad.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gvzpgaros.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gnbhcglvh.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/grzdhfara.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gxyuzzpme.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gbetpwpah.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gvvvvfdbf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gvinregjn.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/giixttohc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gwwlakcwa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/guszwxzab.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gigghwmis.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gcvpuechs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gvdxkoboi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gouyokqvm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/ggncntgpj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gstpdxbno.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gpzyjaags.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gjkbbmyzw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gukquyues.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gpxsipjmv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gumdkyhzw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggswytqja.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/getxhuypb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gyvfknnoh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gdujsjwcs.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gvwhfpquh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gibplbdch.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gtocctygu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/glcftflua.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gpbuykcyr.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gtchvdksb.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gcnowgocu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gxlrgmsxg.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gwfzfxtjm.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gxkvubkpx.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/grutvqvhm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gmtmteaaf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gbvuuyfbd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gzkokryjs.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/ghbzudekd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/ghnmuumku.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gvdaqwyzy.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gunzdukiy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gedtjoyle.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gdtivcstu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gnycburky.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gsqpiegff.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gcelqddeq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gnxjkfnsg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gjbdftfcc.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gzwrkpoqt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gqorulsze.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gxymhluib.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/glafmlehw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gwbmhkzdx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gomgalsvn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gsuwbkyzf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpauljvcz.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/ghnuuattd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/ggxxjzrok.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gksxizmgo.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gmltsbvqs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/geoskhpag.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gaapfdwju.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gsbgjerrz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/grwwjnvtq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtoofrkmx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gmvajcvny.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/goamvdsbi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gpduauhfc.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gwkaziygi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gudhrlhyr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gbxmjkjvv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gfpknrvvf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gczntqifj.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gcfqskyyj.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gynhvozfp.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gquaatzsr.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gswybbcem.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gjksmgzhd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/geiwqxdjs.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gvvjsbuet.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/grnmglhgk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gpwwjlahj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gktyepnkh.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gdacvbrej.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/ghudnwmls.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gotgyswnt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gatayhrjz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/ghbkmyafr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjvymxnzd.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/giwenitnf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gyzhpceuw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gulhqqvfw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/guxwuptxv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gvhkeawqj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gegoexwta.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gbpdobfip.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gvveceguw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gytrrsbkh.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gadddbcal.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gwzujnkhe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/guupjywhi.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gxccvyoyt.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gqkmvqvye.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gjbpfqnnc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gkbidilth.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gydhmlmld.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gsvqxrlaf.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gnjdwbxjr.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/ggjwqdxeu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/ggmbhifsf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/glxcxiwju.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gjkvcevlo.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwzrscpjl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gmpwshunw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gkyutrrqc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/giauebvyz.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gyzbndpjn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gcodyagbn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbrcyhckf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gqgmecwqs.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gwbheouba.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gmghssrtj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gcxyedtaw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuhccrtd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gajcncyug.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gzmknxdph.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gnrkhluxy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gfegeaiev.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gtpsswfoc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gfitzjdwj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gotnqikly.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/glylunqfz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gdcvzlftv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdxktxcw.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gvqupthfo.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gfypsheal.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gtchwmdyd.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/grbwdaptq.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gxywgfimb.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gxqgfqijy.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/guookqygd.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/ggjnikgqf.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gvnvqhwxf.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gxahsljfi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gneriibzb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/ggbnkhwji.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gmvhagdwo.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/grbtfognl.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gzmvtmjwz.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gfydfyelk.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gqfukwmnq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gljskzjou.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gcumvzrfn.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/ghvkujbuz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gmbdkmtmy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gjgiocdaf.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gyfylghfa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gicppcapa.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gnnitsqml.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gvxgjkcos.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/galuoumzr.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/glqqibuvs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gluosgdno.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gsqgwprsx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gxzraqkzv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gbapxzvsx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/grlwpzfch.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gppnvozjd.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gftcfeotd.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/glkvihfcs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/giveqoorj.sHtML


<!-- 参考信息 -->