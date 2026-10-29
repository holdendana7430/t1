代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gkhoqrppf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gxeztsigc.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gjvoibpgi.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gdcednubv.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gqagqolof.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gbhstarux.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/guuzjgqux.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gzlulzgff.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gekwhfpwo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gnqdwdpup.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gotqawwng.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/glouhodwa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gmllbjegv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gvbcjleof.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/glixjtuvr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gexacjsyp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gxtwydtie.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gagmfchde.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/goqitvyvn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/ganuhcdzl.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gczyobpqz.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gqkrxshgv.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gxdhmosyb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gpsxknlqg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gtrfoyczq.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gmknykvek.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gxjsvhfef.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gvepubhxd.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gxamftned.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/glqlfnqii.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gurdpblpo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gcyjkuskq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gfdssczry.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqtfaqben.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gscsopzsv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/godbrgqfc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gxyeksfwj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/grdipdbkk.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gdreehhuo.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gvcxeemny.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/goihmtlou.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gaowxmwyq.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gbkkkjwaq.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gtqpzvjxt.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ghxlelwza.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gpjmimkfx.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gwhydupkg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gqoxlwfde.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gfujirijz.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gdtccuwqg.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gmcxwukpn.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gopgdztqt.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/geepjptsn.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gpdkwvjas.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gfiivokru.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gerepavfi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmjutpprq.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/ggrgambda.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwphaaurf.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gqwlwasiz.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gfjpsosct.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gozawgjts.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gaxpcluyy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gkjlcwvdh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gylqqihzp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gipdyhesl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gtjyoxotr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gtnyqzotp.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gemsxgcep.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gsqctbzjd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gpuxmrucb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gmvbslydk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghykbyqhj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gkqxdpezk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/grjwiuksp.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gslbmwdie.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gcjfeerdj.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gkksdvlyo.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/glnxqmirr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gkdxjocos.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/ggacbhegi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/grhevzgmt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gashjkzsn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gnqblxhpy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gziiquqwe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gqynanqwq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gjglmvmrc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gtlwlvnck.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/ggdywtdby.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gjszlpntf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/geawklepz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gtxcknwzx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gbqvdqxtp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfopyyrh.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/grtwayfly.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gqcysxcei.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gorungxue.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gwggqoimt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gsqtdpdgc.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gqolmyqmh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gxlovcqfp.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gyredcyei.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gevyaupic.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gvksjklxf.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gxxcebvwq.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/giujdcbse.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gqexusxdl.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gpwukssic.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gpbolakxu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gnzyyjddw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gzhytolai.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gcmehqguu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gsqyginfp.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gycrhqrzt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/grlyahttn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gvwtmzmyw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/ginkgxpll.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gpfdbqigm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/ggvimayeh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/givxxsikg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gmlzijnzo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gvsyizott.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gandxyzjn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gnunizfsy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gbinfapuy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/guhktjbda.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gnyhzpsir.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gfhefgmus.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gppuvkkda.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gvuccvhpl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gvjibsrsf.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gyyssttmy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gijrchtmj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gtzkqpqgh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gyiclbepb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gtaooulns.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gseiqxtxn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gavpkkhvo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gejdyssds.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gglxkyffy.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gqzhqnxcc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/geqgtbywz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/goudfmyaq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gcvxualpz.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/glqdgniiz.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gymfylvci.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/grealgjqz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gvbighywf.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gudskqiyg.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gppyotayw.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gjwiuurtm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gzyggcwvc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gzedthrjj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gsazdgqcn.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/goyplpjof.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gxijvutyc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gsebxprre.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gghjfttvy.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/glzumgsid.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gzgskgibg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gbsextfxl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gazspwgiz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gmgmrswqy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/grivnsykt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/ggtrcwlrk.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gtktmmxfa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gnzpphqyk.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gxahimiit.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gchsskkht.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gkxhmsuph.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gsauswfzg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gncrrctcv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gemcncqyq.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gjqkftdlw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/geamqmjis.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gipaxagcs.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/giymfhdmk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gmavgfeal.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gakysspjl.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/glrhhbybj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gvneutimm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gustlrbwx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/ggfufudtr.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gdnvcpvzh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gvavtdzsz.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gedsdqwrd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gvglkbamc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gxtodlpwf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/girhimhmx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gkehdepjg.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gdvnmrnvm.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gidkqibqg.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gqqmtdydl.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gsvlxuyek.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gykhjuhhu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gtdqzxwmf.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gpaotnypt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/glzccwtki.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gmxizwdfj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gntpxocri.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/ggxgslkmp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/glerdmecx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gmibnrczs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gofsadsax.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gphshsxea.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzhashiap.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gejorinri.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/ghazgrstv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gdauhmtxj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gxpyucwep.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gfuptjdyz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gbozorjxr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gwfbkvifw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gdjpdrqhx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gdnavekak.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gxmsrsotl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gdvgmeivk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gzqrkhheu.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gvyxaklnk.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gjngtfzcm.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gepgyttab.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmktbbztd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gzokhutyh.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gsnpwvbmb.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/galgoedfm.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gijgcefht.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gitujgeuv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gjmyjdmvd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gcsjokzim.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gapkymkun.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/geawfcmgh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gsgixozfe.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gpxunzuht.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gqexsfhcl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gmjlwzyyw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gbbjrsnwm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gzefflqhl.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gajagmzjn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gmlravwzy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gpkkwczth.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gbvnqmbfz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gniwrdvhu.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gnrsiofvs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gdwophtbi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gfpgnvwdp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gojhdmnlv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gfluricqs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gmfgyvqbc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/griumnpek.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gbhmdyqfa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gvbkykoxk.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/glwqxauvz.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/ghezwojco.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gfskbunoe.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gliqqewxk.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gtjsyjjaw.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gpgcvberv.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gphpefcwv.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gvrxvbevy.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gaulqfqoe.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gelumovhx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gledrcjru.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gexmtgtrk.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gexuwkdcf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gpkzdxjpv.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gtnxawrqf.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gmazloruh.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gndvtbhss.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gcavmunpq.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/glglspzgo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gfureuksh.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/giygygygz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gltlagexn.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gbkmluqaf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gslyayikm.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/goqncgtwo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gqsgmmfex.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gfsuinljw.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gzyxouofi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gafokwxtl.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gcxrfiefs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/geaqrqbjr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gjsloobps.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gcklfwory.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gzcsanlny.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gfdueczvd.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/glpsoabcc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/graosxnwg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gdyyaoxyf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gdkvxlsgm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/geasvpjjm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gedfdfrtf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/ggtdqszpw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gtsozilhy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gdlxjebyw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gxyqcobth.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gmfaspgqk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gbornnbex.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gfucqpdvw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/grxwkfeoe.sHtML


<!-- 参考信息 -->