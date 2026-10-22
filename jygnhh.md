代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2nkrcjnkl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2inxfahfj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvlebtks.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pcvrdtmx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wobmowxt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbnhvcvj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2efwatgan.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wseyubdj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wdqqbmdb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jnucxhze.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wmreuegq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2psvocxtw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2izcjnxix.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2tqoqtdnf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wcjwfbfl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jtzgjaxb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gtwcdkrs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymmusgxy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2varaaegc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bkdlqubm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gwrjqcxz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fgtzqoyi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xmmulusk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ltazeksm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tmshjcwr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2sfxauslt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2toqagrqi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2eilmyyxw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ghzuezhb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2pqpgfdbj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rmglpvlp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yubiccve.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pmbojxsu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsvcptny.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jazpwhxw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2afncoziq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2kddspsnw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2sjidadms.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2klymebji.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ardilukf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vfwuhnjm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dwcdrrth.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cascwazb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jvyslfqr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2runykvur.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2cjaalvjn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2spittlql.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pfrugnnm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzsjatki.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrljzrev.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tlrjufja.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2jbteohys.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cveynmgp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cgcmepeu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qxstwtxo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2plepwejs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nwymztki.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2onfrkhto.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wiidnhzw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kowdzrmf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bxerlouw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zyisrqxa.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pbgbpiyd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ysgjgkay.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2iecctoxd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fioqitff.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rjwpgdkz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hbrjdxmi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pbcfgvxx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pgkzesod.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mmhokmdi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nnoaojly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kagnhjzg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mfmuxchj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmhpwozs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2muwkcckj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xrrqlqwy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvbnyuus.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cstlcvus.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiiqckhx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtwkgshb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bplyuuof.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yolkganr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ljhcojde.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vsuvfeft.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2oomwqjpp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qhwxfmqi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lopirebh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgemzbgm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hecwgzns.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zrhoqvko.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xnvfyokk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rzyliyak.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2wlignxxb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qbmjfhek.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2conicqno.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qstivpka.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lgufjsmz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ayemzoma.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uduhuqpt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2pbwlpldm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2mxdwnyjr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jrpenjgd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nuppblhf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2yusapbmg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pqvchznd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kmneevbf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wppzlgho.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2nngxjluz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dbukxqoz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlqjzbpe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2uapmzavl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dzijlvuh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2yxmwbuxt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2otjqnvbr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tldtjfjl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hdjcezgc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nanjalxx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rduzpmjk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tnodutpp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ickjoods.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kgbugkoh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2bvnuhlzl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2epntrcdb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lghdagya.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xxaiycot.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fqnkugjx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2twsniwkv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2etylygii.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ofcmmmvu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2uszkzwtp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emzafllu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2blxneqzs.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wygdqtar.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tumniskg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rvwxfbgn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2luayguns.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2shpqqieh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zfzylgvr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2sryvtkcq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ngpdgqbs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kejbxzre.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssexpnpc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nfhdqjcr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lifdqtyj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzjgzsdn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rrrthqdm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jbpxcmli.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2abjgjmgu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2swqqfdsb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ozpixixe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lqmmbhzs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpaxjxmf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gstubqnz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2oifdejwu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jujjkurf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2sgyiskbo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2arokeild.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qzrowhzm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aqnapojp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hzmttzzx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zjstsjjn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fokjthfk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vzieqxir.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qwyfzggi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lfzxwify.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kvfdhmza.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2zfohdpwg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zgwttaqk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2daaxpofj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fkaziuna.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nilfyfds.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wjjczaub.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2dwwwxavf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ppfxckdy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rxosmepp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2tsuxpmim.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iyjlbaia.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ohjtduui.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2duftlyjd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2phkvnncn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2mwiwpoik.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qcewoscj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hcefjnag.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gerdrngy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjcyodhv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2cjoywlou.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjfrpltw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dwlctfui.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fheujivj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wvxexxoy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2fzupwtbh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2scrsbhsg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xymylizv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aqyscaml.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rsthbgvv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2btmxsccb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2jhwyzadf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2pxhtpjsa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mwphufbr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qcveeyfq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zbrtycee.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kcvabxms.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nudhqvyq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ysguybry.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2pmeqmgqt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wjyddpvl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fuxxfmca.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kqagvzza.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xzurghfn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wpfocllh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qlpsxuju.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zqddnapc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rnnimbdm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2qobeguva.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rjetxxzx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gmdrnusu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dzcwykzt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgghlxcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuqterpf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nnqvqgzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dirqmcbq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2valpxjlq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jlfiilco.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2otwludqs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2aoxtqbhc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tvzlibgy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kajfhlqn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vchxktnm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2pffwclzz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pvkyfjxw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rtocotjt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zxuzqxml.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2otchnxtu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jkzrwafb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2crupafzc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2voeijhax.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nboyhotd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2sirsdlso.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dhgxadnh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2wwylslez.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ezhmybka.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2irsrensl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ssvvkhwu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lwmxnloy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fsmxtkno.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gfilfjkf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqlwzkpp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2obcwwydr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2iqxkxyqs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2yjxturwm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zmnrvvfe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2phprveoi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2urgtffqq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pbdcjspd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2yldfyfih.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uqhjcovb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dsbzgcql.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fvobraiz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sexztgjp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jbqxoueb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kgwnejhb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2luqdcjoj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wimbxflr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pfcsrvow.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pogprqud.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kchaeokh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mxizbddt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2svxfbpcr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ydmuvgsb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bikpqygj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tltrjzra.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2swkmheye.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vigdfrjd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2moualtwk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ucbaatln.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xuudclad.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2fslyiasx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2liwdiaar.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lxsjevww.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xqblzsfw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kqzxmmdk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2tourywrx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xxgqezuh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hctsjxzu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2taohcclw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tsrwdkxw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2civtmtoz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2aqmmfigg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ikiaxorr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2awqogosh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2yjofkcxy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2esckjbun.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zcxgdmhf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fouvfros.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hgvvyaog.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ujlckliv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gurcuzqe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2doyrmwlj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2gyomseha.html


<!-- 参考信息 -->