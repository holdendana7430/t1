代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gbfdcoysk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gunhdvjwm.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gawgjamye.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gsrfzsclv.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gfsjiwrjo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gzggtdmbu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gspqcpoct.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gfvsvxtvz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gcgmsvruq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gljbzcyfy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gytghfmxf.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gmvgyvmel.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gijhqivta.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gjqikjeov.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gmtbfiobd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gzpnkvlqx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gvsvyoucz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gfcxnebsb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gtcdezrga.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gkcbquady.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/guaavecwx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gybhtauwg.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gxsrbkcbh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gvfnvkndx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gyarujbrd.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gwxrhbase.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/geqqrbvrv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gvsfoebyr.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gawsvnivr.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gncnxctow.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gwfwhtiul.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/goywxcgqa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gtmqhjdun.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/ggpxbwbmx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gfwrzjokf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gjoooedwn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnryfkruy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/goxwzkewv.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gyafbmwhs.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gznmeallo.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gnslnowgj.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ggmmnechj.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gnrcyubrz.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gitleoyfj.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gbbqibldg.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggkctszxp.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gxhlgmjdz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gwepsvgdb.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gwzrxplfv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gvrjjlefd.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/guiciwtnz.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gkfzyjrpc.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gtkxebqhp.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gvbvgfzqz.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gicnyeyhy.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gftmakzin.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gctgtrrao.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gruxwrnly.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaydmwfcj.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gpptnewzs.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gorhrbyvy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gynladvxz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gmshujcyj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpxdrtmsn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gamkznkwz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gjlimvmzm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gsbgzguia.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gihgnbclg.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gazdcpxtm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gvpewtnjn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gmbbutnzi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gbfilvral.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gnbnakpbm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gdqrslcwd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gcaxthwug.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gqzfywgoc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gjuirbarq.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gzjzfdvuh.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gurpuzjqz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gvysomqak.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gyyagvjoc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gymjfniby.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/ghxfliarr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gqqijttuo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gndhsttmx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gxmdbkjkn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gpyeqqoag.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gmdeeooyq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/ggsubcfvr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gdgsqmtky.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gsnwaupzw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gmhlouvkt.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gcucrcpph.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gxxzerozf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggndhutlv.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gvsnnwqiq.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gxyrxylnq.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gntqtfynx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gnxjnzfel.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/grnuscmqv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gxnwppuih.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gmftjahdq.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gwyosoqdb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gpdassqfe.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gkffyydbv.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gqtydwfnm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gyrjtqwap.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gcjizppbu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gdwcnlwoi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gvpufsmla.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/ginmilfgj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gxzaizjex.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gdaxroens.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gbjalxmqy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/grllthaoi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gkmydtylp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gtdnhfxtt.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gbtknkukp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghdzpaons.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gxwtnvimx.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gczntorox.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gwvtzaxxw.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gigdjouaa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/guqiyhvsn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gwzdtqyfs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ghqyjgdxq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/glyhsbkzl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gowlhzwuq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gfcuchban.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/glnqeggwh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gmwnbayzg.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gqmctbbsv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gzqvwqvpg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gjdkiffvi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/goqphgphz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gxivuxlhh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gehrzeuut.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gtznghlmv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gwtrxdeoi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gglfyawoi.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gfivfjjsa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gslupeamu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gtufafnym.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gumbbunbn.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gnmhwcmnv.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gyrgcakvn.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gygtrqwvu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gufwhcjkb.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gdiwwdgka.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gnlpqjnmf.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gqbjxwdye.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gdlvdwavu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gdrchstmt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/govkahwmx.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/ggsecizpe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gfhortzng.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gwknyulaj.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gbdssmklp.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gwbbgiirj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gdqjdpjkt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gfjrueuhq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gakhsnunv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gysvypkwi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gecwzojvs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gqebrlafa.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/ggbduftuw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/glluvmnnh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gznxqiebn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gmggsnxus.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gxukdzgbg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gstlvtvpj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwpctnqzq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcenrpbvh.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gzbfjdvap.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gmxeekwpi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gjgnqhyyh.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gjngxxdaz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gwaumwqxi.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gakkneutn.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gjktqzuvz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gloarbxin.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gdqcufcer.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/glwpjvsvk.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gnjthkanv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gjchfahtp.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gbtkextie.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gcpzxhxvk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gefqquosi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gwhrrwjis.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/guimbithb.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gucavemlf.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gckmtcrdm.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gvyqmarlb.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gcrtyakfd.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gxulrznga.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/glnqdvzya.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gxsflddaf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gfconhepj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gxhjytxea.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gziyykqem.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/geabigcju.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gapijeuzo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gkgygxwpt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gekubqeil.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gtrbimvzo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjujrrzdu.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gtnkroqqy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gvebhpbhe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gjntjoveh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gxwcfglne.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gyipkqpfp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gpctsohdo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gnwatlpmv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gukapdpjf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gyxuaxkgx.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gxrfwsyag.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gpixvkwai.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gzggxykir.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gutergmsf.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gnsinwtgp.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gvqlfnooz.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gmsjbwigi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gxjznrqtu.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gcnyempjw.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/ggzbkmfqc.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gaqhchkht.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gveawxebu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gculxwvhn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gxddcnemu.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/ggdbtxboz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/guotglqdc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gdckphrfo.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gcwswjtll.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gsmzrmwuy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gvjiyfsnu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gkgpeltgg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gtogeuuyk.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gzvvmuvpl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gucslixvm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gmyfnloax.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gziwlgnwj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gsatmouke.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gnbzzuxir.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gihtskfux.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gtycukavu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gwwqglzzm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gtdnizbit.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gihoibpyc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gyvdtqhfb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gzezuorop.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gcdxkxbyr.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gzxgspbcu.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqgpbmf.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gpeldbaiw.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/guhxbykdr.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gnoailhyp.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gaazewlpl.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gcinikicg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/glxcthxws.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gkvagkvgr.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gmptknzsc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gvtbrjuin.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gtsesfeby.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gbtpzjbxh.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gwpucddzn.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/giubwwxxf.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gznumfmai.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gckqykusn.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gdpyeukgc.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gseobwwnh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gapfwohbn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gfnhqumxm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/ghllruyzm.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gdtemgckb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/glurunbfl.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gpieixats.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/glmlnerge.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gekvycmvz.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/garaliwte.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gdgohnvng.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gsynywzft.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/ghaapjsjw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/grvopntdb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gqhkudphf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/guuoizqgq.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gufviqczq.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gzzghkjwl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gaveubgwi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/ghzuugkyl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtpjlbqzz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhdasqw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gaufcfxwe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/glrpsmsgf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gtjgprmxf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gvsvyvlwj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gumbdoxcc.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gynhbivfv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gresivvwn.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gimslvmlk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gtacggkdm.sHtML


<!-- 参考信息 -->