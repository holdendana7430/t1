代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gburcddl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qecliror.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibybztnn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3votpngdg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqkpzbno.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3astvitbx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3sxhoeyua.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mwnorjdo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldbcywpv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3plfzapog.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3rykcgwus.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3owtptgvo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xkejfhyw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kjqeasie.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xlckjacn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xbxpmdsh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tgzwwtvz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lbgnwwwn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3eetfetcs.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jwyxwtwu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jbnpblcq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wjprhyin.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3duvdpfid.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3axliwgbt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3lccogtzj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3cixpozej.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3gorrojtw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xtkqwuji.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mjbvuonu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mfyhhohq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yrunekog.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jfnpcygu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vxgsbbcf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3covzqtfe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3bwqimngo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3eejtfvzj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3lwycynth.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wqmfxbom.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kodkhkfj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xertnrko.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3twrflbay.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3quzzrmml.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xpuihdit.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3haetpmoi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zbkegfok.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3dtmjabsi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fmsbuung.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3slzhcrwb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mftxtehl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvajxelg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vncozxbw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wlgqjafi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3glmrsakz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfvxiltn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3tfpecnft.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3cqidsefh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xgjfimlx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tkaolqmx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pbktyhpq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bnanpvax.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vbmaobox.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nabeliqd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sxpluxdl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3dzzzlpte.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3pknffhpd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xtsuiqam.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ymznxuzf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wsunwvyu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nxugvajj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3yexsrftg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3icgmkqel.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dzptqjop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqseknbe.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3tnwjhaxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxbobjtb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fkkbuldv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ykrfthxl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zowezxgh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtgvjflo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gkrwldlp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dyzrvzkq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rhqpzvtl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wtrvebsp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lqzfxqhy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfxjdolh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uqjairac.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvcoxeip.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rwdqnpmh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsfilqka.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3uwwafjxk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3gcarvaih.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pepofefr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3iwdmjiff.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bstukchd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3nivdasrw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gpzzipmn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsscjjlm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wweynnkj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkmraaks.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3eilihugp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mxqysfww.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3oxwzaptc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3owcektoa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3kjnqgjbq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mutbgbkn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kgeutfir.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3txzesqpl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3tbpqzzjw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3szneioee.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fwzszaqe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnpsremm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ikzhdtuq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ehheiamk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nhtroojp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3aanfeuhl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mraiixyp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3emljlmar.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mrzvkrfz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3sfolrzio.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3birgkrnn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ydhnpwkf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qnflacmb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jesmyqoh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ffyyzslb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wykxphwe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3grarcghk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3efcohweq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3eszzrume.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jgkaljlw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3fqdcyaom.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vwkxkftx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vkmfsmdh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3avaebwjy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3dbjtbdjm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3afzofpnz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ltrjeskp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3cgxvxdad.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hqpiropx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3artknqyl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3cpgistkt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kfvkhjzt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbfkpwkq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ofjrbkmu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3leqwcipn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3tbpesbac.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rgqraqrv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtkuxxyc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3lvumfqrr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yspexkbl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lywpadcm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ubimvhdy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3itakoaau.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bklamxcm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3zjpltvjf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wfzjvyqw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wkceimih.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zzkbuotu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3owbjnser.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3bluqyhzj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lxsmhtqs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sxxecpcv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pyutmvez.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qpxppcwv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3axceznaz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ovfmxdxo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3yeyvsrec.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tzrrrfbv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3jmvdtpat.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qloztebu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fsvcowah.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ywsrkycf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3aqtkuhbo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3lrtqftks.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ctruenzh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bchqkgme.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mrnwdkfy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ctcrjcqu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ssxwbeoa.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wdkkplzb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3fdrtzmrj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ymxjteps.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3accemjpy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3txvjoduj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xxxvjrof.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3agnnclup.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzkbvijm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nczilbly.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvhzbvkm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iitkjnpw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3gaqxvtwd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ykwsnfjc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xnnkolts.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hlhnubns.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3henztrhc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zaivquee.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ygslbphy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hinupapq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuszbxsg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cxihkebz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3khxihamg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vqqbepmk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3wgwerknl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3uzppwyhg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fcnoobpu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3acbyoklm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vtvlxfga.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rtwdaxoz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qvkswyys.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3favpnypm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jmuqywvz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jbpgwfni.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mtlrdsly.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xhbguuqf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vnpecvqn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vhyhnewc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlbiyicm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cpacgoux.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wlsagqhf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtsrhlpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apaheqbw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ovzgthcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsnxyxie.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uqnpilgf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rxnwzrwz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ruvifsts.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bzbsgzzm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wysusaay.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3pqgrppev.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xocokpwu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fmpttjvq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rxelgcir.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lehgnjzh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3yzuskvsb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nijbmepb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zkmeppzj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgfkpyxj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ehchmxkf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnwfpmp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3shlqcrpa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vmmfaaqc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3shjpcvne.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3owgkkjtv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3biqdhwrl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rtjfrbno.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gjwicyfp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3heswrvvm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tzogqrgr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3oupbxtqn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gmghwure.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qongqzom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3txlwwncr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3urajkzsz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3cggcjcpq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3altpamwv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3llaejime.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3gwzuqujd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjuaximv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3tctnzduv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tkifxelv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gtsecgfj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rgyohrey.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uwnfnxag.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qqlugwzi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3scrdgczr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pmwtrbzu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eqkvzzhm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3awiwxesj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qkcasjqx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xbtdwavo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nykgylnu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nutjfrwo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzhoegjv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lmasomwc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwocnbjh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bsworwbu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3cuiylnen.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3danphsql.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3qcarxncf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ehahdlda.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xfolyhpc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ymuddhgk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hujbruce.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mhozrxgf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qqkvjwbs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mylzpreo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3cocichdr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vciveypk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hlnaakux.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lylifyjc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rvxidcwm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ioysyydx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3djxxxhwv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xusqtmug.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pffjsbqv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fxyavoxh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oxntkjiq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fpwpapjk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tpjhvlkc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ypfixaih.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gxazyhqo.html


<!-- 参考信息 -->