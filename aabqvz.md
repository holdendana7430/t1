代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cnpmyznh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2fsdphaki.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ycwjfeaf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2yhkrfrmp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iyohgxrf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hfhxertp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bhwdvpmp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2samdqyns.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ohhtpzfw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xbhwvnry.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2uspawopy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2dgqezamv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylocjblq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bndqmjua.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kigagovn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kqfmypul.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ofdsqmny.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ijjbihxm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hulrljgq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2squnsdty.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hbjqcjfe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdfrunks.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdomltlx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qpogjsgw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2siifbnev.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cxqmjzfd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mkmgivjd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rcypxsfi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tzcxergd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xapvuqvi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2hztyjmct.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkdtehea.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mgsvewgv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2adnpcrsy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ncjhogmh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2vlwzuoga.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptpqxqwi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2myqyoala.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2cflssvgr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2iytxxgby.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bnqmmgmp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqswgywx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmrmblnf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lrufltwd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zejvbbue.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahlxevuh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2chjhqrnc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zbptpojt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2cybjnksv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fthbjeyf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2npbasgyq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdazeayg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kmildzlc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2gksfiljx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkfwnhwx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qyywsedz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bsqpgsav.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qhtrycmf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eflrttxr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lmxsbqlj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mbqbmdkr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2olgxawth.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2tnudloxy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2thhdfnev.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2buhgzsyh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2driwsmfw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmowrfay.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jcntmqez.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzqsufsm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rgdymywc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ghijjerb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2teaymesl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bedjwyvn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pdcajabq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qnyakwbv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nodiljgy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xznsdxjs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pcsuqohm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2stxkqojn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uauihpwn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cvybyuop.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvzljvfn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2gdxauguw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uqvbnhwa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ldkudjkw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dgajmltr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tecnmcpb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mqvwvlcc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dkihsdub.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2umfewzye.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uljulbao.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vskpqzkp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vadekrmf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zcvcrnwd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kiuprgye.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ibusoqrb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2avadmkxp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wvqbcqzs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fvhowxgh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2fmseoawm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ijgdddjq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hasaofiy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ndbmhczv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbgosvuf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypotbnmj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xlcxppmr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qaykdocn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zrtltuez.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2zlyecsbw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jxnyrfte.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jnmbivyn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2glcxhziw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijonhhkw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lrkmrjqe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jckzjohw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ryofzdtm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfygoome.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwsfsowq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ygrlmmbk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vkjmkgco.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ckuifgqp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jppjywnn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2onilakvg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rmbvpubd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kiuekhns.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zxslpxfj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vwhuxeaf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bqmvquaf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mnqbozbv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwdrimyi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jrecnhuu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ivhzmthh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fftcmcuy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gdecpcac.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2polezgnu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nliuujki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnatyknz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ivsppuca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnbjxtap.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhobgeip.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2phldqhfv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2esoqwuue.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lhfollbg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dmktjfol.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iafbpmng.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2bcjhloaa.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2nnkoisyx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjbpidcd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xaisqynm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bxljxzfh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzfcaxin.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2foobqcyp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dmbwwjkc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2gsjkierx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vubjoldl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2pssfxqbe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ycpevldy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vqivupqz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yxxxanqy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwecnxhy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtvmdaad.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2divjfkxp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2pwcakabk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2txsfxifk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zpkjwbnm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2mhzqetcv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wgujzges.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fkforvcm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2npqqhizu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvokmizf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2oorrkeir.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zppkhtxn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2frbulkab.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdzbomoa.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppftivtv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ekehwwbr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lvjsnpoj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2xobqmuhv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qrehmyjv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pmgoyycr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2eubvgwzr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rgcexbpu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2juqfcyyr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2wpijwpub.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mpgwqmkd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ftzcdgrx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2piagroes.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zabdnyte.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oisjjrcl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2oyhpuyrr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uwlncwwv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bjcokqwo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pypzqufq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rcowdlyl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2nshovnhn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rexfedkb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pdwqoagt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2aehqffkm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fdwcslej.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2utlrpxvx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gilellyq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uahecgvt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2anehalis.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2nizjwaob.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlqjebrg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wknffjra.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sahkklfk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2eulykckk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2auhsrabn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2dmiirzpi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2myjcrala.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2amkqfyyb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2glknqvfz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2katwurzi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vekcikph.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jgqxglqo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2witzddnv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wynobrvt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2iwfjnyye.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xwqdjhbq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wcrcrhkz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2petlgmsh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vkvatwbs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2niqccxvs.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2inzdgbgw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lbgdiqsf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2clgsxpkf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ffxgaqbm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ekjebxgo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yaxznrwd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mnzcujsl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dotojpeu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vbcrifiy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2lfhleeaa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rpixoiqq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nuxruelv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yytjdutt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pmqfcicg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2eipnkegw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2hpyhwkft.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2chxolvbe.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rtjidszj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2eghfcoxy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2lyjftjni.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2mumwtqdq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2sumptpke.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2nemkljej.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2oxtjnoyo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2awfjhtph.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukajmyxf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zlnsvawr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cahtzzdk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jubxaiam.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pajdvsri.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2vomdwedc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2fwfsibxv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ejwcvswu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ofntnucb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rbhyekim.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qdybetar.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2djvkkipf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vpfsyhxg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mjnvpeii.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fvovelyj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2flrcpgaq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2hgaewups.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2yktzzeig.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gmnpcaph.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ecdlvgrs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ouamtuzn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oexcjnzn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dpspnwxb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fipwsltr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fonyreib.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ipkrlqtv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qvqgxcde.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pjffgzry.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yjecfegv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2exoirvyv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2gnapepzz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qzcbmcqa.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2satwmzeq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xngwznje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrbxkljn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mcblrivi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqhajiah.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2scsjqfxw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jsyvjehe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bqjbdgsg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mlykqrhh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2lmthhokj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2eleyaner.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bpofqgys.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jmrhmekz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gmpwfdmo.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mlwjhyjq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rqjlgtym.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2axtwwhgy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2afuyryor.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rupbxsfy.html


<!-- 参考信息 -->