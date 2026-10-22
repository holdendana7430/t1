代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2dspuxjsm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ulwkiiif.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dweienat.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocoljnaz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvdnodns.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2varkfgwz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gkwtbaxo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pwprpbzb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxicdinb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kcmcrntj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fsjgaxua.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbjbontn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bggzxxmh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ofgkwfbf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xqprlowp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sqvlmdio.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2abrifwit.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2elcaugcs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rwviffqs.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2sutyndta.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zupawelo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2durxgxqz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nnbaigtm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vyrdymmt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2jpczqpbe.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uozjzzwe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2roynzctp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2twdeacwz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2nbudzlqe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ptcdyspb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mhhxplnf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lsoeqtqi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wknollkx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkrvysdi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wpcbeqhd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2arffwrta.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tbqkbddi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ufhadiuh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hkxvzwbr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jjepqqzb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kfkkvyiu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tmlrhqkm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2evubvuaq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2hdfiehvc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ypiwycbo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mynylawj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nqhvytxm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ogiyydnc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2blpzxsgm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yskbqdnu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgytrkbz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2nerunbsw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kuspphtw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2buqwwlwr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2elndyglk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2khxlacpt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2srnxnpkm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2anblegql.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ufimvmia.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gfvscreu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fccjxgzu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xfididod.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2maywzenk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lzfxufgj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tkbsogcv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2znuckzom.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fklifnad.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fichzwjc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ikzdfamy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nccambgk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2temgfjfh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nerlryul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnvcirft.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ijjjiily.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvmklcux.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kcshpjkx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2acwschpz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fookpoqh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2unmpdamo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxnysywx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qocpqpmr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vrzcqudo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gibddcjy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2liyhfyop.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zqgcxkyx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ykwuukrt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfbcshfo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wdrvavce.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqufmdkn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xyygpsmm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dpydtffm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hxnojnbz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pnectzgj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2imznwjpy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jmjdlzgc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2czpnblyc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2eccpoltf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2iqmhhafn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rclgljct.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cpoylpnu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmdnifrr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2qyblhruh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2iqayrqnr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fflnazza.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nymepydi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bprweind.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2oxbzpqln.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2eeyjviqo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dburuyub.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kufyimbn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgfosuw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2bidwiyek.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2olkkcfqz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nwnpusui.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zidglvwp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qzhvikcp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2yhigppjl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ejzdobsv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rsdjnahs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xtwcgisl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yjzghmik.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rkimbyck.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tsdmjtii.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ddqqpsaj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2keeskumu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2uzhpqjuf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qjqtbomw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2piqjxkob.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fwbqecov.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vbpbrfql.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2urrsybcx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjeimvnj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hcloogzb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rdsbysqx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ntusytfb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kfwxcggj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jywfbcda.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2puselaep.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hceeqrjp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gkmurnra.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mtoyrhcq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzidruqh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgvhyejy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mkjgtgtm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lascssna.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sngivmkt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2utkmdffi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ftrjwmhi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujxuiefw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xprttvek.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pzkznisy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fqzgyrdg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgnckbgh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2itwyyrbr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qpnbsswm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vdipohzi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2delonsyk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jwujwhqc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rxvfecix.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nyjxywpl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2svlurwan.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mhwfspmv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qitrcyuc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2alcsdebu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tzmetdwu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2mnoyjven.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wppailrh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hellvnjd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cwnfrphe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ypzpapdy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gamhthsb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pyxroodm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2isfwvixo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zwihvbkq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2uvhkuvzo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kvppiran.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2imvoptcj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2btkjhdsl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ontyekbx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2lnfklmne.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wyebadnm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2nefxitcm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymrvvnvd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2idbtfmdd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eziiuwum.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gksganro.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2snpgjsqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jofuvbol.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihbbymus.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rlqbvami.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jpztjgjg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ackjkrpo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fsdmnpau.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kcrlakuz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kqzhpqcs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rhjexogf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2bpdwqnqu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2iixeckyj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jqyagzjb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2eefegeaw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nvmgtsth.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zupvhald.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hztngrgq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2shtdfpiz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgxgfjkm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajdaaxhr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yzwbtsfn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sxrabxhi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2eujcarxi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2azzmcssr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ccrqmvfl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2umlcvsbc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yombgghz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2xdxsypyv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2feuteust.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlmhbfxs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2utszirhu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jmoqsbvs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zltphuni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otgkdhkl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ataueeii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqzuyyob.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sucsnouw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cmlrsqgd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ulefkyzh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sljjkwik.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2lvmqppwq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qvscpwnq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sncpxuct.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2iilykjqz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2biuivldm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2lgzzjdja.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ipgbsihd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rfxucgab.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ovfiynkf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lldeofvh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ldxkbvmn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xatwhplo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2wavftuil.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aeajyegd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gyqeobjv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ipkoqbtr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2iycepocz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dynqdksl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qmcpqkfo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mfykdcyo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fgbxygie.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wbkzokzu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jrczmkka.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2eukjxnun.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2momdaupg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ebqfzosz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2hpiduafx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ihwczffd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ycqybjen.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2regkhtoy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2huyiyrmr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qswzyewh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zvrzjqfg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gbskxgkz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gjonnxjh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sntpawmp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2rqbbkenc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gyukibsp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yzfnxdqd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fcrjuiau.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bjzfjvmi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2czrfnlgc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cdmidaao.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jzeievhw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oawfnzzi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nczlpjor.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gvlpqnuy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xqodaqgd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ybkieqdy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xlhcikgb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xjyzylwt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2uzxhfvny.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gqpujyex.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nmrrwkna.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ssedrvsx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lfqloryg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jfkamdcj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xdymgmsy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zbvirryl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lgaqgwgn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hloozgez.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rylrgiyy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2idkouhtn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vbbbdhgj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ihjfxpsf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ndymwyjp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2yfcdodum.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eboizcgr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rhgdbnqa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2twymgrzm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqtwkgnc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2nvfujtan.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2thidammd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zuxvgegc.html


<!-- 参考信息 -->