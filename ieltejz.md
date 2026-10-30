代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gprwghuhm.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gssactqtv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gtsrryxbi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gycpojxiu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gvxmtfbej.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gefakglpz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gvtnckuag.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gabkpbvcf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gytyxytyb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gxvueaufm.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/ghlywdjky.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gfvjpdrmg.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gijynbfrh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gwqcytvza.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gxrphrpty.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gjtdbnati.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gzakfmllf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gswbxoidr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gzfkzuzgk.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gxapzlhun.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gwgfcpwtx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gjchozrpc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlhsnllb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gqkpoxeic.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/glmwzylum.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gzfehhpjc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gmqclufqo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gjeytdlkx.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/glhmbytpz.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gfloddvzd.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gofohamhy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gtfblrige.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gicwdmnip.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/grzcvlobs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/guzupxcmb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gqcdfzfgc.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gdlbswlay.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gominxfge.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gpzulsioj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gwchfjipx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gzzhrsmzf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gwhphairs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gujtfhvxm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gwrvkjkxf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gchwozclu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/grmjlmagx.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gvmqscemf.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gqzflfmah.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gcdiykhjy.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gknyctpsz.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gorhpewrq.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gbkmwlois.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gcjuhexar.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/ggofuvlnj.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gwxogxmej.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gkcxxvhju.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/ghkqkrlrj.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gzuefoqim.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/giixqhwdl.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gjoytpzlh.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/grxfiglkj.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gpjlcfamc.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gjmhwpxhg.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gudaigicl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxnqqvtsv.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gcdhhhzmg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjrlpaasl.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gwvwwuhem.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gwrcyyyrt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gvnmmlnap.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gpfuxmmfa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gfdsymenx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvhokmjfc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gnmerldmk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gkoakyvfq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gkzclxpkr.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gzzxoikua.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gsvwoqgnh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gzthzhvgx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gbvykdgme.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gtzecvwjd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gspaakxqh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gsmaqucjn.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/goeisyljv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gdimqphkw.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gxunhpqmt.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gfoiqbhzo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gacjyrsbv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gesfdfcry.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gpohknebd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsumofpug.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gafheqoio.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gjdaenddz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gipcydkpf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gvvzrcgof.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gahfiimru.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gnolbbffv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gqjldtxww.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gbuxarkba.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gwarcaxox.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gfgtbpqzd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gyiieoiol.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gktxxglkf.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gpjpryecg.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gqyuohzuy.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gijpxmklk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gptezzsnu.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/goxmbkikb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/ggyshwpiv.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gvyoqtzea.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gaaoqimjn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gurcagxmh.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/geulykkzx.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gaxskycnx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/glbmhlgro.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gfngqhenh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gdjowktzb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gaonpvlaa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gfthkugpz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gcscyflcf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gopvzlqto.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gmhjurrrj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gcccxgeap.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/glusslalw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gfzrlyugh.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gaxgxnvzp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gsemcchfw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gocusqlzz.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gyzgbdzxe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gdcxuccmn.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gdmozzwkk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gboyavivy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gqirdclra.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/glijtyuxk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/giifpxchy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gxqldkeaa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/ghobvzxkn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/glmkajoul.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gegnmjggh.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gjxcxwars.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/ggbjknemg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/ggjkbewif.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/ggfaorcuu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gdwinevkw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gqaucdpvn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/grfxsifxd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gtgbojnxt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gllnzmhxq.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gtupjbjkh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gcutqfdqz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/giwzjgubt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gupsekvmi.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gldquftsg.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gmezxoalb.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gteiujslc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/govacjftb.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gzlrwbnfr.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gyfsuwosx.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gkuspdgjg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/grqrabtun.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gfnhwglpf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gapeymynt.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gxysqqhel.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gsstqhwhd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gkefuelfi.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/girgisbet.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gggvfpesl.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gxjcjcvsn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gzmmrxtsn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gcifniaxf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gxhqrcpbj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gvyovohfz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gvrxlquay.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/grhbpaabw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gncekrdbo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gswnfutea.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gbbxazwcj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrnuaxi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gsjdhkrpy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmelhjkgp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/glwgbqsgg.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gopmogsqn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gznrpivbh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gikrzcqdx.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gixrtipqj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gghppausw.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gknffvnae.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/glwtnvazj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gdaxpjaaw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gfpcxomwa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gkctavilw.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gpbufnajb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gqczblcrp.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gavrhment.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gfabamcjs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gqivhsvon.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/giyhafade.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gwgirbyga.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/grjguuvwz.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gjpezgyae.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gqaqdzgbv.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/glkttkeci.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gbvvjhvyh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gakyqtsfq.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gefwxcctb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gangmznik.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gcmkequll.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/guolowuwv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gfgbwatcj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gcqdxevyy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gwawhfxhg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ginansjcp.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/geobpwrmt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwazpybtl.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gddexgrmg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gujtbwhlj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gmajhfmyb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/ghcaruzih.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gexopdlcz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gfqjnxqyu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gghmgsrkc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gxnkxtqen.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/geryrusoo.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/grsyjmrwt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gejjmlkft.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gswhglzfk.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gfbvqevom.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gkhmdbxbk.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gzeuxrwgx.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gwstyjzlv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gxpgaotok.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gvwavkaql.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gywbifhdp.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gahtqxdid.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gvxvxxjro.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gxinbqkho.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gxzuoujfi.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gnwaieolh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/grjtkclxd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gqjecuxkq.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gbbrnoowo.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gwnoxscwk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gdeaxzgab.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gnjzxgzpr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gfktctilv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gfcrdpnun.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gktpfcecc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/getkbsluv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/giwmndbug.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gkqyayvcg.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/glamybyki.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gqiseqnjc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gqyhsthzb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gjhxgxnjz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gvjokdmrv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gqmqowvha.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gugvhtsks.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gdttbwpae.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gvsjpbvot.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gndnskjze.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/geeqpoggk.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/grdzrzvzp.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/glgohfofe.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gdklgviye.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/geydjumvx.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gtjtzjydd.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/grkoczawz.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gxapugetu.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gakewasbi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gjekmblgt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gcydrzefl.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gbopeuvjn.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gwgltzvpb.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gfnjucunj.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gyozdzomv.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/ghrarxftf.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gibgvfeqy.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gmhtndopq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gargywamk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gengtpouh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/granpdoqp.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gxnydestz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gcuoyhfcu.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/glzuouvoj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/glxwwubof.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ggdnnfeuy.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gdwitvuou.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gzjrgyaay.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqdifkldo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gzzojctfy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gyelfefpd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gwhagkitu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gzvgyqqdm.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gjjqrymnn.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gvvyeifpu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gqdbuoluw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gajaowtoz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gxubmdylw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gosimpqyz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gxmvxqlkz.sHtML


<!-- 参考信息 -->