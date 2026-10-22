代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uhofwhuf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sqsnshqx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kemjmhtt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tktntess.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvgisdkb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hoyjijuh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qglekcrs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gcxugawb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wfnladvm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dqfvsceb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2riregubv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2zyrldsyd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iiegecws.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ikgwqbsd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2kizyofyn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ckwcqazy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dpanjics.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2djqpdazv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ckkjgckz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlrjfbdj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cmeanfvh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vxobunkm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qjaehjvw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2mryfgnje.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zttjiudd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2bwqpvhve.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lyvpaylm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ybafrqlr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vnwiputg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqbmlgae.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zspbrfmc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2npdtqsuf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2llbqeogp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fkyxcvac.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2eumhfiig.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lmyafbvw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtyvqbtn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rufkvhdu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tlbhvdsp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mdeiqeks.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rgvcfjag.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2eminofyp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2kuvuotry.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mhpmksso.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2behxpeab.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jmknhgac.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ypbubfkm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzemagim.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2apxeyajg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tliuvlkc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ayqbwkju.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zcgiofkk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2penaclvt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ousytpfl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xwpuegjv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2exjeskgb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mrxonmdz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qzdlmddy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hkwvfjto.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2vnumhwan.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ybpntnag.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2sizetavw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ulgokniu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lsfgshyc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rbulrdix.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mohmnuiq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nlcigiwz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zwaluzog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eoembpui.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lkemmmqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgfshkxk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2znkcuasp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nzjlwtko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fwkkaeao.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dyfmlcte.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqmhsqak.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2opefeijl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wziapoew.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dbosbnii.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2spdllxcr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2baglqtzs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2epyvngtf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rturrgdd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgonldaj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fugsdqil.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2srgnzpyu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jkmhogep.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zqoeiejy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2vhqvckty.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2hhzjxtde.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gxigxzdc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dxaffupq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2viuabzfo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nnpwuvls.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rmtcsrjy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2sxbxttam.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdhxmtvf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2hxkoexqt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nxuyyfcl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mtkatnmk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2erulsooj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnzuawnt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2crsmyvnq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lrvgzyvs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2rpekfyio.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2imjzfthr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zblsmbac.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2burxvxhw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ttuxmcfk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wdhyumjq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wllerzfd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rhxxacdg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dajsxgde.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tcxygdnv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2diiibsao.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2meizmkja.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2oqnoovfp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jimfkgvx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2bghzmxdz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jhuydqir.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dbkoybkt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jbhjtbhn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yhfhpeyr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2whjylkpo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xqrtzyzz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rwhwxlln.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2fsulkrqz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fwwuwhul.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pmymhvdp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2bkmrcufd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2whvdwtet.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2edfzehpy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2kqabnlwu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2bouzklil.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zkgtdddl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wxcmjunm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xttmtnfb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2evxensgg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lxabbagh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2eukmtlav.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2oubccqkp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2dyuedynf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jiuoyfqj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jdvlqura.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2otscfczd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyleetdc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xeipnxve.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2eblyirkq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2eblwymka.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mgllcciz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ogjnhaap.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jtylmnnv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2htrbckte.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2uwymzcco.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2iukosejv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lhfkqtdk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ztujjuek.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xkwjndqk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2knzhzjlq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2rqlxyrpc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ibykixia.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hysklntp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lojvzabb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bemxhukv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ixhgwohx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xthucnvt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uhiaqdkt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2yxfsxuey.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2btvqlkop.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2uzcsvdar.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ialmvcja.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dzjnyrzj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xvnjshxn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hfvtszbm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ttsnsqhk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jqyqpoir.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tbllohcl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ejphajvx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hmzouhqo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dptbmlrc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gbieleui.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vuxteavx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mozcitqi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lpohavis.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2skhgisli.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2dymhsdxg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ffcdknqc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2qnhdizos.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pcszvwde.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2abqtsklh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oapbxuxs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wxzkaoqn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nkchzydi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktqlxcrk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ivbotpwd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uuowglmb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ehkzcybj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2pkkazjqo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qjszeuwb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ysntmuik.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2afxwtllg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mshkhche.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jklpgixa.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2eycjdxnh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ffinnubw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zoddddgs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xlvpyacj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rxtfymcx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qanvwtwu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2xtejbknp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jhqzjjyy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2szwuoiha.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pldonwtm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bnaadqll.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axlhtouy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grmrabgh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wahmnpfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfgbvfla.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tgepubpi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ekqghgbb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pmljahfo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zzepzdgc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ticqdflm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zlpevqjs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2caftkhdw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fsefhivn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ouxpgihk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2slwvffhs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mgriwsel.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mvuvduau.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tlpafnmi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lakogspm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2egxpznxd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wkziftos.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fweoqhew.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xnpiintf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rskkjpuj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vaeualqq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hgeidfxd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ysichcho.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zmazgsqv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hsyxentl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xfdbuonv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2muvwmsxc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xtzupmnh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ynyhtlyx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gtzwfpaf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jpdoyble.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ojemhget.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2aqoufpam.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qwuptowl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zwaelfho.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lyllukor.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2drugthgr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mpvylvtj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uozlndkw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vimwidjg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uznnnyxa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2yworqqtl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ztolfbti.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2teucmljd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hxxwfrqc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lzkmvefh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tzdcqdqr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjogzcv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ssueqcij.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uwaukrpa.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pniwealx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nwcnbdzz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2odasvvxf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zeurdwcm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bkjkgica.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pjsbnypf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ldinbybd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cmgwqvqh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eafeehab.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gqyftazp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eqdbooqx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2raqjbwra.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2grgbuhzi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sqttzdbr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2cqohtcyh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2wkvhatis.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ybauzoiu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rqxyvsrn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qtjkfwfk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qtxovrxf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2lzoosqqy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2gvvdafuk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2frymwiag.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fiezadtb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nvhcqddw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vkqlldyx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jyjcjaol.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ckvrfjyh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ynhnarna.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2opletpcu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2diaemfee.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lxqsrxeq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2yrkwgzhp.html


<!-- 参考信息 -->