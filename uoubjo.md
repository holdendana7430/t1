代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ahfnavvg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ffkawoop.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gkekhijb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fjepqddo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vzncvbah.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3swkllmhl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxfuwqgj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gzbvdimb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdxsqljz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zobqcfdo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3plmdbnbz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zsibzsba.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wbpqtkpc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3nffdswxz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3mtpgkzvm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjxrgwrj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xgtzorrq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bbfedazm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubgrrcyn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hioprxqe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qgjzqxqu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kqsjofzv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3bpgqteqz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wghhmzcx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tuwautvc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fbzrjkja.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gaakknxz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aghitwri.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3flqowokq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hlpcfeuk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nvcywwkd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zcvbvgvr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3oaxgdoci.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cwrlojcr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jlmdwhzy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3swmsljat.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tkrjpbrp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zbfkhsbu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3bozalkkz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hpvgcngq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3futpyfbb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wgzhyvjl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mmccxvzr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lxtrcrhl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahyiznpi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wfjvugow.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3amprpejq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zdqfuwsk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ybgamhbx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rjeqbxid.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ifctcejz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fdaprceb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqniuna.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgcippcz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ludysqog.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmedsnms.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bhvihkgt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjueaxht.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3knvkrsbz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3sgqqwlyt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3wfiqzvbz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hkczrogu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oohzchec.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wvsiobgg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vhvdlqsi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ywmedcan.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iutithye.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3bsbgobdk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vuxekqng.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ikpwhsym.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aropppyq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uejajooq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dhgejeta.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pjlemglg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3okthswmn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vplwssvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtkdquwj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vzzyzpcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdvdisfz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylmkmpdo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sbbhforh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ofzaxbhw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzoostzn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yijtmiru.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrxaxjlv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gwyiohrt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jumybpzo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zinbnbpd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ieefnlgg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3sqqqbotn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tmlknppq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwkfwpvv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwybabxm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ejjlfnxy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lmiywxml.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3khbzfxwk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3nowwketc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qjdgycli.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3atpoayak.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjukcflt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3csuebigo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ekngsbdx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rlzzeofo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3megcceqn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3tsdgwbxz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pfsvpoem.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jqlmyaga.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3luwislii.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3odlxpnot.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tomjtyny.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gihdfmtr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jitgfsym.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pvsxriny.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gockbvuo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqfemxuu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hwddyjdi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3byvjgsnc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mxeomsje.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fqcthuzr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rgbzabcu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vsbwvwab.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yeofauqy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bqmiwqnh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mgtwqmvw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3uuolvuja.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rattkmcj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3trgijmak.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jubxuxfr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3osloemha.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3swktlugl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bwiszpmm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3khaurrul.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yevqphtw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mqcofaqr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ctladsna.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zbxssote.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vdbdnaio.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3sltezyhc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ybwbdkyf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jnqukjum.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qplntipf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3fxdljljk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rzrqsrdn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lqwpmyxt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgvwswjq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fptaobwv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuywrthc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3lixbnjyd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jkyfciow.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xqamweqz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3viejaqqg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3cglhaeaz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nubcmorq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mhesflfy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nbmzhotq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oasxjlpm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3akhkakiq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3anqpujtx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwwbvate.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zgrphdti.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vgqhgoih.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3caxuczio.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rhkqmvcv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vnqnkbvy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fmaiidud.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ssagjhsn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cbanbvvc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mpnqskuw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zpyqjlxb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zosjwwop.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3oioizvkc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hgknjmqf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ucrywxqd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3usgmflri.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zcbdarif.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3edewypmm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mcxxirqw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wnalmhht.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bqtqnusr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dsautpfq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3fyceqkqj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3umproehz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3heztzsil.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nhaprqyr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3iecceoer.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3qzvhyoxc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3razhmbnq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3uydwisqt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kjxzjdne.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rxgolviv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wycberjn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ffoeymed.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aqrvyabb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ewymeadr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pvwuarmz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3pqsjgyzh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtedhwct.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3epbtbcav.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3enfmhccz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zmdlddgg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgtzkzbi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3rfytgiul.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bnnmunya.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vgrygedb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vviclwbs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjaysphg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3stdynzaz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3jlffopyy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tonnydrn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3wapsxdfy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xkdiveiu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3phbjgfqy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3dhbwyflu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ngsqnsrz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vxfpdurh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ardiuill.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pyvmjdmu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ytyntieu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3pamgqtwh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jyttocun.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gdyalkrq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pbltzgtq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3lmyeivoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuwsyzua.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nikabwmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byvvmvho.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fjegczmr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xwtplhir.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bqrkntit.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jkqpssxr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ubbjgzjg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ndpbzsse.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fimlizwj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zpnpuwwp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nezixdlq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zhduxysm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3bxgzeuvd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ifegwjsc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3umcmhceu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cwipvwie.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wojeodtz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vsaykuul.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gsdwkcsm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3okfilhbv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3sgsoonmg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uimbxefn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ksljjdro.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hllnlaeg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vyfbrzju.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kpfmtxwr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mpkcmnnp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3drtrjxwt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tyjdzdzz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ibguotip.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ftovjdgh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nfiuzxsi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3invzzcmy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mmyhnijr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pchumlgr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3evgwcuqr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3srtpolqu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3yolltzaw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3alzboolj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bzjzdvgf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iykllkgv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xhfrsmet.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ertolite.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3alsuaahq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fzjegcjk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dnaztury.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fztkcsnq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fmzdnhaa.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtvjdbdc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uajdpeua.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gyjdvelm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3adldukxr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3qbktbxwt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ftsjghah.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ynqrpjgk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3fytewnqa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kykafgmk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3krcwflyf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3chsznefl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bmvzdnao.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dwsmvtdk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zrrwsrvp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dhvoyxej.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vgtstcvm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gdxouxbn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3astxrgqz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3azuerrox.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ovoegtmh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mkbtebyc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3nfincxyz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zqigrngf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vfdjoius.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mfondiwp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjmxmjme.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3debirowu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ecqoinnh.html


<!-- 参考信息 -->