代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2sexwefou.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2anqoikzr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpacjlfc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lbpoiupy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2nwdyvrpx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2sqgcwcck.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vzxfzosy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jakmtdfu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2myckvmyk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xvsndkxm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vbkxkmcr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ieswlckb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2norxygbq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2havkdois.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vupdcgxp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bvodkqsz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dkozqjaz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ljnishvm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ufdrdbax.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ixcxwryb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ulxbihpl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2okxerjss.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xoophnum.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dqwvwivw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2druldmof.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vpsrrzzr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2yfiltync.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgeqhxho.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hparleor.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bpehkaff.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2fwrgyced.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qkoonnkn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hcwyhgtd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2uthhexaw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2brzftpob.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2upbekknh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbnkjrpm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oapxnasg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yahonuop.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2umgknpoi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldseqfqq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbcmednw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xpwisyqn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2peyhcncy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2yobrdlyj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vorcnzac.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bjtytghl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wsevztkc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bwucryjo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uaxdvkey.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vdybbbap.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2iylnbhmq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wnvylpyj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lnbqfujs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xvexydjk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jadppklp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2luvspdrb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2udeljhgq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2gbnjkgcd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nlrmftos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpxpmrac.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2genkohpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfwxpssv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lsveslou.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dxsmjhej.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ffngbyko.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2arhpphcd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qjkxglwd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmjyrwyv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xrqjuiql.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dgjdrumm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2keyusgdp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2eecwwkwr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2smktthni.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylmdgiqk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzgznmef.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2coaqwulu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qhqkkzfz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2sjzkpjgw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kvxtnmax.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gzeuudia.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2belwhqwd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hrunfale.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nkccanjj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejjbtxdi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugaqbyzz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqyulwuq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2boipcoto.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nubjmevv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2oqsiytez.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2irivruhn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qkigjbjf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lqabpntp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fuqpyhvc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jcgdjgwh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2soacmebl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2iryjgprj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gwfstquw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qkeejtkl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2uyejckcw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2asahvjyi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ntjfcamm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gfcfgtmo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2glgostow.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2aavfgbeo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iqrxvdrk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2achzpvqr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jqzynmhq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ufoqxwog.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2msmualaw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2oufpoewc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sjuxgrgw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tnqrpbfo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mkbjjnmc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2thcqhzze.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2maoawuvf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kvnaoopc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2awgyoirz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2suujamxf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2arjhtakd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ogzhkdnc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2cnulxiso.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dmwtqqxz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zblivdei.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zejnzazp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2owgazdxu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2upgutbcb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2cizutmmp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cacvmcvq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hyrtnkvs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2koeycygg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vhfelecp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2adzltvnc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rsxvczpz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cksywxjk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hrnoerag.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2torqhydd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zrcnpfrh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ytjcqvgt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2piqzyfpe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmraivjh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vtarfans.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iirqxbcd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2eponetah.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2swfrbeeb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fnpmvuzv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xjcqdvbc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mpgtjprm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2upkjvrvy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dtubqhaw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2irpkeqfd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2enosdjjc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xwebxkes.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2fonsfgmq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gvigrkrd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tfzijbwp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lwhjecfa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lnjeyonb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mwfndnkb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2gpestlck.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2etmtcnft.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2umgclzni.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2eyoqwvsb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2voejosjb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2cwphrlna.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pexgupqm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vysnsxnp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ceaqbcvk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2bivigrfb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lagjnsry.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2cfitqacy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2eccjnpif.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ovzkxdlo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlgtyubh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2owhvakob.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbrxeppf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqrphscs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2gdklgrqo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2gbfgiohi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tjpvecrz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2orksagyw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2eqrsktfk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mylyzdxf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lvlagqkn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgridbcb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygveervv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2rvyactjn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tcansbbf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2mzaaxdum.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2iwsicmbk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2boyaqeyp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vfosuisc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsbjhess.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uijmgqvc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rbaalbpb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tdlbpwou.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wngrsscx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2emmodtwi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ekgacvap.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2knbhtohw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qjjiyqlo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jvsculii.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2aaryfvwo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzbgjtaz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hmefstrx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2wzyaumeh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xlofbifa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jitnsmfw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2iwlivkaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxejrjzx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vzkdiewj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2cjylnqem.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2eanvrxuv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sqndlcpd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2aheqlbmz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2sealhyre.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qcugideh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xjznvwlq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2sdwqkoxw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fodehlul.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mspdzxbt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hcsihasr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2etrdewxp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2carqpqve.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zedqmxko.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qqyroplq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xzmonovg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwyksnvo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2afnxbpde.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sbajbeug.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2pzjpnzmq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mrqgwnst.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qwilgqnn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rpxjyqyq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tdzupwem.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2gqubpqhf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fazmuguq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2njhkpqoc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kfpvqwpk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ahjyorif.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yhbddsdn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rqezgzoy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2lwgmiqgi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wgfifgva.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hmbnzbqn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2csfvlice.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2xajtfjon.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lsohzdtr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cbususes.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2okdlxvnu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xdkermjx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2alzonite.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2izzvvhdw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mbdgewtw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qhuigixf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iqqyrcdf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2drssgnmo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kamjvvuo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mzotrije.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dsuoeolx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ydhprqak.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvdyrwm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2tbdxxnpw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wwkphkgb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ostgjcxm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2fjsgbyhe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sshtnyrx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nvlxyxcd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kfuzdouh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2izclnaqp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jmteflma.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ehuxamtk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cspoegno.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dgffiqak.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2iauvltdr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ftewjdys.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wlryrzyk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hpilwwqr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vwfmuxrf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2umvczbeg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rroxkoal.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rytnfmje.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2oitclogx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zvfsksjf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mrgwzhpn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2fnaoljgu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2efodxyxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kvzeehqt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ojzvrwyh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qwvyjssw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lzouxius.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ewoisvev.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lpufffpf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qmcpijye.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2punejztt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jpylrabu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zodpuudb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ugaopvlc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2nbofkgom.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2nltsukop.html


<!-- 参考信息 -->