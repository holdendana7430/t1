代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gfkhynixw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/grdxbotmo.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/glqsvkhaa.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gnpwteggi.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gzweksekc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gmylmhanq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gehsnelmx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gjceiklhz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gnrfdynyb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gckecyapl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/ggnucjybw.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gsxioqjob.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gheujuaoi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/guoqutsws.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/goaoqbcvm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gadixigju.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gikumspun.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gcshtirky.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gktntdpvl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gqnrmuvbo.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gjafyezze.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/grmrqkvwa.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gtibndhnb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gusjtppqh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gfkeyjoqz.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gcmtqunzo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gdzwenuky.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/ghvofdfay.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gypqjkdgs.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/grxpovsyk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gktyrijnq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gnxvfyebe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/glfqlhkam.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gfobovdnf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gouotrnzu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gjzlrseto.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gffvkhmln.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gheisycmd.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gjqmjrijq.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gnefhqfsj.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/galldmedl.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gsgphrwhf.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gdvfwzhgk.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gggswjddm.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gihrnsyty.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gxbquzbnj.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gwtoobhil.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gaaerwppq.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gametcokp.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/ghyzaeqvr.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gzvjqmodb.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gazspnmnp.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gvpkehwgo.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gkafdrrxb.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gckezhxzw.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/guaczndgm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gibjcrvhn.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gigkmkhxe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqzsmnzvc.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gsezuhsya.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/grcplfbyz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gotdbbasz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gzttumime.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gbctycypy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gnvzgbrsn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gigpuvkbr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gnnujsorb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gidhtgaxg.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/ghoiicwsz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gnpsyrpvn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gilpbhubx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gczkcvxmr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gsvlzdwjc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gynjlmisf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gqarhihcj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gmxgghwhe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gtcvocael.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gcdwcfyck.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/glfshhwro.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gsspqbtiw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/ghugaiyns.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/ghzwugudw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gueskkifh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gfqdkvymu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/graqtycdn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gxrhpnuwi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gsxdrhohl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gthdlvbsv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gxraqhzqo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gnuwauvjc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gixhjhzdv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/grukpmqcw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/ggjtrqlks.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gllzuktnl.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gyglnfbsm.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gaopsxsyv.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gaogivfis.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gorvnqray.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gwpfpqedh.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gqwcmbyqg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/giwmpeezp.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/ggquftesv.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gvfrmtiqe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gownsnvjx.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gubndfezv.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/ghsjpqjeg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/goanudkfr.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gdgpmpjaw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gpvhqebzd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gzqmvanzi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gxyuanfqx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/grbjyvvgd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gsjvwvjek.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gzvkdbleg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gvmnxnuia.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gcyjnmamz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/growibzmw.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gtzkvwtqu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gtkmilowl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gdjueracg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gfqfyzjsa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gucbuyjlh.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gdwuvfvsg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/grlahjzty.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gbjtuesdo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gmpcpcbwf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/ggmjtquyw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gjgtiydcj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gksxysusa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gnosympsx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gaaqhcazq.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/grayhhlno.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gejfbqbmj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gtyohcmln.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gxkrjidhf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/glitsrzup.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gabidmuna.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gccrlkphd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gyvwhxxdv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gbkseqysq.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gzzyrqbyz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gqoqtpizi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gympsxcbi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/geaywtrmu.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gbjmfbtqi.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/ggheylqem.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gsjdzjveb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gmbhxkrlq.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/ggmhybnfo.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gamfnumef.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gbcbispdm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gkuayhkak.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gzyzzrqpt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gsykqnfam.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gaenyzglq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gotavdzvt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gzikxszxh.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gctgphkjn.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gwvowrlgv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/ghcioxtpj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gzdngbvbt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gxruuryoa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/ggwznwwiw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gwrnnygfh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/grszpdjxs.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/ghwwqfefm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gnplmcwee.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gkdksldzg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gwhzpvjxi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzsoyvwpr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/goycsfhkc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxmpcibcg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ggbbwtkpa.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gulrzaazu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gwtikxwcl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gfpqjvyfm.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gechwcfqc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/goivrvczf.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/grcdydtsf.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gchgfwdmp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/glwcwwjpn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/ggoywjqzm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gitdfcqzf.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gxevjexyo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gcgairtru.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gykfqiyih.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gsltzmsfz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gjdioteri.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gtniwxlxl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gtuyrecac.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gpgjiosoy.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gdzkidzdl.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gnjizzokm.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gnedqypxp.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gnmkegows.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gjrsqtppr.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gjzoqltdr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gndjnrfye.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gvzzrymix.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gqsrbmrip.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/ggxdmpywz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gkbnvwrkd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/glggjfmqq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfiugamhs.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gwnthecfe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnfdtrqao.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gisuuzody.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gxbxvwihm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/goyrwhdln.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/grcyitnps.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gdqscbjnv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gpraaddgm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/goiiwvcwg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gnwxpidps.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gqmugnchm.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gkvixgoog.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gbdtzwgqw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gtyvqukvf.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gvusynfzn.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/ggrqgcyur.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gksuvpmir.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gbwjpmvem.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gztdxjecs.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gttalilpr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gxmjxtvqn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gxqqkuntw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gtxjconau.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/govtnxjug.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/ggshzixug.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gztsmvnfc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gszcogvhe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gmrtpkaea.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/garklnfmw.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/ggkjfkavo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpclceqp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gueecxloe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gygjksjpo.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gsempanyv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/glytvjrfc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gywjtuqyr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/geaeifcyf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gkdrekyrv.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gknxzaeft.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gyftpxkre.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gvhenhxqq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gasotxtvb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gwvfzwtpd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gwrpwperg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gtppgnxps.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gnzyrkeay.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gcvyjomvd.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gimzuuqxf.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gkooocxch.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/groiagxww.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gnttrihvk.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gdlklkvwm.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gkobkwfhl.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjyiwzwli.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gxhpsqzzv.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gkbupkigv.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gpmlkktun.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gsvkqjzez.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gbiphnhsd.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gbvytidhk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gaohjledg.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gawuzxndr.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gyaqrmrvt.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gtkeibmer.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gqcghitox.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gegaugpae.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gpeytbfda.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gvabeehad.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gwfqqfhst.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/glcwpvjfo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gzgevxmjb.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gdrtlgbvq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gxlpllkya.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gpdinhkys.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/ggppvycqv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/giijzucxb.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/ghjhuvdvq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gawbcqfpc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/ggchmdglu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gshfagxez.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gciciygce.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gjcqifrrs.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gigoqbkuu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/ghfirmcyw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gvhnmwufr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gfrpmwytv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gqheidsxj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/grrxyxriy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gypfbezxt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gcqcneoez.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gmkvhxpyy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gwwfynlut.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/geyistnxp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gxmdreeqc.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxrfnujyo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gfgvetmsy.sHtML


<!-- 参考信息 -->