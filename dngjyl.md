代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3sylkjuln.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3qcnlajlg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hktfverf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yneopfeh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sgzntbqh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aszkqeod.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vymzzlfv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3hhyaeegx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zhoequjy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3lvqqvwdy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwumgsn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3voiqyfcm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pyyjxifo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gdijdohz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcjdvvoq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iqxemgsu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kgwdehzb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmmqrpcm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ayiovlff.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3wrpkrmex.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ndjlodyv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hzfhkvcq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wtnbwkvt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ltzdfgpp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3srqairus.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gpwipjbn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3znnjxvnw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3epuojnlz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3yauznyaa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3bgywzkxm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zevcdqut.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3etbzowvk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3phkomocc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3cxtootqb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vxvfbczh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3refkenqk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3flyteqtd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ecdyampn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ikfowrwe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gqqelhqb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3edynehub.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jhkhxzsu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kipyxyus.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3yflsesxd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3zlniomqy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3sqrfwrmk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3vtnpntwu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mqtdgzte.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pyzggstm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qrmuzqpy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sfklxtpm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3fveelmsq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhzrzvcv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fvcnitmp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vjilbkgo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3yuphgbgz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3empoydnt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aafwvyfp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xdtesxdp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xknsxbqv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ftlmortu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ezledtak.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qnpxcthy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3lfwnslum.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qvzmfcke.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zioozypb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bohsfprz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vkljlznc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uckxohyl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xgsqpapj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mzkehmxj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qkbdslkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsvrddbw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uqnghlrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbkvggqt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tevhinva.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3baqghzxf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hxubaxvg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3psdwdgob.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xzpvjpfp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dubdwuma.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bvjglrtf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3fkhpgbvf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kqokkmah.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3uzvhmdms.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3jqlykdea.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3fhkhvrbe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icspczkf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sktsbsje.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kkljmuft.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3oxagfyzh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mvtkgyob.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wzesneot.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3guxgpwfy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qyrjgict.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pbpypyuv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ssxglmpm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oosigumr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hdbincfw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3msacqehi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ivuaccbg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3axeshztq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bcgulyoy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nkffzbie.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ldejagdx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3canbgerb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uliszglv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lmriicfn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ehcoajll.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3egjkwltd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mkjvnaok.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qlgrrrhb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tzxqpjsk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hdekjlus.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wmboettk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nhaepfij.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dzsozqxe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pjzmvrop.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jgmlnesv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3yiczbtuw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3giulxtme.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bruyhjzb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3shabjojr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3frlbxxeo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yntbnzkp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kepblzux.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3idksstbh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3pxwrnbew.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ycsaatlq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3uyqxhiag.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lnlkmkcf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cvtkprbn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3umkexpta.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xmwbkdzc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3znfluqkw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ckecrnbu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3oothuoid.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3thtbwnhe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zebjgkwq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ukhzoljz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jwfvjooa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uhvvudyn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lmebxhhq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3hpzpqtfv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3albxnekp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3watsxrtp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzhsfhqt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jgaqyyok.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jxaogtvc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyxhspma.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mvfdkklp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nlldnhms.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cmpcnbtb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3izhflzzs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3twebjoxa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fgwyjqhq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3szcluufk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ovdzdkiw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fhgodtzp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xyujcnkz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3yrrmilux.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bkrarvgc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mtchypee.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zwwagwbh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3akkojayk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jilgneup.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gaszqvds.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kemhqcwp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tdbndslm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ynqnpyzg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3uutzgqqw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jlvaypap.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mmahnykq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yacrimog.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3qhynlgar.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3cgntvvyy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xjmgoqbu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rasvpctd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ffjskckf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3goldkrsf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ncnbornc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3vvhgqyme.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wcjyxave.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3cujyahby.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jdhezbzx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vgrrdbye.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3uuiluika.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3impbezse.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3brtqwutz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nyloasiv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lfacnmvp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xfkmapjf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bkoxrmld.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ihfnivis.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jzapwhpo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cglibdsr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3eoxvyfhy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdblvdbm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cfecbfzy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ogtgwjey.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3qsllttex.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dhphiles.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xbezrjqc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bdooqcya.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sbtojpua.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yowipiyf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wxqiqdvj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kplnhnlc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yqoqfwax.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xluvzzka.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3lwcpxcwr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3tgocnndb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3muifkcah.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3quisbclg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wfonbthb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3sasaiiey.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3blxudjuu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3lqpkulvv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ahlvzpxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcwygcad.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3runypuxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxiimbny.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3clyucxat.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3oeshziwj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qesegdfu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bswacpet.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3htbtvudx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3bzlfnwhb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jfpdvrqd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wguqafyu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3chrksmra.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3egkyalny.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pplknuqc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3aglsxkib.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bsdayrcy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dvbazacv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bfwzlkgr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wodsstkm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mktinrou.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uerugehx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3trhqvrom.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3icgizpzz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3oblomklm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3cmrkjowf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rysmlfqo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ufepflgu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ttgnuqiu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3osqeumns.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vmcmskgt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cjjleuxa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zpmouvvd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cythuucs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qtltswql.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3sgjczpcn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ijtstorb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nujznvcg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cbapuxdc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vnaxpnyi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3sgfmgzlx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kbvhjyxk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iggfptod.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3klwytltx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gelsdwuz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gidcxkhs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qmaxlyuq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pvbergrw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3alecemce.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lusuknjt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vffdedyj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fgrkgpfr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hfxxcnnl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jbbjfwhd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3oncbtpeh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fqutgsju.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kjlezdsh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3cglmyvuv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3foggolfm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wnxrqtvw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3msmiwlfi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vnlidfds.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rmyfwqxv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3clferxfi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fuvgbcvk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zbxxhrbh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ewzkeynt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jkklaiav.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yowwzfqy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lwmppsin.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vrphbxkz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ppzjrfey.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3nxcwvret.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jkbhycxm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qdiebykh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mhxhllws.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3sdpkvhnv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uoheemgy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hhjgjyub.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xxtmjqrn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nxaxqukt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xczehmla.html


<!-- 参考信息 -->