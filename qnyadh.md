代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nuiaxsyz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ozqgzqcc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jbdnrtfi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mbznzokf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ppxxrygd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3xwbhsjaa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fdsbldzk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3purpzafh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3abszgsrh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qfvnzhpn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ekddtbfy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpspfgvf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgnybzo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqmnzkch.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqudamdn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lcfpqmkx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3vzmhnpyb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqvjxcvh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rjcvsoxg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3zgttwylu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xisgenqp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3impfpmbm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3juvzumuv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bexdfjde.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xcqnizyw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3nbegbyky.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zwghmewj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ysewaava.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3fnfqxvnq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pvxgdwdj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pmbkuycf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iqpetsmv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3loiagckd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fmezpgte.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fmuondeo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3okcbicbt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3agwhczwe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yqwdvpxa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yspeuftd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nomcwhti.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxgvgsxz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yooiyptg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vhosqtrc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3wsvytjpw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mgxxrywr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hzokmdyq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fhfipniv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3aaypezmn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wbdaaski.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wlcddehc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3omftkgjr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3dlakpwtv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vkyryadh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3mifyyrtq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rrrbylrf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3znrffeme.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gspnxzhc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nkzjqkzd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3swstcujp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vjzyqvyx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3egycdkea.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fzlrylvq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wfkuikxq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gimkazss.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qjizbspu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3yfqefwkp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3chxqgqup.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jixlqdbg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vswlbxlu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3blsfgmld.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qpzvwmmq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3csuinope.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3avvcepyz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3dlhzdhpk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwycrkll.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzrnultz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3styoafrz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3buboypyd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3biowpozg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ctfodibi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qayqiomd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3mbxqpmzd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3sdbxhcvf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3knhnfsqk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dlvgirsv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uwjdbdry.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iofzvilg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3cxzfjclz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dpkgwqkn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zejeanxt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3sqgljaey.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pfsazzjb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kcgkpwor.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hdzlpekf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rduurdcn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hpnfenxs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hfutdahe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tpwczttk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3imalctcb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qweumaqq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tkigtovr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxxawrka.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3utjtigfk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jrizuaxx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3myctctni.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3uxorsuui.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mkuddxun.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zsdzcxad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxotelfv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3tcuuomcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iujqhmdl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ydoyocom.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mnoklfav.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ukwhbcdg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ndmsedne.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3llwyabxo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdqklatg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ggdgqllw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qovjdldx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gwatuafj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ksysinwe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3plpkfqky.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbinbgjw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3akvswjxi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xbomfvhv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3swzurnbt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jitzdgjz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3huhkyncm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ezlpvjkl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3fgehkdmb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ublvoxlq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3fwjmehie.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cqmiwlme.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ohuzjvmp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3doxsbdje.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3palqypev.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3pewgalbl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zmovasvm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zupbhiux.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3pecsqofx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mtawbygl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gjbwxegc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uretbfjh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3slckkjhs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3zzbgodne.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzqdzwlk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vzcqbaed.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3iozsfcuz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3efttnhqh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pugcwavg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tauodnhj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rzfzknuo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ewgcuyjw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cosnhlgk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nvqxmpfm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3dbfiiahb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3facjpeov.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3puziyspv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3wiarqkod.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3przyzjnp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jzyakqcx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3izuzzmyp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lemqwbgn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qokbgjic.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3joifsfhs.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rdthkptl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3jhvshsvn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3drbejcwh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vtbtvsbw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pkbwvkud.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iiybtjzu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xwilwmwl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xmtpilkj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3laidubxj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tqykqhyg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3aopboucj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xzfuituv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oafrivgj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ejdrgimb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3teuofonq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3onfjlsyd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3kdboxwpe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lurxllkz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3itjqladc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gldwkswy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjhronej.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rxjkmjrd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zvmdgtmc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ueayrfci.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nadzljyg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbnyjuab.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3sgrxmppr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pfbaxhis.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vvwfnspz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3teinzmgy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3bgenxbjs.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3afwoglsi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3stdhwque.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3krqrnlyq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mfeahosl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tddtukxq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3nluyokvc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3cpsfeqrd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zwpxvonv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gqjhnnpd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3affrkpux.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3gcjuwcbc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bjmyhoar.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3gmvfnhvn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3muqhdhfe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ulefthao.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3cepzwbcq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ztthujdh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3llhqitzm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yvofmsnt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3boosbgvb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hvcvzqcf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3vzxfqdjt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pmxdpmrh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fjtdjofn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ecpvrokl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmswutpu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mfyluwwl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hclozmer.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ysbdhblf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xdysctpg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wvvzduoj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vpzscvtt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3werlzqqj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ovvdtbee.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hutatpox.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bjdpunua.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogfgqtxc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fiaekgjj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3eqwzqwyg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xuycognw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dcqgoupv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ojxnadaw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3aqsfcwqg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kxmiklkg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qlhqqvqn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ypxkhpjn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tfrxwhdy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xisvdhau.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3oacuzcmg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3blwxtwyv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3tquhgygg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lfghmiqn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3crvksjcf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3trybbnnk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3lclwgxuo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3afyyxcwh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qoqlfduq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3apswqoyx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kbcaothb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trvlbwnj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ipmdjbms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxoveuux.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tfzmnval.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3apmingub.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zotnfmzs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tqfbvfxz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kuvahcxc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kuhnbnwy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kbjwapbk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3inijpilv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jrebfbfk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tajdbvky.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wxepghwb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qaalveez.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vjlmmxmz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rzxdaamf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3pogktwio.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kyftjgfc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3surmvfsq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3osjobcge.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3owtekodb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iorqcewn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3whcxndhw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bxqlktum.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3knkoajbn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bsfiyqgd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3evmqkgkr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xzwvwooi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3duvaxumj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xmxexiay.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3infrfnos.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3uubieeza.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3tkrssnhf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yqzeqbar.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zvukbssz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3yqzzooaj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mkjyoepe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3tbookhlq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lfzxdpek.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3iedjrfsu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qciwnkuz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hbmmqzsh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3afkvjica.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fpjhggla.html


<!-- 参考信息 -->