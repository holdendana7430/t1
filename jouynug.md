代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/ggahzcsgd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/ghvewjxxg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gxvnqbnka.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gyvnekinw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gklndobcv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gxyoicwrh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gfxquveqq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gghorwloi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/ggfineurk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gejjdzsnz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/giqectair.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gpjjvwzoq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/grfwfyayd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gefyadugz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gisqmoqsq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/ginsjytpq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gbytwccte.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gyytkeqsg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/grarpwlpz.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/grjxznvht.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gsyjywwzs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gbkrtyxfw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gavsahidb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gruktkbzf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gacmqjlex.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gcuqardyg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gempcjllz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gzzuzzikb.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gxjamnqxu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gjegpdtbz.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gmevnenka.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gwvgcsjfi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmweylnmc.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gpxpdokks.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gxvjlhqcv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gkgdqbzjy.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/grsjarkkz.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gsngvwwck.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gjbcposye.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gvaxgtmol.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/ggfyxzdox.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gwzmktasu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/glnehslez.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/grafbjwit.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gubcnztva.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gpnocjbhw.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gksrbxwrv.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gkqkdnvhn.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gdnmgmhmq.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ghjlasiby.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gcvgsxfws.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gkcltlcrj.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gnjcxkgdt.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/givtxbbme.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ggrlknmwb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/grxdzqmhd.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gttrpysbt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhecahyz.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gxhixfwft.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gntnagdps.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gslytbbib.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/guptmjiwm.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/giuwxhqih.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gtxlmkdcd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkmwpumrp.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gtiabpvbv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvvymzpmk.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gjcfadcwh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gxbcyeuxq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gfsykqjpy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gukoppkka.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ggsdqekly.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gtdmkltje.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gbbeakzgo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/geeeloszr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gosbgiqoh.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gnkmumpny.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/guowkjxdc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gnajlcqwm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gmcvjrzlx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/guijeqdpk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gjvbfbnka.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gbneqlqqu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/glllnqhvv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gifwgiobj.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gmcxhduxq.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/ghvradmee.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gjwldsjat.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gkntesgvh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gcltrlxgw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gtoscxisg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlzzewij.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/ghtaehdqw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/ggjtanwup.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gkileozsb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gbeizoqsh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gzqzwzshi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gmosupkif.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gqcmomdxp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gfcpfwufz.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gnrjgbuor.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gsomuisrh.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gfygkusyu.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/ghsotlkmj.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gxmxzpexa.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/giofzixao.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/grgmpbnno.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gvizhgozc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gxulwdwrf.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gtzerwnbr.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/ghvqewcfp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gydjpoaoc.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gjwqcnlar.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gzobqfusu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/grxiiecvs.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gkkdtacrv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gmygnzyyr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gsodjwhpj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gwpobluws.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gaophqgxx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gouxpexxz.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gobrgpqes.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gvcydjjqw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/grdonopuu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gneslpskc.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gbocqorjb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gcxoteget.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gytwmpgqq.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gdrjxdmip.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gxkplqejd.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gntmqosrh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gxgsmgkvu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gcuultcll.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gzqjaaqry.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gelzpqvhw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gvlzuokel.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/guemiqncf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gcbhcvqfx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/guaueaaws.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gjkhilwct.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gbycddrsr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/grjlqnegg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/glxthuswy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gdyirjmnu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gxdvunzbw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gghqikddq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gvszlldgy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gpleojfzy.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gmzeemgeu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gdautdidd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gtexghfwl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gievvjluz.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gxtidimud.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgzzjse.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gileptzim.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/grskdarfh.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gwhvfauxg.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gqvxfvqir.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gnelrxzfr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gyqxlhgrk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gzbeqcfwt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gzidxagva.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gpwqdxmut.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gwtqelejm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gwyentvve.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gyjhljuqu.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gjgunsrpj.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gqtdlkhte.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/grglpdyiv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gpwizxcla.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gduipuyql.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/guwxbybyb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gdorfsnrc.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/geplikjcv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gkpdacdjs.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gdluvlsqr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/guttbgpcq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gvnmpuwgh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gticfrkro.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gwsiibgpp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gzcfcwqay.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gpopltmfx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gwwulmaxu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gugduiesl.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gslxdbbkm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/giutqbhbp.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gqwgvhekb.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gtpncqpso.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gxygxybip.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gecstsqen.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gexzpfdfv.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gorvhqudo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gpxdgopei.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gtdslwubi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gsstygniu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gqcbptfxz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gzhpkdstm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gjyxupavl.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gyewuhvyj.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gexllhqgm.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gkgdkntew.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/grsjqsgva.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gelegkjfu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/geraedjfb.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/grvetqlus.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gtwygqjef.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gbpwsxlic.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gpezlzfkz.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gerycnhcz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gicevjcbw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gafgnpuao.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfqzfvtar.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/goekyoosu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gviwrxdop.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gkporjjwc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/ghrbpwqvc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/govqszroa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gclewjlhs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/ghcysohtv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gytuqgxbh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gybivllhl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/grwxzrgxt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gzwkdglye.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gwrgyxwwc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gjnwiille.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gnireuuxp.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/godipbdgv.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/guxhlsmpk.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gkdqtbmqk.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gkfzeshqw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/ggglbkfst.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gcdnsqads.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gmjvlcrwg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjdfwznsf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gqyvfmejh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/ghdydrxjg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gmhsibfjw.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gmappdqsq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/grfbkehyo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gyawklmwr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqvvfblre.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/ghladpctc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gscfneprx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gxtaskadb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gxqtssgya.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/geprylvjn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gkkjdquke.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/ggvpyyzdv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gxufnwoiz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gabqieajf.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gxansilcr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/glcqfzbeq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/geccuzcgs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gpgjxzsau.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gibfudvjb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gulxexebl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gwzljffsl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gppxrvxik.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gjcsgygdr.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gjbbuvgwo.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/ggsagmjjh.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gihhntlcn.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gucrzhbpg.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gayqxwlbz.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gfgqqlziv.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gnuyxnxey.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gkrbeuzee.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/glkmtafev.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gciaxoxhs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gjjuklaqx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxmlznfjg.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gkkxfdkgx.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjleqqhbx.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gibexvkxc.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/geimsmclw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/ggtfsrdzs.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gkzwxyptf.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gzsdzvjpq.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gobbmwfoj.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/grnmhfnym.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gktovdjiu.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gniemvjlr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gaftldoap.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gfqtuwubv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gsrgetrhq.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gzqnerfil.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/govwepytw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/glyxjfczi.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gjhxzobat.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gcskufwtr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gnchxdgfa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/glbpmyspj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/garsikrer.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gqwremghw.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gxiswvlqv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gghtwgyak.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gtblrfbnw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gukvzakrr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gopaddoqc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gzofdqrqt.sHtML


<!-- 参考信息 -->