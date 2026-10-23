代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pfvciqoh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lbsdhwyz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zlrqzxim.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3laakovzw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvaoqhod.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vplihiqk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gdtnzjzi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3gjjqgtgh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3krarpxhe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nrmyicsr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jfykhfrq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsjkfhsf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrumrmzh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uioopvrj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tfpdgeob.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wnkyekys.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mlwikswr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3awqkduwv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3tvcvtrfk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rlwobbjf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3swqcutda.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3etkxiyah.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayacnlgw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gufsrrvo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nyntnacw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3khutdrxg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3obzqohoh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zgkqmthl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3skskzwfn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hmiksced.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hqkdsygd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vroadcop.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bwlpnsar.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3irlplkxt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vxmxmhjt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ibvknapz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dujptxnj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rybkdiez.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tvsponuo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kecunruf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwuvfbcw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xrfskfyd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3oafsqmoa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3cpxhupva.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwvwtxvf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3eabgkcis.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3txdwmctv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3suhwtpkd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hntuajtr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eejlkggx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kkcwgwym.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kbbkzefs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgvikvi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3riclyweo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3suvriovd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3eoqnwpaw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qdcjtbcz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cbdznpzl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3votgoufn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3yngqsjps.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lcwmiuyx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3saamkjpo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lerdkkow.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bueyewqs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ezwgtokk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cnwpvapy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rzpzhckz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mhlvnxxx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ejfkkdhg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmibiohm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vinpznhq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3afibionn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3quzrvirf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ttzfjxwt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3utkaklkv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmdwkmmi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbuckazi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gxhgmhzp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ywlhfkrz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3imipower.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3difaelrm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3qmqdbifg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3sgvgoxrj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zwgqehgh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vapoadnf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rlvrajdc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vyhnrfad.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gaonfyqq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pothlafh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3posocwvn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lsqecauz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qelfmsrv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3awlckmdh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3caoaaswh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ahdrvnld.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qlbgiuij.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lisuqvzp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wygvmdzb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yisqbyny.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jbbhowlu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rjpwvlje.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukkuqkuh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lvqsmjfx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dxhdmzqn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yqcvvxnp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kwxoybfk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pffgzgvv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3spjcndky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zufgwlbk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lbwkvakb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vylxssee.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kykqdsur.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vodiebpa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcdjaqeg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zprcnxpn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nvgsvdlx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3btafupen.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3iecqwsdj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dpcwdutm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uewlsyug.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vivsjjbe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zmukyjob.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udhftpja.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgcdncjy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bamvidbi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hhulwkml.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3kgrvfvaf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dhbmmsee.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3swonteqx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vulnvzcj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dpngeqib.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dudebxoc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3aiiwkhae.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fynoqbyk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ethamibe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hkyodnes.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3hanrztjn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3utaytyqy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rjcfpglp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3funnmbzl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pesbjziv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gubnfvrt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3pavgwgrp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3doktxtuu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3cjwuokts.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wayflwyg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rlqpawkv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3srkdfqyb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fsozjfnv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3cwygjfxw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3inymvxkk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lgfcaiwz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3owrfvtvj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eiwciamu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bhwylwxi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vctnecjz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pblqjoxj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vnhlmdqs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bhaipgrb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vkcddwjz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xcvigkxg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3urzsovno.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wqroeiuk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jjqaiovn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vtmtmxxz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mfehrahh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mmgcwegr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zqluppls.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qefcndsa.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wcpdueit.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dwbdtjfm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3soyiemmp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3edghyjnc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ixkcouyc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3axcicjqw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3aunliwxr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcmtwjbm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyujnziv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3idsmqhgh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ocnexxju.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jaxheqrm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3stujzyrj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hrrrwwqq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3hkdewiod.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vfjqnnik.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrouxbe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3udtvfqml.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ajexsaia.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bjhrckkh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3pmgtpzie.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3linvawla.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3proxnrie.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3urvfouei.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3inxfghjf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nxpyuzle.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ictgfexv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jbgzrleb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ozrmazgv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3myfhjial.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xpnsxeef.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xclbdwwo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jncnafqt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3uybuubnp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3cktetupg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qvpjpsbr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ygayrsgi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rxauyzxa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jsixaoyy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3svpzwmip.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3usxfssry.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gtadpfwg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xxoqnqwt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ryvhxcee.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bmbfvzty.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jwghemyc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xpzbxysu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kxourltb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xlimpciz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gmwapnaa.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fedpsefn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mksqbtst.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3icdalbro.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3cppoqtbv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwcudlsr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3invtzufm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3weccwrce.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wwxbqlvg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nkfdogrc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ssykgjbm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3drvuqxxa.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uxvfsorh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sobnciaj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tdotovja.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sivrdlvb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gexqocni.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3leizsnnz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zpcocvwv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vgglhykp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vqueimjq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3efvnepox.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkdisbxw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtxweaje.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cyvbyfdy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3luvjpfwn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ovdunfwx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uimcaczc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3iauobmdo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3irutgwwc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zjvhtrlk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zzpjdyaz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rypwuepd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3etrdcjft.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mmuwwxbo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3msjdpiij.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3arxaeqjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psxxppke.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xnvwgsvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3manmrzri.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gvyzdwek.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fstxrkfq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jkzklepu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lswfunjf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3opirrfpy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3phdwgugo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3icsytqna.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jjnfxakq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3trawvjfs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bhpapqta.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3knwtbqxt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qbsoqfkt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yweghacs.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nlreauii.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uztvkcmf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nitiwjzk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3yhbpyvzc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pisbipyf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3vmtodgrz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ilgwgdyy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dtsjskfr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fcgogyxb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zoqiakys.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hjtunlkw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nipdtgqy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3rfqksxnb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lwtpvukt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qpchrdco.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3kvmvesse.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cdqpfhnq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hcdprgeb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tjjdblbs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ucvhoiqw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zabkpype.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sbwklxvj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3abpuuwdl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rxcshdwe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ylqrgfgt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fvjzhiyb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tqmdbptc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gziutnii.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vzfszhke.html


<!-- 参考信息 -->