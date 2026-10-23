代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cdtsndtw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kbmzitpp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xijsaruv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pecvevos.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gmmszoum.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ioixyqju.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjlkuwgo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3laogxhhi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwtuttfq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsfeaqpt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ruwhfrde.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hksmddcv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lryanaug.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vekcjkyg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rbmxzhxa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvoewaet.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ocmhdeov.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sbmtkqik.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fmdqenss.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gzxqdcou.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yxatlwuh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3rbzrkyhx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3uynawquv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3hwaiqxhx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gxycwtsr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kizfhjdv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ochbzqgh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xjffvxxq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bdttwvge.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3byursmry.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wbbprouv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bkdwrhhn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3chavpvkv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3euoefilz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rxgkwajo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ojcilpbg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cbbyghpq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3neuvetmc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3oqwnevxk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ejayelxm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3spsjwwiv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3adbwbikg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tkybzaiz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3evijokzt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvexigv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3tyosmftf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3llwijoip.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3twyahpfs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ipqemvhr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3iiwfnbae.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tomrcnny.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3pvmgqgle.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rwqjnzox.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kinwgyiu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yngomuyv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gvjjfjwg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xzpthquu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3okaqfzwp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3twkapfei.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pwcqofpp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3umcczghl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vaaljqvf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sbfrbwww.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uylkvhta.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3omoyexas.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hfneyfbh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gawpnsul.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gyvuukmh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3izylqdpw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3niqqqzzz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3esglwaax.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bomjdwpt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sgkqhxsx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kddbqznf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ilknyxfl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rldgagob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgzacmrt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bbonzyik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exowwxje.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cmoitlhw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nrkzgwwu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ztjtzfff.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3heqrpevo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sadgkiam.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgtbcbna.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3oydoujig.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3sgithset.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qzhuylko.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3olsyzbop.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3rwscvrxm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qexrlsuk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvoaydw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kkzmvvsa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vmhlthrr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hujkkbzr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zutkxucw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lzdsvjqz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3aidcxozd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3getcylms.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xmbwoodb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lfkejpbc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtiimjen.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3olbcwwyu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rpqgxmph.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kphwppkg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3rctajwdn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vaphvplv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jquvugtq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gnetmxdc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cwrlyoqx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nhsubtkk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3tqtnonbn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hedcyqik.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3myomprdy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nxxttupl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3duekzboe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hufhgxuk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ntuiuxur.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cpsoyqkh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3huekkoxq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rcxjhjfq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jaczdtnt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3amvhbzyq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ggsuojkf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3kufpcfum.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3htheeklt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3hxnmvipc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ryqyhgez.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pakdbizb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ljvadssi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bgyumwaw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3icymwfsq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kegcbkqp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mlgctqay.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdzqwyg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jrnlfjbl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lfmwhjha.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qolfijxc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3mxeorjpo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3gpklsglw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vwoshije.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3makhkhyh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3adiliioa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dmnilsme.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3dnzvwgom.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcstgldq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekidpeau.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3myzzfuqj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3agdgmoqq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3cetwdwai.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uopxaiaf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dbxqjlhi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zqakglno.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tfdaulqe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xgtuzbml.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ytwkkahc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aydjraxv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ktsupeqf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmvyavca.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sbqnlhfz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wtqathga.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kzxhbiqj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fbpynojq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3kqpbnojk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3dieypfwo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3doicmnjq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nvklstvp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cwrouaye.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jscwtltl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kcromvza.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3sxewzocu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3sgkhwyxm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kgmqbgwz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xphvcmkg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jbcpexdk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vbkeuetc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wocjqdng.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ayjiqwni.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3cazrwlue.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3evaetnuc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3amiohyet.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uvfmqndh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3acolwhxx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3zktsalcj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3yhvtdsiw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3toigcwub.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zjrhrgvp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kqnyxtch.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hoqytedv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ekkjscoo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ozwxaarx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xtomlkdg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gojwnmko.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3kqhymdwb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3kisafchy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bwbwrbsc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3umixgyug.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3uyzzuoub.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dnxvawfn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pgxlvihx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3otbouujd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfwdcgtz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mzdliumb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lofibpxy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gcwovbfk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqczdppg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vsazrmxq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3etdxcunz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tbajcjck.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qbmbumyx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wgbpcgku.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3stubvzst.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3gcxsuobn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nzgzxvqs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ktczcdhq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kndnsaje.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3puzigxsy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3gdjxzxkx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3hzwkatvp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmbejtii.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3epkeeysw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gcdxsrbo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bycpjnsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tiaugdvw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pgsjcyaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqjwobsj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cxcbosxz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dmbgqilh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wryxzadp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jcgseuhv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3attwueiq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xjghrjzq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cxvgyxnv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3cxbfbpui.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ybbddxrc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bbqgcuys.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jynknivd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3yhyjedjj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hsrbjuyo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3frabunrc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3osqmwyug.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fulyfisc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3chphzvqq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pjpludnz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jrolfecf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ipwhjkuh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ijrmkjte.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3omdmflkj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nnmjsfso.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vomsloje.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hbxsfyup.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3myqqgoce.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tpbvlnmm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vmaauwco.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wjpzhdrh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3tfqytzik.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3yktyjwyz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ychybhas.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qlptampk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3xexdsyri.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fjkojqeh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ashvnvlc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3crvrffos.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tqeguddl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rrfwxttj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xjlxabkf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3oaaftbed.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ugiftuxz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tsmagokd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hmwjaajr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oexdxkpt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xpnqdnpo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3twfwfcqe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lyiftcua.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3emovqfos.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dljhumkz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3nrzxlvsx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gokxusay.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nvvpvzyv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bhosshru.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ozcakdsf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hmctcgky.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rkygjlbe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ymfcvnrf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hwjsjtwg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kgvatpny.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kpzelnom.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3lfuajqav.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cniflvpl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dxevcfme.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yecnbkit.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3vamlebpv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zrzxvbcf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3pmlzozkv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tdmwobuz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3iiohuhkk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rswivjya.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mvrtgwsw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mogcptgm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jmcrdalg.html


<!-- 参考信息 -->