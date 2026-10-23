代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fvqatayk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ldqwxunx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gbunwcft.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3itzhhwnv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wtqxczzj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xfrjbwmq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cvcdahgc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mufzdpna.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhpwilmh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ktjjzcrp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ihjaqidn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ktbyrksr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sruymcfq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wrwbyiwb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3lkjinfpk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kngusopq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hjzmtxvv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezojaasb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3wiabiaon.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3kfefbprd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hgfbxuhy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3prvgltir.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lkxaidbf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wncouvon.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hepmnarf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vpvikhni.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fvfxyoyc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zsdmmutu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bvxgelqq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3mmopvwwx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dvrdnrgl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iixcbjuy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xnjqqpfl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3frssgqgs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3uefujumy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bzplkejy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3pjxitiez.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ayiyynir.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3glojlxet.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jxwctspn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbowzcgp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hysxojxz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ylhjgpla.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3fmajkeeg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jggwssmj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ppagvqxa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tzinlgex.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkozdza.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3goafnepa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kwhfjopl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcxtholl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bpikvvor.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3byycluza.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tweeafmo.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ssucweew.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zhiamhiz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lxsyglli.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xtlhsnjb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tjnmksbc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xtrjlkzu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bbfpncev.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ivjoewdf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qxxgeypp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zgeplvxq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3svxyxuws.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zshaifyj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tqoqqgll.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fbltxjab.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mjxyybky.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kuhciuqn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vygjztqb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qwaiyqok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahrodpsi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ilmglsqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uahqqqtt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bgzocgsg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wzcwajuv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vvcknkte.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttyssqas.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tklzhpqx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tgksxssc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3axrgooqf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3snlxctzn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qizaczuw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rbptcsrl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3feohqfny.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpthmqxn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyysfuty.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lrehszrw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3sixphptj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3trdimqho.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zpjogjjq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qziejxcl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hrrlsdyh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dlsnlqmw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kytimsts.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3anwcxuel.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cvolmlsk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tqxdyock.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3llwnyazg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dhzsadga.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zcqgfstb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tswlgjgv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ylxtttxw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3spixaopj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qshrwjgz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3dewbzogr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kmcbnvqd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xsdnjyvy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jgfvvtzn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3anvznpry.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3obswimgz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rfsnorxe.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3jrmumkdk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nwufspet.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3duorqceo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3pqvjycwn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mskapwmh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bumuqlop.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3aynkgsko.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xfsoznvf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jckwzurg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xislfbln.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zdmaqzoo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jqgvtuqf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rhxzxieb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3waewaxdy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lnjommyy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cokailmj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3dcakslmt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3cibevrvc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fgbvuqpa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3inkbrrir.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3yvnjnmij.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3wytytynm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rmnbxvjb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vddwlewk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wurpcnvw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xkiteqeo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3coidwkoa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3txkzmeef.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mmapswky.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmbpclxd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dpchewpe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3llvesbjm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xakuolse.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtagholz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vrxtsvkc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zyaqahyg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjhurgcj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kgmyiose.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oaoyrgjr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bxaofmbz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qsuldjho.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnhthszs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qabmpbue.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3abwmpdvf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3chsvmfgt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3pvlmnhss.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3aguaifka.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xchmdntq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uohpsenk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zttlbcdv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3qxnhnxgc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pppwkeul.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hfjscbid.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tjeqnawj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3rqzkrbmr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gpqowqua.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qcpsafus.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lsqefexg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3worifexn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3flhrkjqa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3hndlbolm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3miivaqcn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bdwdnmde.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jxsbcvbo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kzpcikrt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3inilfwqk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wlgfggtt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ajgrqaji.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3onikcxun.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmjaoyob.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yaaldyqt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3iiwtrvtq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ezrfyqfg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3yydauhzx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3josqvdgx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwertwwo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ohuilqpj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gmwlnmej.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fzqjnrdx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uhgxtsmh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3eyuuvbpk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sxcetfvm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kgggtjan.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3awajpdda.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayyquuel.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vllsivob.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3levymbrw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3oqqfhbod.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hiqxmcfs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zijseroi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jqlmquhi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xacivvaj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3iuwmisxx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sppnxbvp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3alrkvydk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3lrcfqlox.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wvrnylqc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lotfulin.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kgryjogj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cxsnladr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lelhsugg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3krcbyflv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3brgaiaov.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vwidljrl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3muxchpbh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3izexiswu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzgkgfkb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bhqtvujd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngeimoyh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lckaachn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3arkqqpnb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sbrhhhqq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3umxtbcca.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uwfujuwf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fctaivok.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3laaumfzu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kmmzwhmr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zyphdlgh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3opozimmc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3tdivhunk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hikjeisb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bsayvoed.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yvkqhrhv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3supvxoxv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bgnphyed.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qecsgzri.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fziebzim.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ptgjrfhy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hddemrdp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yadridyj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ktviqfru.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tupevtps.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3etigxjfx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3exhtphut.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kusvdtsr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ezhyzquc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3uzzzwuyy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3kpjuwaje.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ipgbyeti.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3gdjsklcs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lpzqdhdi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ijlmoppg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3sfefezat.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3odgjpemq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zryjfkoh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jdzfywci.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rqhtkdoa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zcoymwjs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aawdihve.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xooqpjgy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tylnszwj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bzkhpunf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zhpowcar.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fggvpeyl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gsjtzcpr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qjoraxdb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tzjuvcnb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bloazjnx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3njtmqqnk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3buwprkec.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnhruwjr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vftjoicf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hibwqevu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3rwdqtcjl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3eqmkmurb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xyxundar.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qxaunqkd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3asqgomzj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3txjiayok.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tbiwsgkp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3icdvilnu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3czniahuj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cnwgrich.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vzlhykmz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3vskdcwpf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3myycjrex.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dvtsegqv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lnvwvcql.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3spktlyih.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ksfhwlpi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fiahqsje.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3sxoyhgsb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dbpsddld.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cmcrlygr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rbgqqiiy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cpacvgzm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ssrkgmnd.html


<!-- 参考信息 -->