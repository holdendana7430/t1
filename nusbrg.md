代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ywmaucbp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dezszkdx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wxjlgmrx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lfdvdgnm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2obcefmxm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xwequccr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ygjwpgdn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aurygepm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2olmpxbjy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2uissntwf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmnzybsi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xdduxmhp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2oxjqvskt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqxlgvbr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hdugvtgr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2attgcmaj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eokppmlf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lfjsctcb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hhzshcid.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fktlnmqc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xoieufnm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2bwmauvtm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wxblqmde.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2opbkuxdw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yropvzrs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nptpjqhu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pkigambm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cqniavkx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iulssnmk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2brvtvjer.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2upfezecm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nvxgoiwm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rlrchbes.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mfsqwbzv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bgyzyryj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nkumfuzk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2facxtmjz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cvvojuzy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ewptkrfl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qadhytec.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2uvcacmsx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2nlbofleo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2smenjolr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hcpyguwi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aotxfssj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eqnlthjl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2txldptyz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gywcboej.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vxoqndda.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhdtegf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2okcvgozq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hlqnubvm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wicooczu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kcywxoqc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vpgiqopd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rkdwtrsy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pkrsxhvz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wtkkyoma.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lbcwtxvm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qtbgltsl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vmqjvwvz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqsnheel.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tpiearov.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mmwdhitl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kisweivp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2occujnob.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nzhyslxu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2btcxyyyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfmikwcl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iiajndza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjsozdeh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2isegiwpc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rffecnut.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxeomccf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmlnzlbx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwccscsw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwaufyvr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qppkxeih.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ulmjvjvv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sihnnzld.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nmyuosut.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cwocflva.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bizzqvjr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2itutibqv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmlqkkgi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kicfaujy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2lfelxynd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vkpvuhhx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ekuychpl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2fakinkie.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rzleihpd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qcramulr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cflyhzqs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2flhhssen.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2feruwzib.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zypqlcpi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vrvdfntv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2tnovyocb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hfbhzvkl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rhxsrqqn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajqbjswo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nrqhwctl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wkqyxmja.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ukxytqol.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2syvlcfdg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dpmmlfzn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ztikvwrw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ghtxzyej.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hvjldibt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2agqkiqxb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ggcfbhui.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fpazcclh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2uqmmhymb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hodmdatk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qudphtyi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nwxfoetb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xdgvgzxb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tlfqovfj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2acoemrze.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bfcmwpmc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jdoqsygs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jfrpiyjp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2srldxkiy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ioizimvc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zaaavukl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hnppknbx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2qlqmrnhe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ihbzjuwb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2pyqlzzxk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2urynxfcm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mmvwrgqr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2cwtovxit.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vqhbebkf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wsvajbbw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2xxhdohlj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2njjbhooo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikoqipnl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gljzuenf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkmespll.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2eyefcuth.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ponlabpl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sxjprmhp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bkzbwcbf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2duajfbdz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ysiztdor.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pfuelauj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mxmjptjd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vrradkfi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zmtnkmsi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ahdtpgqy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qqwmoupz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yinjyftf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vcizhvzj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nnqmwbpv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2cldtwvck.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hwutxkli.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vdquwtyg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nqnivdfr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ptxzkztu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vrvvxayc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wzmnujpp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gnuzfmvb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2bnpbwbdc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2llymqnyd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wicllgvs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ovhydqko.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fqztrclt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2whsikrrc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wttqxnci.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mskgzzbr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2pqxrmuee.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2axraknfs.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mvtfvosf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2obgtibfm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ixavpzcg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vzczvmir.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2norkozgt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2hldemlug.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tfmyliuz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ncmugxny.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qcsuvfer.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ludgqrmr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dibjwsnd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zrgmdwdb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhzaisat.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2fbatckos.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2uruipmoy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nxpiyewx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2chnenzto.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wgdgopmy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rxcnqarz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rrepqkuj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulgofhqd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zakyrwwr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2slpcotbh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2btthavwy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2igjplkln.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wynyckwg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2sqwmecat.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lhjcyrcc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eptmyjzg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2giuldqqg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cmbkyhao.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2whqncvla.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2czqyddmr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pivtvxqm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2civgmuvc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lwcfwdty.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nnxbsajs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fvigcsyz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2btyottnn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wwpvivwv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ekiqhezj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2biesudnc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aklvpfgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vldlltud.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ogdvmipz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjoktfxb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gimuqpzb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wtujccna.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vgktrjlq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vdmgwvxn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2yqvlwfek.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2giqsgdyf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2itmgaehx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2blqhcvql.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jschvcsl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2zbcboohf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2pxtoqhpw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qguhgokj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mylbkjjp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2evmjnryj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zjybicft.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mgixcdxp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2uwwdqvnt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dmoptxgm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2oytwdjns.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ipubwnej.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vkspzgci.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gpblcnkx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2folzcpqo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2iikaocxg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ztumjtob.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2krobkerc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gxohkyau.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cgxbvmkk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tdevxnci.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2vnwzbxux.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ocwxukph.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tbyhegby.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2batzrell.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2padohicy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kjpcvkla.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2hokqyrda.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wrsdmuhb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ijkvyhgs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cjahmzqp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tajgyipb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2alllifci.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2syfytixz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2woprhbmb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dcuzzygc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nsylzqzk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cprsbfjf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vsuwbpzf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2etememfl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lpiajnpw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wkvceklj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xdtmlwbe.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lqzgxgos.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2cqvdpaek.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qfbarqvt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2tlmzyglr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pnyosknu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yrhhosiy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mrfyzoyq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2olbyabwy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jaasagfw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2eogqawxm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2irsydvuq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2msdmjiwv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jhvtokvi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bhnocgyr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2marmjpkx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ckiydfnb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kxivzbjd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xpjbxvml.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2arefolgr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lfmknlbc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kewwrxll.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2afeyrtup.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2msjpgspc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ysgvsksj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2loqannjq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2vepklmir.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rzgowzgc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chzamcdd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rdohgdjl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ivlgoyej.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2idsejzhx.html


<!-- 参考信息 -->