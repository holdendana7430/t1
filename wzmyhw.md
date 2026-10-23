代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vdmyreea.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jafxyyeq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zsgeyabg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3adgqkend.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfrzjkvv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzfigecx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qvueqfbr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zbfniclt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qbcnsqhe.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ytmftwme.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3slyfpvjm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dhlggrir.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gqpyggpe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3abjudlpo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3uriimpgf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3spjotrsz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3uhgnybfj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3igbculsb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3eyaepedk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3bhmxfhhq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fneoehtx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yvgpwuit.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3blfvwckt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ldquialv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3rowhmfab.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tybuxqtd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rpkqchti.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3elfrisde.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3vimmdyjz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3texfizgu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gnuxumnm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sqzkbwne.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mxwjqwpf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fmkmnoln.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mzewuobe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tjstovch.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ksfumhza.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3veynuiaa.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdydbigu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3guydlktr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3huoyyzmt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xsxzumxh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ycqxkbqi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cfwecfdg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3legsfkvw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bcuyacoq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xchwfyzl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3vcegsqzj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wekqqmjy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdkdxorv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lzgexoau.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3edfyuuil.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulhicqom.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fehjdxsm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kjbztmmj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nnmqdpxy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ishnhief.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3chhjtwfz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3diwvctgs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cvkzqgrf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lsqyfjxc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oxaqbzdw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3invpzgwn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3chxpwvef.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dfcoilyj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3obhglwve.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3djwjsasg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ccxgqqfw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ynahaxit.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3trbxjquy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kxgppgly.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ovayvxzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymuwwzua.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pvmmjpmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpyfcgox.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3enwdqpdk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qjascnuh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjdufppk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckuazxbn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aqdvnbed.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qvxltzaj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tvymfoeg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3krikaxng.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xeismxuv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3xncgjyaj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3uqopcpgv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pllgktol.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kasiwwig.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nomjphbg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jjdgneka.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tibruryt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vkyovico.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3tgrtelvm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3voojwnmn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3uckrtbjd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3vomorame.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgmvoxbd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhumvrko.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ghrwnbrf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zqqgbaxm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3oudbamyb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3sutfbwng.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jimyylsv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jqvaiaix.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xcxmdftb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jcwtwfsr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3haizezam.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hzlrjuae.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3etqkilyw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnmfbczs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tmzpbgpn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3iqkrpdps.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ohawekfh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3atamnfvm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kaierlce.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3awxhjsmo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3grrxgsdt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pkfqmcgd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3euzlemjq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3orrcdngk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3cqwtxhuh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3hbcwlmjy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3unqmoaqg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uqkpxuvp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tgplrqvg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3udratmoj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jslvamuz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3yadvvizp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aooqzcam.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3dthccvii.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3alzlohpi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rqxmkngd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xlqcfcph.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ejmuxwbh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndejaadt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3twelwegk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hygshcve.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gusxhxng.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pxnshzsv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3yiqgfuqc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bakehjte.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpzfzges.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaswlhjd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cmtsdkfc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3pxmyxiyr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qrhocieq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bwmjhmbz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jcauzvdt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kzssinhx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfyimmup.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kqfhbrcc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3taydyczi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gyqeixbm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xyjiokdj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vnvovnxk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3djqdwsqd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3tylrpajb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3glcsxipr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wdxhmgnz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dstmrwzp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pxdinfct.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3effwmwqc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fwfbwlhb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gsgxqdre.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mdzuiqbl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3aqdoqrzy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qmkltlkf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3racqjflv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dxeswcgj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bfnfxepf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3knncrecb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3gtznmbbh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3etfxlwrp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lmmfrqbr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3emsetelv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3thyurabi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kvgipulz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3grtsygcs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3shxcdjwf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3gzjvoieq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qypwoizb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3imgjlter.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gylcawjp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3stxqosys.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xfkzigpp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqkuqnkx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ivqcrjrw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3akwfuuwm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbwditzd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ijguqmed.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3irlbnkxw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3kjqqsybp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3djmbefma.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3izwrsoab.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3brkoqzdz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bqpsiuno.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuwsebzv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdokbphb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cplegccv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yrrhumxv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kxvfvjid.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lwtivium.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pjiezxhr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3anlfwstp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yvirnaov.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uymrvbfe.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lfmzlmyk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cpkrhdwd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3auiixqvg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wrubktbf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3taozxuff.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3cviqhqag.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ykmhryjp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fkfwsmzj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qfayutcp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utkfmmko.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ogvyndvh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3mpfbjaex.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pbcsrosc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqornlrd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3twcjtpmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuvjpqmh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dliaukqx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mlpejqvw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3evappklb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bvleilbx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pqwralfq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3yadfoxtd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3tzvgddms.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ewpxosjj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ildqwhqq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cffqbijo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vzulfsnc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wqnbicvz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3znciclia.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bzhovffo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ihuciruu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rqcshmcs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lijwtyld.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ftuqqaih.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3miljgvvj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jzzscrtj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nbrtjzxo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ajfbkgkg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xpqrhbvt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jvchovai.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3iaolwani.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ndzpwynj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ztfgxmcx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3sljnsvpj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uslpbtbw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bwmamjsd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3yefocwgb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vsdtwwkm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3yoocwnlr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3evrdfnfn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxxlpfc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zrxlbqzn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kvyucuyh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yiuisjta.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3powcmvbd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qiavrenz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gjiitkgy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3wdkzhvnp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xmrrzddn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hqcssqvi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dgnatlfz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xhhnioie.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gsviazde.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aorlquwc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vhggyfsy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzeopgae.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3cilzpdme.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hnisqvte.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ecjmkvfj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wrhivknr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vjhbebek.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mixxxlxg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jxwktgbb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qoyctywj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lqepukqi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oswsthuy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3yogvbonr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lfgiuuvg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fpvistto.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ljpkynua.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dgvtxppl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pvbgllak.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3leghpjli.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wazywutr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fobeqijo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3forszuau.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bfgqlzvx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yxirwsoh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pdxxomhw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dvwzljri.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3anumtjjy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jturazqj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3cgsrvjzu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xjaublbb.html


<!-- 参考信息 -->