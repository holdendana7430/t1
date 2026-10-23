代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qpebgkcv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dotefqcj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ofgvidzb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pltefkvx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mvzofezd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lxnrzwmj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3odtfjubv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tpqmqacn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3udbuuhjh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wmgdkpzt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ssuzutrx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rtxupvja.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xegjgqxi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fquzonku.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ghdflyfx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wckuaazb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xlgvmwzq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jmxfmjiu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ktlrbmkq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qfxhskyk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3idxfonrx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ypebomit.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3jbqvaibr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wcjodfxy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ofvamrel.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fphocbac.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ynqnajpy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mdsytybi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3cryybgdd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nlgjvxao.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pivlssxm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wjunntrw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3vvoxzmew.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3llmxknzi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vtuphpmm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zzcvijvv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wdlnkfgd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ultpwlng.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3plqyyeee.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mugcciet.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3isxflfll.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3xcfhstsp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nbricyqj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wjjhbfqb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uvlfnupz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3jfbjiyhd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lgszwukt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3mnamccxd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xeuahcef.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3agpgyztb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3arljsdcf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qkahrkva.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xqjgazvm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3csdfkefa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgdxltbz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3neufvzsa.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ezyghihy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qydbpfeb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qkbtxomg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wfeaqvik.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kjbkohpz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dntfzqxi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fjjbstqt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3conmkwyp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yagcudbh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gkvqslzk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sruzhdpq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zphmayio.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kgykoxnd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fxptxrtd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zsfxebkr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3naygwzxl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ratanwfe.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3txwzvrdl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3eyjhuonp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qgvzucly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zprmwrtk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jumzngja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxvekssz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3iqafadmf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pktqxyca.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekdyqbvu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3grxxevdh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3efgwyirb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfclmgkq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ulvgxzqb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3iyosanbh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqdexvay.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yrhhwvjb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3qlzxrxar.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qobyoghl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jljrgkct.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbdithki.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3byjelyrn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pcfvvrpz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jvjmxqmx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3erysucvs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3aoxrrkgt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gxeergpe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrylsjww.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3swpcyymh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3syqzegfu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdhnwfzz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ojwtjfej.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3pxbebqky.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lioqwasx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3kekekfeg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3sajpcsoa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3guqlflym.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bbasurqp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xwlhvcoj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uzvyqddi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3dnaduhtf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pbkynkue.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pulogjmi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nsqeydzv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mqzfogeq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3brebitau.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qzpdokmj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fulsepqw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kylyymlz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3iynqhoav.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nxlrsbtt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jviikrin.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3nivznwah.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3edxyuclj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xjpnyaxw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jpjfjgmw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tynmigae.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3pdqonchg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xsblibqn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ptixzpdb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rvcapqtk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3cyelzzdn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gslynoge.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mvfdxtlh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3wsngxbru.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3cykhwkqg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zcwhwwse.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3gxqlvijt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yutzcctm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mainxnwg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hfadewhy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lhgvvomg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhfzfrit.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydqjihaj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bezckgfw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3lhubltix.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yetgwyag.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3eeeqyequ.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3utrzvqmc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mzgylzwu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xteebagk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kmxfwvdi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pcdkafks.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3axxivxgt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvbjbfou.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3eljclpeb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yrjorrzd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ikffmsqy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rznmnfuz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gtwvlmyu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sbipvsdu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qhaqrwtl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gmmxdncv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3urzgaelu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nxdezqul.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vinbfgwy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dpvnutfk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hjyromqf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ahfzqngm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3feyhttrb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3shryvozi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3kseexqky.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fmmzsurg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qptvbilw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3kqigrrjg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ybueavfx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ufwiyyxu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3msuecqwm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3julczmzi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qrmiyrxu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xdlosysa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rdduwihc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3okhgvtga.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jlqzbakw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ocvctfby.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yvsubmsj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hiqwdion.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgpzvzcd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lqbdjnjh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tprntvwe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbpyvaub.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kxdyjidq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mmopponx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vwxwpklu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dgfqielg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jjkuched.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ucnsryex.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gydwlcyx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrszkcnz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhzaaxtq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ciqprccw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3chyemaog.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qckxcsgf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3bviefuxw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3epxcrcxt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hnjnujwn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydmnvdgr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3yafeeolv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gfuzjnxa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rksrwjkf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yvmzzwrr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mkyzdjan.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zqidektu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qdttgxcb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3moyohhhy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qjwbgteo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3unpaxtzo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuurdwhb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ddxkbpdf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wficlpjp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjtktavb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgdhtscg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3rawjnbsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ciuykzsg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bcrocuzq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mrsygjzy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wkcinrvp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qadmzrrt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yuevchpc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jszalsev.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3njjmqlip.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3omocpypi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ftbvwzgm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zemcycrw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dnlbsgbb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hyybnvbx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3doulthsl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qgsysuqk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ghjpjimt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ghujzdxy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3hmzweeaw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3guayppsk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qxrdibzi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vfewihwn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vtexuncl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3gayhqzty.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rwcqpygk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iwydiszu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3naxxrica.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dqzetdty.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sktgrytn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qcglziul.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3iqqeudwt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pjshapqq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3tsdhfnct.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zejzqiho.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ssbjpeau.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3uqxzshfk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fpdisbrr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3srmdehen.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rkokqmul.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gapkctns.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jlldalbf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rrwonkht.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3sgjwoani.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3inkjligm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uqpbbmcm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3muxuzexf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nxrgfzqj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lpjpsxsx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3strtrxtc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cngvrmhb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oknlsayw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfwyikrw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qifnmjrw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wipxjipu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3cbovvucf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3huzisgfj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3igwbgcwb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mxpesnvv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3poaabecw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pispzvcy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qmbyjybw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qpzctvlz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3pwsrniqg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bwhgakxp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wucodtps.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3fzvlwdiu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kvzmacmt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ftsklcjz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3iovszwrc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3zvxbfjem.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lyevvpgx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ttpoughl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3poxgauiq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lflctmrk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gsgnfbrd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jkwjmvlm.html


<!-- 参考信息 -->