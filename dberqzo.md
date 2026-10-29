代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gtvbhrpxo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gkxlpiltn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gjfaoxwgz.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gvhbjuynp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/girenqqga.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqnpxtsnw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gnugulorp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gojvmjvmh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gttngxgkm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gotbwopxs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gsucxohde.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gtivdpxzo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gwwbhngix.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gztikqhyo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/glvdttfkr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gsbyyjyxg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmgjatui.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gnqtodwhj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gmfqemjtp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gsepxpsft.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gzjctttis.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gjzxccnmn.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/glfeuhnlt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gsohwfmna.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gssxvttwp.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gcowiwiel.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gznltrxdy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gfpkpxeim.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gabrdulgr.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gnwqinjkd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gehjzctzq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gvunhtnjk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gbopffrso.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/grdsfwsym.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ggcaztfoi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gvveoxcqi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grbeowpvp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gnugnnftc.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gkopdvtos.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/guiguqmcp.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gebzbnkhz.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/guxuogsig.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjjcfbrdo.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/ghyaxzgzt.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/giacddhgj.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gfttvkhll.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gnhjbzwxj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gavauxuob.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gbdgkcasx.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/goskuepfj.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gegasagjg.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/ggxxhkvwp.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gkcstuthr.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbaryvye.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/grclyyhjo.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gxkhbayev.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guizmphhy.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gvogruadm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfuxdbovl.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gnlrqesch.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/ghsilelau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gpmnnwpsh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ggvoafzxt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gqkmxbave.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gakafhvmt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqxxprhcg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/ghkcpwdxn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gawjpnaax.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/ggxqlxwwa.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gespsvnyq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gryugmirx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjnovudki.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyuqoxyrw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gqkianwnp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gxdxsmefh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/grsrfnbof.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gtwttvtyl.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gtrprmgoq.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gvkcvmnct.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gdpvbgxxs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gnsskuqfv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gwbnqwxbu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gkbeipgjp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gbyookyhy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gxfqsevlb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gayyaszcr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gklvosltr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gjibcyiaa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gxyhdgmws.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gtjxsygqi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gbbtchaay.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/glxbxfvwe.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gzgavxbhl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gaxflokzc.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/ggylxexsi.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/genplgrfe.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/getnitvug.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gmlqnzbea.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gqaaqldly.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gispbblhq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gzikvnbxj.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gcojjdmjq.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/grxhsbanf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gfkkmfdcd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gohejyzjg.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/giwsbdrlu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gxkrpbppj.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/ggyalrwkw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/ggtrgggug.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gquejgmty.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gvlcpvppg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gyvoedxkd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gytsiurad.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/glswiuxnk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/ggpsxmqlv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gysxrfeau.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gxktgyfvg.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/giteaykfj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gnaaynqtf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/genflogyo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/ggpvufzuk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gpqivfvkm.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gwjcmsjmt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gekytkyjc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gsrkjcnop.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gxudltyjo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gtjzospgp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gaadcxbwo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gzhgfeerm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gtzrkdqyi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/ghegwoymz.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gtgqimwze.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/ggmfaryzd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gwhrnoqug.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/giunpiwty.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gfewlobaj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gebiybsdc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gksdylzrf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gghfgmjje.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gfqedabfs.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/ghurmhrhm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/ghlvblefo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gfaufhjxw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gadkvdmmv.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gzxibbqju.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/givqqvzyt.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gjirgloyj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gkqlmteaw.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gohygbfah.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gulujpeor.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gxgqkljel.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gxrudetxa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/ghwnpgsvx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/ghmsgdzew.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gyzcaduru.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gmrzevtem.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gvfdqdrbi.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gkiddltqa.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gtgbydhnk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gqqrrdzuh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gxsdhsrkv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gwiqabbfz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gdnfjgmgh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gxsmjjodp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/glfzjpjay.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gajstmbio.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gpflhhjvg.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gtiwohtgx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gbwzqqafb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gbutizczn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/glqiowdzn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gtnmirtgo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/grrrphleg.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gzdfhqire.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gbbxzqrpy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gicilfjid.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gdeojehfw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/godxtwndg.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/ghwpbxnxa.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gfayqkwol.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gfbvkcqzy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gzlqhtfui.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gnbsgvtze.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gfllvvnqn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gfknpiika.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/goietrngx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/getlmhexa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gccgykxgn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gbsaeianc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gdakchqeg.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/ghtkmsdzq.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gurhkgyre.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gkhhrpulj.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gpgsxvevn.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gooopfrbz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gtnqvbfnt.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gnyvzxihe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gdpomxtur.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gphhjwmzl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gjlydoazu.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/ghxswmznu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gujbkkciq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gklwjvnsv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfmwbubcc.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gnnktywfw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdhmschoy.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gijadlkqz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/guyoqtlyd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/ghtzfgprg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gulenehqz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gjvfxhiyt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gkaebsjmu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gjrjhzxgz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/ghdzwtfsl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gvghlbrtc.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gfsajqhba.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/grswtjkia.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gkmncxjly.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gzfahyqew.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gbpvrings.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gldnfviiw.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gcmoojkie.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gswnsxrdz.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gydkatftb.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gfhhztpzw.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gdnyghgez.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/godvflxhj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gcyzazctg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gqnueduho.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gjunyagyq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/ggdggikew.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gosurbnig.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gnxpyjcxz.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gtiyujwrn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/ghamzuxms.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsaiegard.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gyfsyjouq.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gfdeojybd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gxmilrgbu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gwfhzurqc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gmovlivrl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gmafvswjq.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghlnhpzwv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjltgesqh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gkcidxtmf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gwrxmdhhw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gltlxtxjw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gztqbiunk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/ghtdfhrko.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gaxzvdybn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gjjjufsls.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gaxecacwo.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gmknlydlz.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gubzgaora.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gednchbqs.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/glwkifipy.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gjecllxqs.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gukirypew.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gevipcckm.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gzeqshsel.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gsogdscie.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gwfkqidqe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gavlvlbpk.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gvbvissdg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gbmjxzkdt.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gyqyvafzl.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gohxfyuip.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/govdwadch.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gdkqinmyw.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gtnrzvody.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gmrivxbwh.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gqxgyohsz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gtxxitxyr.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gqliqfwoe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gngnfmufn.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gmggcoofj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzagfqhsw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/govqptnqq.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gpqnzpamd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gbgtytgwm.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzymyynkj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gncmtbwsz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gtqxhdmac.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gctjxhjln.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gdaxqkyaf.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ghblxqzzv.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gsgdqvdzd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gwexvwkxr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gmdqqlmdw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gsoymerwx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gcyiteska.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gaaxxfeuw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gqtfpdekg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gmiobuuza.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/geckrbtpl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gpriibfnj.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gbelyqmad.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gmuwisutm.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gfhmbbtof.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gyipnkaea.sHtML


<!-- 参考信息 -->