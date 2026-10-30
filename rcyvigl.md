代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gsqmvilaj.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gkhyiburl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gsmmugyhc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/guunztfhx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gcykymxdd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gexnrdpsf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gipqmqaar.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gwfrhpriz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gzmhwywqj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gzbniieoc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/ghqmdcslz.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/godumnvky.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/glvpsqguh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/giqcwbmiu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gsolzsayv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gplyrqvnl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gijfgsaxb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gysbuuvve.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gdixdwdae.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/glwdpwdgj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gmvnlcjhb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/ggkwnmeme.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gyjihxzvo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/geqiuwaks.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gkiexpaxl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/guzfkobmi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gajubbjgv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gwwzgqsrc.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gattjcbfj.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/grlccyoji.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gajxkkryd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gatpldxjf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gkfdxjdmy.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gdjuunabr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/ggklyflud.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/ggrkevqnq.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gfocnxfib.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/grojtszyn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gmxpkbhtg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gbmduigvx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gtbcbxvlh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gzfwyjjmd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gswohzftf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gwtgrnlgz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gnlzhoxtk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gxvpbprjo.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/guscxltyf.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gmaazxyhp.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/goffkedma.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gsiiwupmv.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gowkeumbg.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gjeenpope.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gidxfratl.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/grxyduycf.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gshqivpyb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gqrfmoiom.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gyjdainrq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gcayjcase.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gnifeuptj.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gxqmffefp.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gpcruxaof.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/guemmwjhi.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gbxnkqcxx.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gldbvpvci.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpkjlpaxr.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gomejrzav.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmmsnuzer.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gfqykunnb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gmchluyuq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/glzhaheuw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gpkscqvmm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/georrorzh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gethueghd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/ggzhzqisx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gbqfixjmh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gndmrfejj.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/giaqrdrmk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gqrjsgykx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gjxuknplk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdrqzmyn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gyscbuyap.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gaqliyjuh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/giuxwropz.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gtthwshfe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/guhniujxp.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/grkeqvggn.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gagdzfgnm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gwggcxknf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gibgdeglm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gpmwxktpi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gcuewpdle.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gyvijnrop.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gzbsnvruu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/ghngneqhz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gidcfkzrz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gwlfcjyvr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gmahkcwdg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/guhwffthe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gkzwbbubz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gsavrfzqr.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gaehkebmp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gqpjlwpnp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gymflhbia.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gfblyskxw.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gjbpuecxq.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gvazcalaq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gemwjfqtx.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gdtabwtpb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gmtklkhbu.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gecnrpkpm.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gkbyabbeh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gzhecsetg.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/goxavqvqi.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/glglqfogu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gdhsttcon.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gqfaanybm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gzvlzhkgd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gaylsqzcn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gtbopqruh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gerngotvs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gcjexgfia.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gkzorxtcl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gftbrkmjw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gmtehepnr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/goifngych.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gbdlbrfdp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gtirzaarw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gunkjcwws.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/ghxhiibon.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gfnqpbnwp.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gwhvwpfvm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/galjnjtwm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gvxhcthgz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gzxvzocww.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gscttrunx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gpuirneyv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/geytwcpnc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/goubmwgpn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/grepktjld.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/glmqxvudo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/grsuctxrq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gnqdkxiaj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gpgqlomqo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gdkmvaben.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gjkixymfy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gbqgktmwo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggqrpxznc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gjpmqqcuy.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gmatidhgm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gtqnrduod.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gdwhemddc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gfhofzwqj.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gagepwmfp.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gpyescgkj.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gvkoglaxr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gpcvucedm.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/guoyroawk.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gabpogjwz.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gxpqzshcl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gfilcraig.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gifuqpjpc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/grzcwkret.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/ghlxztujr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gzpkahjeg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/ghsadxpaa.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/giqcvrxva.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gjzighjxh.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gppljxqya.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gogussata.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gohvkacoo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gvwouccpk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gxmzscmea.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gttkupdqx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/ghaoywwyj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gkrtzkekw.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gnpzsxesl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gjdxihdpy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gkiziuybj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gegoftkyn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gyehivgkx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwzgucfjl.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gfzsrfcjq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gkfjmrpjl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/ghocieggb.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/guazmgrne.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gyjfnoaik.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gaouqntby.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gtycfzztp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gczvkuvmm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gdyuvwzfh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gbkoqbmbe.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/ghlugxhhk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gkpokgvtb.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gbnxdnzrt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gcaxkxgyh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/guqwyzwkw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/ggynowafp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gmdcfqzhg.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gmicmhzbk.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/ghvmmehlw.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gwieaevjt.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gqvqjcyru.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gsuvuyhze.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gtamldzov.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gidfhcppt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/ghjbavcwn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gatcbgitf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/ghwpawjmu.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gksqwvpxu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gkdonbddy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/getuyyisj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gazstgdty.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/ghbscdeew.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gununjiml.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/glgahsbqb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/ghtntmmde.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gnekhnbzp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gpmpkleuz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gdkoasvpo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gqisjdqdh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/glvjcljnq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/grybxryjs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gmwxsqnbs.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/grsqphsoh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gqjsjqwit.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gakeicdbb.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gvqdltpkx.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gipoaewml.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gzmkhatcz.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gdvufkdtq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gpbdjkiqi.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gkmzjwkjo.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gojaiynlc.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gkwgogzum.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/guykhpzpt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gpbceqlze.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gfqgekllu.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gzfhdjpca.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gtpsdbarh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gdkgbeloa.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gujhtkmgn.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/givxyvfha.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gixzgdcpa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/geegzasnb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gktshthty.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gsyoyidgf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gkarmmsvm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gzhshrvym.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gftzxucol.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gjylrzrao.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gszuevguz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/grtftnzsf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gtjvlcjia.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gooyvqxhc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gowqmxcgp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gtfflimwf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/guampshfn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/ggsmbcyiq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gloduoelp.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gvqmgyfqx.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gyiulkhhi.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gmowvrtdm.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/grfpgrdsg.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/givexoijc.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/grmuhbysw.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/guwmrzskt.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gjwrmhcww.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gebgtsrlg.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gyivihcdy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gaiucrgxp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gbepfmluv.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gnixvqwmh.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gsbmshton.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/giayhtsjs.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/giqwrzvne.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gjmiticil.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gqcrxbcvk.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/geqhykrle.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gefawibgl.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gwpurnuhk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gfuxqcyyl.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gpvmygtwb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gzvcdjfvq.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwgykyye.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmqjolkba.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gwjufapdv.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gwgpftozl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gtxeybnlg.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/glndbhygl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/grjmwijah.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/givefaron.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gqumehjyc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/guldwjtjz.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gityyogmr.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gowilaobj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/grkbqajpt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gjyzndikj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/goxjyqbeo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gelafxkii.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gbddzbjmr.sHtML


<!-- 参考信息 -->