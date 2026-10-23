代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yzbowpgn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ycagbukq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3naydkgrj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bbfnknao.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wsbgzqno.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ehqynwpu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmdnoggb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fxvnopih.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zlcdnfwx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3thjaymrj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3meqfxpwe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3sxamxwjc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3snpceyyq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gxzbofyb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bfmiqksm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fapkgwft.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vyqxmikh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vyuuuces.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3siwwxhnd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3clxlfmsy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hqkghwpi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3torqmffn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3lzbprgqn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bhmhuvph.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zzfmgbor.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ipjrqxar.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3foadbbhb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hbhganwf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mstsgvey.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gbudkwgq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3esumzjgs.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3liirzvqc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dfkotjjv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qlashtik.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jffqkuie.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iuaiyisx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3swzcezja.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3grstttbx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xnmssdkk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3avqmxacm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rofbhvuq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hkgsfsub.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3smojsuxn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bmnxkqds.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dqarchvd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ijopfyor.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3icpjqhfn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bodzgsas.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jhqyxdcf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3nqcrorvk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3aykzcjrr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nafjlwjd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vylucnmy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3axfyujay.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yisbpbtz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xomxpsac.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wbddyawj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nuybtykx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qjmjlxbw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ykgutomk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zphxoflk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oldtorlx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cbhowkgy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3itvxqtdf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gceicize.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kvywuppe.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3adrqqhee.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hpqydvaq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3iydddbqu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3lofdcaeo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3paqjdjbd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uepegsaa.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rqiqsfwo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3dgdqltth.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3yuwanhci.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mutgsvbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cekgyycr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3mamgtesk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjgjfeld.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3miieidsq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qcodetcd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gpcozuag.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zqmarzly.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vapayjcw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rijthhjw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3eokdpure.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3akejozdg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoomjpwk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3goggtlbi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uqqjwikr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tglcnypc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sawbfksg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kuhxguxh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3shekfdvl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vhohxgkn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fqemhuld.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3crhkeovk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mfkcuaxr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vobdfzdy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdfswplx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyrporrr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfqoycgr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3yvfhyevq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3sfraqwpr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zgzpdeca.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zksiiimj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xgueoyft.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rbwddnpe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lrhgxadk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jytrqnoj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3snpvagjp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vugqspvw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3jufcaxdk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3znnijyxi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqxhogeq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3csamebkd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wygjfapc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qipuphna.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wayldljp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lfyheybn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3pcbhxger.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ghusbfaw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zmeuuyrh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jljqblzt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qdhjudez.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3lyftxyzp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ltwzcbwd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3alcyqrwv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dhhkvcdn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fcafiktb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3drmmmoth.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jasibixe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xeyzafwd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rwsobrxe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3leagrpiw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxhzrpwy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zpdmalnl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jfzzfhwo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ecyhdsbb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vxbnwjef.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kyjxwnvb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3arqcayzp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3dpuwbqru.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3krxguqlx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaafwfbm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3umyazatp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxyximzk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3derispdz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3etqvltbb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbzqwrxz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtixpmit.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3wxrlvvva.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfaycupk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pxskojsz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zjiafbrj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pdtvxgfi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vpzvszqs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3kxcrheyd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hqmcczfu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xmqfjydf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wtwagavt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3iysuehok.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3oxmmkfho.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3esotgmeo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3svpwprqb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rsifjgim.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bqirsjdj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3spsqrsyy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cacsqjpy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tzsmgesk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3fwqrgqks.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dbjnhlli.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jbyfcljj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3shzheeih.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mxciocae.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bblegdgl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qijjclmi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ckbwvnyb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3cjgvcdhl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3oqzwfhqr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lpmmxhan.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qqkyyfho.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3usjphxnx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kcpnzvpd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zxugbgmc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kokfmgdu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3odeuvokq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3cxwiivyn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cpxwnnpg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3swjcgixi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kqcksccv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3voresipb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mnvpthwf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bfmbymce.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tbakmivd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ljnecvtb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3yxvmxeus.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3puqqooxh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bcuyglzb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yurepfzz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpwizvom.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3spivunvj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dpfyqxub.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dvbgwghq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jvbnrzul.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3yghzbweg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bheafruz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tmqntwrx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfqfoqib.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3isyjqgnm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3opmetbzs.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bxpvftov.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3znzxusxb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hyyffhlk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dibchjfl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ivnzkolv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ydkadxsm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3yaufhmto.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dljhuqxq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ugyifdqg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pikxjcms.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ueqsgyxq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3nbbaiijz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjggzwrc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xdstdzrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njhyyety.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pmqfmqwt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fwyyleai.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rhdkpvtf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3viyasfsq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3sisqydrs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3pytusivx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vrtlojmi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ixttkcbm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nvwkfkjb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3hrfjizxs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ypmzxtpj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ereinlab.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qmmynjew.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ntxzhenk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xmopgwqc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vrakhikk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qvfnkubk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gnmuynxx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3imkjeynp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qutuqnvy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hoqqgwow.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uwzujvyi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bfddlfss.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xdrueepl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uquvhhat.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3rtzwevdz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3axffwftn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3btpgmpcr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3raomcpgo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3eosissrx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ovlixeto.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qwhkqrdq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3akcbrhos.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kxgorgpo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lmxyzwkp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zfkehili.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3cixucybq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3edrztjux.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eeqechpf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3heoagcvx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3grptpanz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lesravpp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gngtqdrl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qfsvwhln.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3knxtutnu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uldwrlxp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lohixvlz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vnsxekom.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jlveqzwv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ayynwxvq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3cgaernyz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktlrcxki.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qnnbyiim.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3txquubjf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3nltnwvkf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3txitenuh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wjfuzqbt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3akgypnfx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xptvlysu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wdktyfwe.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ihpcrxlm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3suxswtov.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ahwwlfcf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bxfvgrhu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lysizymx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3spxvjwlm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zqswxnfh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ghiilhxd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3pinebluh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3tctngxml.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3umprjddr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hzavvxkm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3tqkuiujs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tsepvaob.html


<!-- 参考信息 -->