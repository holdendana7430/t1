代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xfxyhipb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gwafdygn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vgokizfb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2glzkxomp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gmulzfza.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bsvoayiw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ejifodho.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2onghmahf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zbqyzmck.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nkrpmbww.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2yuxspcei.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ifelotjd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2efeojtjz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2twnztwzb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2giynelvj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ciwncrok.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2swodxtan.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipdfiiez.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2dijfataw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kdolenan.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hhwdtuqm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ubnxdxlp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wbbfqcnl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ikozyzwa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gxxwbunk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2divyagdi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hgwkvlhu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fioowgwl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2eielojxh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2cxssvips.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vnccolxg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kypejiez.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2abgzkcvq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsuhyfup.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kdvbxlng.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2koibbded.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2izfltetp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2cksbpyjl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffmxsdzx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yewuwzln.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxojutbd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2fbcszqhy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2odipnbor.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vcwaugbq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nidohjkp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hpgsserk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2iohbutzc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2sunldryd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2skvrdioq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mraksxow.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tkomtgyt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsykdyms.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sritqagk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wdbubiyz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2svqjmred.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2boqjdxrx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2unrwdkqp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qvrbppzv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iolbyxct.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ksfltmdn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kzesuqtc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hipwtawy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cdsnollm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fjscnwsz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qumqycrl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xktssola.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zpyajtkn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xehnzztn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rlxejhzo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vfsmmclf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jujqiffw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lrdvvmgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcuuqqcy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2udbzwnza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvifmtna.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2csqhtgad.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wiawovac.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qhsmqvvd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2txorjtgt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiarksmi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eitaqnlp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ryuztenz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2axrsnjgj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zlzbfnvi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2uypyxqwz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nngzeomj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2sdvrlbyl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kymjolym.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tffkfhuf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jxtdtvyi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dwqapxlm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2bktulfqj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hxptlekc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2moioyyxa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2elilnwkl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2cczefndp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zzdlhyml.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2thhrcsog.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ssobisjo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2aauzncem.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2gonjanss.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2zfefplmt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qdvlpegm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjrrahu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2zdprnycp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ixpptbhd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2htracllk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bdqbjlgg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pnzvdzde.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmjzndi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qelpsdzd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wsrcxwzx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mwdhwuvj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ojcbbpss.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mnqnwhdl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hkjebdcz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kyybtyje.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2sthkbgrc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ueuldmwn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2srhdessn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2swelwacp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2sgprcyhq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2omaxrknp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zvpkuhuq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lyszrvnd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2drbflevr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lgbkiqtk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ilsjbiis.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2alqautoj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2codmxgby.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hiwjejfs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ijfipdwu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vambzesy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xdsqtfzx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rveffacs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qpemhtri.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2klukaugc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hxxfabzx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wgghjwqe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lmxqjtbi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtaeldhb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hnhrgewu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ftsjdkms.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2qrvrzhli.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2jsjotmol.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qnrxdnlf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qgcqepyd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbcpvwer.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqrxlcks.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hnpaalgu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jylyrmxn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2knomkhdv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2eywybbqa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mjlmvepw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ightnpot.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rvjzjjtj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2abikdrik.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2exmrgzwp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2swehjvoo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ypsoblkk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rrdeaita.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xbhdxzjo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tbvgjsrp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2yjlqieqr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dbheplle.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ndazhjkm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zflshahy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2waifjvok.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jostedvf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bmeynncm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2byeaaris.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bpvuaqil.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2dcnzrldb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jketgniu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kjtdtpwg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wsrrvjib.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vlnuzgrl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ttpurqoi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hpmuddhn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2peqxngdf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gszyxntt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2iiuctvlx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bszufnqm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hhrhazfh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zahoaxkw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vddqkrzg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2yjlexaqd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tbdiyoum.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zigmnuth.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2qlmcdcmo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2nlzgsueh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2udmsnstm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ypjdkjjo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2upopxmlv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ixyibpov.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2exprgbzp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipjzmvoe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ibgndgiw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qeqvvgpa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nbaswrrm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2avuhsmbe.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tiptymmc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qpsabebf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nzqhullk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2szvgjeil.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2uockbsyf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vkpuaigg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2opufzcvi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fbvlrfrf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yfiknmjb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ihuhwvho.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cxxtkbcs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rbcxidsz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zqdhsxco.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ccxqteho.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldtbxqqj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ogltxxko.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ymqwchbe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pgdudfzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syemxbvj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ewrxmpmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scldikyv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tiukbeet.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hdcyiziu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dtsjermg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lklbcwjb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kbbwuxby.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lkresozf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2madaerxb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qzyqgttw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2udhkoldm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bvbthula.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fhbzvtcv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2knafblut.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvackgfw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kddanwib.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ltvgtnfu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ebvdbsbh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fjsinvvz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mccotwsk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2axhgskoe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rwjvoqmj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nkwsfsdl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ojeqfbtq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2acuackpe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ffxfdxdj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pscpzvcm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2urtnjhvp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kzgssnmw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2duqlubln.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dzyquuzc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fshzlwmh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ifpfboze.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2clwykdwa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2esiebjlc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lrwexflo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cvjvwtjg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hqxsnlsx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2plbmtyya.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bzsbzqph.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wzlrlmeh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fqnofady.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gjmwsjsf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2obbaewgp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kxuafppe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zabjttnp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jdhqlbjn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gsxytljk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zgianylk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ukfwpqmz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jzrjortz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2umrdxdvr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nacrubtc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lgcbibvr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pcyvwccc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lqxeznsc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2rraoxgco.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sokouhth.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cysmkasx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tqcjfchf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zjofdewc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hqoeeckk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lzzjtiqr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ookcfuon.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qtanafdg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2brsedvwm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2maxozlvv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2giwfmdvo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dtotcphb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xcqwbkym.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vgeqojxv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2pxqmekoy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zziimsvb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dmtwskfg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2nfeshnam.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uulvvrpj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iqvctbhi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2osgtnnwn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pszpxddb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2yrmtuhpi.html


<!-- 参考信息 -->