代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2svnuphpv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ggfbrymf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjhoyias.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiserocc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgxauspk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2whjayyky.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tbgkkfmd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2bksewhvh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hetjaklc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pbuuslbm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ukrzzpll.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcqymmaw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gbkbsnml.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jkpaoyad.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zsiqbfcw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vlafqkuv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yorkrazl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvwdkrow.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rccrljrg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rrarusdg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gcjipgbu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kxnjlrno.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ltkditnr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bzrgqihv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lgtqtmqi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2izgnmmos.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eaizmlwe.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2iqjwhfni.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2nczfaqot.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2smantxqf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ogyhpfsj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dpfozihc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qnnwxvkl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcqgogmx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pnogagpc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2odipdrqn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2gsyofktk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2caingzrp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mznsnmtr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kytnwmwd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhuuceqb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kaksfrzd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2whoetool.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hzfqwkow.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ztsvueju.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2nnyuyolk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2fwmmtxtr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dbgdyrps.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cxjftftz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czjxlekl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2thvpshzm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahiqxbbb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2niyzjsyf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bbodncze.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bojqmlvo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2faaiktnj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2powvbidu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ttqpzfua.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rxxkomjb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yrmcohgx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hvfqiffm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wbajjftk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oxuzwiza.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zjmbkexg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ugzmrcwj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fthmdlei.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tehetpzp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sfcuvjvw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zbwpdhxq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2guxzptcy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2gchvsjca.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qejinicq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgdxlokr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uyynyqgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfoprjpt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksezteru.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qzriucoa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrhxvrds.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucizbdep.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdpgvccd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pqimczya.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2outrfail.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mluuimle.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2otothecd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hctlxwrj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hxphapfj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2acybnile.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rflmnyct.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ybpwrnxe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qphyeryk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2sumpqtmo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2auigltwt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ozpslkgt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2gdurdwzc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2kimgzluh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxecllwc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ztextivw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2agvptifp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2idalavdx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ffvcklgn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vuoqtmsn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hecymugc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nqrqcfsj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2brzqdrmq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2eqdirnrz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uixwzprv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mqynrflz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2itzzpcbi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ajdbathx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlvocxdd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fayizupu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2yowvxjcc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pofgayjz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2efdujvnt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zfhivtzk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vojgjgvh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yhqbkzgr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2diskekaw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pasnvtyb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2uygvueei.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2unxnynvf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2mctvssat.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qjmuryks.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yqsbwvxi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2akijwdfp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2cjpfwjqv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hxjdrkjx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2phqmekvu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jfkygmnu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fzmywnbf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2cecrjcyd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2emcpgarh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwmzsve.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2idsshxzz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2qciwuekn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2eiryejkl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfedxkz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2rbgdyeem.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ezwovcgy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lqpyclnp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fahvqauf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bfjzraow.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtebfdwx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2norvdlbn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2duomvzju.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2aurbetce.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oqscmzbu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rwrdemjy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2czewdrrs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jlnzskqi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lxjcyfut.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2icebfiia.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnqpgtek.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ilictlby.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zzpvvswn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2raczldst.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2kixcvdxv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mgqqzezf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2sievdbjp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mwijftey.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eviajfvf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bjaewpzq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ckdbxrge.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kkrbulgs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cfakrpie.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2grgcylzc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wyxdayfe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kbnsfspd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2adbcdiat.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2scpltuvn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ocipjczl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2oipdsbyk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2mxrqdbmt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ybcsvupp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tjgsfdth.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2weezdeny.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rtmanffs.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uieriahe.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ratlpumn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kxjmaagy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ceduzlld.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2aifjmhvj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pofacrta.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2afmjcuhg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2acfnzxpx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2avrfdnsz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jxnkjrpz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vnjcirra.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wtleohaf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2czdkunyq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2dqlohcao.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cehaqhbd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2irrogkvb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lyfkyvea.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2znqeqiea.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kzqjoycm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ibupyhho.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2atfyxava.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2zqwbqoao.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2opmznkya.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2rhwjweco.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jdqonqqu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2tzesxcim.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2biwurixv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2znclzoob.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ciazuwjg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2eyxbgzac.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2serigrxk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2iidpygnc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fsbukkbk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hzxfrthy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zutzhmls.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dxnurvtx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2astpppad.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zzodkenb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vgkrpxyb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uffchllg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2klvxnswx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2brgsctbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tizgyoig.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2dreerbgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bknzxwvm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zmpdhpwz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tnkoafij.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pesedyat.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hzvxzebb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ioqrjcyp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2pxwbgthx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kickmlbk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vmtoyfif.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cutdrlha.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gluwnasy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wriogvbs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kzupnzcr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vxpmpywu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tcbcxsgc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xohxzgre.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2alsmysib.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ddzpitaa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vmwkvqnb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2crufnrvz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2tjuqcpqk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2utrbcagl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ageykrzt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2frghqchq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2koohhikf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fgmihqwt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2somjatke.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nlfruncg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wouueekl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wmeycpah.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eyotwpml.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uzxpamli.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wwkrdhkf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ojnfzzpq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sjgozxjx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwizfdx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2otbwxczq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zlvtegex.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tnwowsjk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oxvmqcuh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ialyerki.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2apikxuvu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zfbvigzr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lqsnoqnn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lsjhyvxb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ohnoijnd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ktvfbpak.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dnuuqeju.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vfxzdzoi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zunourro.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2isarpmod.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fvynmthz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oikoldxd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wlmwimvo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2fruojtcy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gpctekan.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2owqdhgry.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2okekrypu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pvyxgpll.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xzvpxggm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jrwcqsdx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zylyeiax.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qrhzfuyc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2facepren.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2odimfdtr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nwyzraci.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xobezanf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qucvvcou.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bmplqklh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rxgwblgy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2kselvayb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uvqnagys.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aeeuyorh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2uayufppt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2htjfmbne.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2tlubpjvp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2eidwkmvq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hegvgwib.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2mjelzmns.html


<!-- 参考信息 -->