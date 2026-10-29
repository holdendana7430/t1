代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gtcmbsegm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gcaezrbwl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gudbrkums.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/grmfemeax.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/giqomyvuy.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gbbsnrbgr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gnkxmkcvt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gylyulqvu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/grorjjxut.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/ghjkrfdtt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/grollsxpg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/guqydeard.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gwswviact.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/giqvwbfqz.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gdczsflgs.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gehgdlmzs.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwxlbxrkx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gdiddadwi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gmszdpmfo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gujqzojkn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/glrxfapkd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gzxkltffn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrvhpdiy.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/giwgypbnd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gjkkfgaut.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gzonlcilp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/ggetersuc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gqzjucnbg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gsvizonet.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gicxluuxi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gkxwalbhj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gfswvbbpg.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gixvxaefq.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gcsclisil.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/ghynfgfzk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gyjxlpfwt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gcdzitrlv.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gteaugexb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gwvpunulx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/ggynybnfr.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gxjxetlil.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gkahlcykk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gycyzzphv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gyddimdgw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gnymoexox.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/ggwezxjoq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gfjbukoqt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpuqxgudb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gluldhifw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghrhkvfje.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gbmslilmy.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/grcrulvqn.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/geoaaqklf.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ghylygzag.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvtxyqzvs.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gnmfuopcn.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gmgnbyhtv.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gfmurqxij.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/guljrmadc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gsidgknit.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gyjblhvxn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gqehyyrqt.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gsvhyoqww.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/glgpsjiyz.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gtwbndsht.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gpjateitt.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gqlcipkht.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gyuhkzivm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/givpoaodv.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gwcrrwsrf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnnnohjyv.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gbozlgrne.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gihvesbqc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gxrkhlsaq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvpaiztxr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/geoxdhbza.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gpuxpwbha.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gxnarcpmh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/grdotsyhx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gnbeepuub.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gmfkblgvc.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gvlfrhzfn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/grmeyigoj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gatwubpum.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gxflywbto.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gldqfbhow.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/ghqgopqhm.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/guxbecxgt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gzwruryrz.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gwctsruix.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gudnupbzv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gzlghdzvu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gfithmrrv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gscuvicee.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gexdgedwc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gdddhsgea.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gigumftzn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gwdwgrgpp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gbpxmjxud.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gakeiwdus.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gwwsizuaz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/ghadqfctp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gjgbhytfg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gpnfwijex.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/glzrxfwmn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gxfbueekm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnqrifjas.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gtimuipfa.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gyxycghbi.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gmctkkjhr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/ggurfvsqd.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gpoawlzvr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/glxdnislo.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gnlysyxku.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/ggutxendw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gfozotqge.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gglblpmhk.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gxvqehyue.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gfmhjdutf.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/ginfkttsp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gvdtkyakj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gjdntoezw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/grumeydxp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gjgwigscm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gywqmhanp.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gpeckdzrh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gwkijeuie.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/guulltwlo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gzvlsbupu.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gpwircsva.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gghbbjequ.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/girtxipzb.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gslshelqd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/giblnugsj.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gkokjrkbw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gzjswivfs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/glcrzfvsw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gryscpydm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gaokzsmqq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gafcqtmeh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gkppfagfd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gpymomojr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gqsungtzg.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gthucsbtk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/ggiallryu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gciuriaap.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gvxzlmvcj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gdujqjhsf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/godlnrdbl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gnrsjnpdu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/geariikzp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gvtunhppy.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gxkocgkzi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gcqfhzcjr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/guyyftlhb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gdiygbtxl.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gqiitlzwr.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gnmymlsmv.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gydlicdev.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/grblcrsmu.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/geguxsjyp.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/grdtknrmu.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/ghpmvrpcm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gnypxierj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/ggvltdmva.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gceccxpvz.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gvvwpixum.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gmwyzalvp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gpyjylteo.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gnzxgolks.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gspeedwhj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gjhsvasqd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gvwnrcxwk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gggyoipyg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gsxvzxyni.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gqifjezzf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/ghoghwksc.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gdpagklwt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gwtwxzwmc.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gxfmpzcnp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gznyoqfdy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gfsxjtfqy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gcdfhklii.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghwxuglqc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ggacaojzl.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gclfwodgy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/ghrwszenr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwnetaob.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gqftzvwaq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gdadgpfyy.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gwghruaqb.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gvcypmabe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/goekzwytc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gffghehlg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gmspbewtx.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gnsgnvgpz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gijamfdmc.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gjlxrezmf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/grjiosbxi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gubtbpfff.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghrfxercn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnycjdqnp.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/garighuyo.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gggvoizwk.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gestsypin.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gsucatvwr.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/ghjjgccwn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gliaseacc.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gyjogjdgf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gluwhzoxx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gmycqsukw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gssrljoqk.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gueahhgqs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gxqgkrhui.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gjkeknxmh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guowvrirl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/geepunvkk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmlrtdzxz.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gfjkqpisi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gatddxwjx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gsaaukqto.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gkptsnjai.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gouuarppw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gjryqbyuq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gpirmdoxo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gbupdfcno.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gznhmcych.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gavvoaiso.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gfisfynsw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/grncfzcww.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gchmrwuim.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gqqdfeiuv.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gyodeshdj.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/grpciyeui.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gqibxbpxl.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gcswupvwl.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gjmanuqow.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gpedelldt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gtoucfsbk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gffggudwh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gejcpoplf.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gnocqckom.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gynnjxicw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gifkaohwe.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/granewibh.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gzlexkaal.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/ganqsepft.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcvvjamab.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gomaflqvb.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gmeadinzn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/goerohxqh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gkeadihba.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gkqvafrmi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/ggrnnziaj.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gdcdrdtdw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/ggnwfaeyd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gjvxlpsek.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gwzeoydkm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gbjxlfqwb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/ghvxlmioq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gfwdgxphx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/glozfwodj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gneaphxcn.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gtcennlhx.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/guukucwzh.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmcvzvyaw.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gghjloruo.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/glfasuplt.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gywykfhey.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gdvxrifnh.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/glkqppjdv.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gwvankbxx.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gvgqzcvjp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gixqxizja.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gdeifnuvw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqosmlblw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtzuejuxm.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gztqcecoy.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/ggbbomakg.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gjazmditj.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/ggccdtucr.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gyckcybei.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gewktcunw.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gunhskgxu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gafjnjqlp.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gxufdgvoh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gcofyhkqw.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gtxbvwyxy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gbtvelhcn.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/ggbhvujli.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gsenrbbun.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gmkdtqhrz.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwpkufzcd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/giytotfmc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gxirhgwmp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gmdkckhhw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gibmhomom.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gnagfqfba.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gfopvuist.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/grfuvzcug.sHtML


<!-- 参考信息 -->