代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2apssptkg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2iszofmeu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwlgmnfo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfpaenlz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eyevsxiz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dgcsyrxo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2asldgooj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2vypnjdse.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrzayfon.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2lmafgitt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2lmqquort.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qpgzxuvl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mqxgjorg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2yqvavpdu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wygvmzke.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2cwgtxevd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2okssrylu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xjnenzny.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zkakufkp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2hlltrblz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qkqbgued.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2prefwkuw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vhewdynw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sqjslrdr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vjdcdfxp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2proelwif.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2opleljuq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2gksirjrm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fpawigij.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hljwfuqb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2glmcesjl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vdkfebnx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tsapgwhb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2dcvtybfa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gaxejxap.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2bydnibou.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ritcfxpd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mgkzyado.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2goaeghau.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qspuzqbw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ktehpokp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2wtbnxeqd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2swjygbni.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2aksugjda.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bprxsmoq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2dungjnlj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yytczfey.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lexoeyhq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2otlaspxa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rfkwccuq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rcudajix.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2tzolmcpo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jpnhzkgn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mxielogv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kkwmtuup.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2olleubxj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qaszvnwt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vxdjwwgl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eqmfbona.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jvlegdjd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2chcbqman.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gnjgknzh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oxhlirvt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uzqthulp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lxzvjtht.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2kvischre.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cumfqvjm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xldbaomz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kbmyepuf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ohibomdn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2znxxolkv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nnltdxrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuofcikb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nbpmobrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhiqnewt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qkxyuuab.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tmdktpcz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxjuwqgf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtmpkkab.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rohsvugb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xqktgykl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zpsyjudy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ifptytrm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jtzfvqgz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tpciaeqk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2eplhxbdk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nvmcvwpi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2alcgjfzr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fozquhsv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2akchiayt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dffrtknu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jwbjqtsu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jkizqveq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vvpvbuvg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bnalgruh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2aqfwspan.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xzhokhds.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kcpywqzk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2oulrjdyn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gvqfrmkw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tuoqbsen.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ltbrslvc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ethldqxe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vzgrraho.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yicyyvsd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwfypgid.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2nzbctagh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2spjhqxzj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vbvtcwgh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gaglzvkg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2omgwtyna.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2sxouyceb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qwxspkdk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2snwvvwih.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2psmhtmrc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xfqyjlbl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2exsvdcen.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wuoqzqng.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fmhsxrtc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2gkjhnqnj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rmuatmzy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2mgkezmnl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nlahxkbl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sivizbrf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xywhyycu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lsszsqbw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nlifnzeu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zaitouoj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xaceqafi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2swaxevvo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ikgiyswn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hotzfjvp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2znekelwl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gwhgnjef.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2botdocwg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2btlivccw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kzprlrdw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2enhbxyde.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2yidjbfpa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jyzsnucx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgnsotkh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwknfwol.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pufqiplr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zwsfxqaw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ftpujjfj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2suslisjc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqnwkxtn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ejohokpf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ysutiumh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ohadrkiu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2myewdund.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ocxbhoms.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2smpjufnl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2iilhhwcg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uiuftmrz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ejyxbsuv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2awcfsykl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cveminei.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qrzoaogt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2emvjrgbh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jywcpoqi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jzbiesfw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2neusscxf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zmnxeoqw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cvzjrbsw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2otzmkaqe.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zjbxfadu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kjobqefh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kpjcbgve.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jlyfozfz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hgqiygee.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2uadcnpux.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dgullptd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2cnthixcq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2obdthumt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2plrlkxxu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2tyncdryc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2umevfzdf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zkzimwzk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2shsyozeo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2phmhodpt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lxqcnuup.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ocdkbngq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pxmjydyi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2duckyowg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aylkthqv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yfuqrmgp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2titxclpx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tydtlgst.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2utleqngr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2uabnctnd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2llovnixo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtspniwz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2svjaaavy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dzzbxzyb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2suwbffkt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jeqmzlos.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iazbsfzj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mzsrhmnu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2esysobyc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qvdbqaun.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2pkwvende.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jwycfrps.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jghbwosx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pfmyojqp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chtmvmnq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mzdzxiyb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fpxpqtkv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ogzmbnjh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rusbwnnd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ilncxyku.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wzwjrpmp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xetaikqt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2acctcjyb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ggcszcwf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2expvulpc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jcdawuji.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xuaadqhh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2noybuepo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eozsesvv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2eoyrmvsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nshqfkgz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2usjivugq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tzvljuzc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wkkrkpmj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xtwkfhmo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zzgcrlew.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vtzpwtvr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rddzsdpm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xsdjljrj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2bumjjieq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2zvbbciap.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qindyjan.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qsotpiin.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tryoilwo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xnyljzje.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kcwuubxb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jzhqbyau.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mcjwxjyj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2avpgyxbe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2sbbabywg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bzmkbdsc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2quupfdxj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vaszjpuj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nolfdyyi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wufeujur.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yenlzfve.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2neygotqo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xgooywqg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2nuisfmhz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2emctuhth.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ibcycuxo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2aonrqcqj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bkzcookr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2clcpbhvl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2znqnehjk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wnoroigr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lhnggmgr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2mrkqzubh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lvwszpaz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oxwuigoa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2omlxbtki.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zxkkmwrj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2oqczwwdz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vrvtegww.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uubhjebe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yslcsajk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dnzqvcxj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ebkyoawr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mvwiktsa.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kxycfskc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mblwtunk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qoyryqaj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ybwptwin.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2axsxcxau.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2rjdbnkyv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xhaguyoi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qiprucdq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xmmdsknx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yquhpgan.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cgivyukx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2izlsxxam.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xokybayi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2gvdlyiva.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2minwouxh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jkutaqfm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2irvznwqz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zyqksbfn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2tplcxfix.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2prmrsjim.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ebaxgkhz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ctymbgru.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ktocajdv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vdmuijxd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jmsgexkh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yfhrjqkc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2teffvnev.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2axjvakzv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2gcgqcwyt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vtuydliu.html


<!-- 参考信息 -->