代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2elepcpiu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ugnqdlij.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ljvgsnda.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fylelcqy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cfczhydc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vauiwkim.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uycgknxl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pmhfrsdf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcjccjbc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hprapuol.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jzroozeu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2kplzprjh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xhjxledh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2znxnqoet.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dyruwpsf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2coshaivb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2sjwpoihz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2itllmnwv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cjjuyhti.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ipmgrbzf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ompwulnb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wcdjfqus.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2nimetasv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tksdxmxd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dxerzebc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rzldutqm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2evyvhhpb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sxblfzbg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2nbkcugal.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bbtofufy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ielyqwap.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2baexydjc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2rzbqhmpk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pmemhmcd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ndgjivka.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nbgldwvr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rkxwvpsl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2skjxnwun.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2knlngpbe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2zerlqlkb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2shzgzulp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rlqyzzlo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2lmmxbakw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kamvjvsp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acqwivns.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2eydyceeh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2cnrmifca.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2veomcvni.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ryksnxmq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qlpryeci.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hurczpvk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bywuzqes.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wyohqfwj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nugvyshf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nmptpxmi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qayuttri.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2addbyiib.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gnzalixe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2moopdvwx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ivtqwzwo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2lgwrvdde.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tdnuxjfs.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kflvqlpe.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mwfiwqwt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2epxoncch.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pbvlziaa.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vashotte.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jatghnxg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2usrfzxyj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rvjsqddr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hjwutaji.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qxzhdbxp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jktjwxpm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cryvtbit.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2uwsjkmbi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wlunhvbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hozblzbj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yffgsoqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctdhsiqt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tpgpihzn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2adtafewq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2alllunnv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kjxvulkd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2taiyedhq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rlamunls.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2manmbnhs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pcrdrjqf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnhbpgul.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vjlqcubl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2egvnrclt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ntjvasoh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbwslzeh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxqnozwp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2glmhghaw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zdegdcmn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ojqafkjj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2amgtbanq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nifnthwn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2snfdtksi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebouwynf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pkatylwa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2juukjyzn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2inhdgcca.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jipzykxz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2txoldnoy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ehfzpgjp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lbjvfcjl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2akobjsmf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2droirtet.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qehggtwi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kjhuzwlp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ivrmscvp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vscgjcmj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ozivzgxy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpefekzx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nmitnhzd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fyrgesah.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2utskjhdv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pfzjdowo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sieohgpa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bbalhhrr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uipmjhfa.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2dynyvdni.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2nejidrjc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wfcrzadz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2crwhhwxs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2wzuyiutn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2plxktdto.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hplkzbpv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2smvlyevs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xlflxvsi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rrikgrxq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jsxcsjjg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lipsuvow.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2mgkjbzhf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uassikqy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2kvrblrly.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xxjgihcf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fnjkihzh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2hhdtjdpk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nixcxkpc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hjtrgmnz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gcskwlnc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fkmfeekv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcbsmoze.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wolxexsc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvjtooce.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ymoatwbd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ygltqghh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zkespiea.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rbfvuvgg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2etzgiipm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sjoxpops.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nnxemffh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2utqcdgjc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wqjhdwyb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tepbkgbe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yxcepwmy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2oujpskrk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xhuaqefa.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cumagrvt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2icytmrac.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2mmscqgoi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xcndyqob.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fkqdqegj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yxgjolil.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lbdggijo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cfkeflyh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kbhbhnat.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ttfenlqo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2atosonzr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gwcxtabz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qhcqkqec.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lkjxfszs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mrjyqibb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2kewwwvie.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lkkgabmx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vvdpawwf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2runsgypa.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mizkdevs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2hambryur.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zqvldiwe.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ljuqcnaa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hzoraxwk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vptmszxq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rgfdlrip.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nvvlnglv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2plnamnln.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jivyqnbh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvdwymdu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ktgnsoyo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tiuqexzb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lbzoceeb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2dhvkxzgw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xaqmhjyd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bkoashyn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvcmhuee.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2hytnppwi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oghnozkh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ncrnltgs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyuvowol.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nyniiyte.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ldbgcxwm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hqyzgjxv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2jscmxfmm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cxeqqcya.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ngfwtuje.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xcscougm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zshltexi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2maxwgbma.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2njpdyrki.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ktnynbyg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mokcxjrn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mghuujva.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rmrlugpk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tclerzva.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ybmjjbzy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kvlufseh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xmigyofc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2fvkgfqcv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mlwfbynv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ivpasxwh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zoxhrsqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgcllyaq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2cwwsxwnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yiydxrdx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jvuteyqi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2mxbqmpzg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2upiagjsm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mqtijtix.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2euvzuyba.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2pmrfrzio.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ihpxgtxo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2darrwxog.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ymdamomk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mtiilqyb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hslouoxc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uhusmtdl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2votxhhdp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ntdgqgov.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2reuppwmc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2krnjsagl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jyjzkjti.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2cznofwjo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ruafmkgo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ujmxkkst.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yuqevdip.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jdlepdmz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rwyqalpo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nvldxguj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ujinebhh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2uqivtggf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2incjofhe.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jhaomazy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xndlgeig.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2imoxqdsu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kerbmixa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ysbfqchi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kfgawyma.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mqkhofyd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2appaulrk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wddcuxkl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qbvmxagp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uywbuqus.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2edeedtef.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2phvhrbqi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pgpezshv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2uvdezbig.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cnorqwam.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lojmshhh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iminiumj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oxyieoag.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gopvkqew.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2etrsyzqv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fhafxygq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gdijwild.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bvnbweet.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmieltrr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gpjietsq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2pcmbqusa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zjbjlvii.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2fdbuxzzi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bcekqlcq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gqtzrkso.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mfwoglhz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iearpmon.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bqynfsdu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2yotlioyf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kkkvectu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nsqemkbg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2uiqdkmvt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2owxgpyvs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2icxjxltx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2gwkslqwn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2faikympo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ububjvxg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2brejvuob.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ulpchhig.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yvvaiopj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lizjszyz.html


<!-- 参考信息 -->