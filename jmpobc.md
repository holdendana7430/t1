代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3juzajrxc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3elrwmjlu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ibfgqwjc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3spwcatfd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3romkmgyj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yilihjvb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hghtwmqg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qtlnkezh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nbnllxws.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vnfwrbym.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sskfxuus.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rvavabgx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tppupejj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ngrniuqq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hftqzwjr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3rdptgryp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3saikeezi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxatzeub.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3offlkmju.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zgmwzuac.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ynkqqvrg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zvbahwfi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3noamwbzg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gifagiot.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ftjhbxuf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tqrozbdu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kagjswiu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tkwcootw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3cciwcehx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3uxwiwhas.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vawrxkzn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3plqurrxm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kejgrfit.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lpejbbxz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cheyaewx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ndouqstt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kvvfxfln.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gnaztqib.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3faeqgkqp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jlennneo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pxvfavhv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tvrjvyvz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yehmgnpw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lbitbgnp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xbnaxsco.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wjqpcpij.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xyqievor.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xtihlirr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ylxzkizp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oxudqriu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tofbwffc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3auggvrec.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rdlnbiph.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cmjwoftg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wctiqnvb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ntjjvoeo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hbnptunl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ndowvzfp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3klmvvzkq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gegfujdd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3alwnwdxb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dudccwwo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ohddjuvk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vnhwwfxc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mrkmfzfz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ozyfovnn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kydpjndi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xjzyqiei.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bxwxhuzd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ofjitoxy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3xigtngdw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ndxvannm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgggcpmz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kfpifbjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hrypxpaw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sxtmngef.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3avwaicto.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyyixfyx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmbhxfdz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fxhbhjhg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gqsncdjr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ilrmrzrg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ekbxcxgn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zqrhxemc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jisojlio.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ocehyssj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3lfzdoabw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thlwrgfg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxggvyko.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3sesmnhua.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rjyzsokb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3htygyczr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hpxgxioz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ivtxixsz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xqoiuaxn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kfknayhq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3opjmymzc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cfmcogyg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mjavgyee.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3musesmfw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3zcvzgotz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3acqeenmb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3blzpqitg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wsbhibba.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3eiuxkyis.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uebsnkyy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3plqjcelp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mmfindsg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3cbpzzxfm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdxhmrgb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wwnkfcon.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ykqdpnat.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fnwqwwco.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jmgtghdq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ssocaaux.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3oxygllhr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fwrblled.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3edvlnbhw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bigjqqxf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3asvchuwa.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3etfycead.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dyiqyfhd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yeeqjobj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wzocprgj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vjtpynhp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3sjdeysms.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3brsvwzir.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3slyygydp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zrpewaxb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3umlmdpsy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zvgqubrz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qpvaqpua.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vomkveve.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3raemtltg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cjvpwydv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3sjazkjoz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ladtdwnv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qjqdtzpd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mpjauofd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xadqxlwr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdmnlljy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eggjvgik.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3madhbkfk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3oazebbiw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3smsvjynh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3knvztfbe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqthplmq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3cxoekmbi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fxtbegga.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dyvwssyp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ehuxkwms.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hhwbtccw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvnwmapx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nmaxmkii.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvnwstch.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3aujkmkjv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tgjpyprn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rutroogp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rlysglfd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ngsluzmh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3tmdiiweq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mioxwdvw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dcluynjg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qululrws.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nhdsxrdj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3aburvltt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3trvpwlnb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3yxtzzzjg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cksczeux.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3saptjhix.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ohkrvkeg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vvmzaazk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rciobeme.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3oviztqoi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gpppxgvl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qqncnzle.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mvdexzko.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jrxigxqy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3branitnp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3nwrauodd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wvkhqtru.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3dmkyocjs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqlitbcp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3lnlhexbm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dhhwklpf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sddtuzvu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tafwnsal.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zojkpvrk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvyzimjk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mwsphxrd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ovfomhub.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3scpgadvb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujymlsuy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lfurxeej.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iqmzvbfm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pqtrttzi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdfnxwjh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3pxoypdoq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lqgyosqz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oeihlfpa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gvsrsxar.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3oeyjmslw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3icbmwhst.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3cshvyuqo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rrcfsrzp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dednzmgd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fkhzvupa.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3znijzvup.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kdxjgfuz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3diqmnlxj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3oabcgffk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3razhgxgb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vgfzbqfx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qddphiyi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3iavnqiov.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3uxnxbcxf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ajtyqqil.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3skxkmpcf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xixczbqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbndsrvc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3nidwardw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsmscngp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yoeahsyy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xtvalzoo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3esvdzvsw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ddiatudh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3srzgyjxx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ovttjxaz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jchcltan.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3iiqfgxvz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ichvngkp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cshmwrlm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3recgyhhb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bqtatwdq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rvdfvqkv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vocpfxio.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cqlvxhue.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ncrwkhvb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3eucnajtd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fnlczbrm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zgjbmdqs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ikdfarjf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3haaduhyd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xhabdixk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yczzkxqn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bzdikjbs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3umdjwmob.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3oxgiddym.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bfypyrbb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ivinpqyt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dkjucqru.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvvwfnrz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vpfkvwzj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qycjqaty.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vcjbnurx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3actlglwh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wzedtsdw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hvmjvclt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3smsgfplr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3emckhdax.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bkjomeaa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dnyqcisp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dgtcwhto.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bwkeziat.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tmcabvwd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ofhuqnie.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xyxvspel.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fqpqmujn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eryxevit.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iiqkydxr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jouqdqjo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ijhvsbtg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dawcayjz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpzeshrm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hqxwqans.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3flivwzgc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3icebjwzi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wpvmitfc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fmxwwvyw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bqvhrutc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gvkxpvtg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rdpubjfl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xhbwfcjg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dgqziicr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zooyelxx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lpejwfuo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jdwjaafu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3apfhfqvd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ktrachmn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zmffjget.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uemyxcem.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3skrilszj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nbmmzmmf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mfbsjgrn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zeuquqmz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ahzbngva.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3agcdeuba.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wpplzjrm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xiigfymh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3koqpnvbp.html


<!-- 参考信息 -->