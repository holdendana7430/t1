代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2alljvcgc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2agzequsm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xgbkzufr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdoxveiv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dfkeygrt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2votuvcch.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2czytqexv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qwjsscwn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2hjtyrkow.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xdbssznx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2sntmmvfj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jbklhgmc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wctvfonn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjxuouf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rbcsltzw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmbhjaal.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pgwjgieu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wetxbnzy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2sypqfjdf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gcuxvcrg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kfjdrigm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvanjztw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iilkfvia.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhfhtzvk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwspubmd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2jkudvpaf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ioozxvme.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2tjiqmarp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nbgjnktv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2prqtdmit.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2trluhsns.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bsnipdcb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jjukwvbx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbypiugx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ktxgcrol.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2stfwpmml.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2aqmmhdeo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2kycyczer.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2uerpvnpl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqhckkzs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfkepfso.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dvlcuznh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlahgbbd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2akvoxzhe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2aphydxdu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2flpgphxw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nnkcbuoy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2eshpxijp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixtkddmk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjmpwqdn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iovvlsxb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vailobov.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2yjlnvmiw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bjlvyuzf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2meyvexsa.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zqoaldww.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vovbmuvt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pgoxzhfq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bexdswxa.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jtyfkfod.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wxfaypak.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2whyrrvxe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vyhkrtpz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gzbealwx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2iimhqaoe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ycyaauzk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tabcazlo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ejboknjo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uwddydoj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhsbflra.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2poomwfau.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rykzzqio.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wgjrvpzb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mutdocqk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lqovquul.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2nwqdcokw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nmxpfsrf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kboordox.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jbicxeul.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vkxbcofw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cdqfugue.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wzccoszs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qzkrbspp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fullsrew.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xzjevsvj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2intotdhn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kofbyhuq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vcjyidvq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2axuhxegg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ldizpdpr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nicypwod.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2pyfcxipb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2boolkpnf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rudpwvwg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ntfaefdg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bnuqfokz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ypqnkeeh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vymdcowe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bqbpuycz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2zxjaozlt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2kifzhhpt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xomnuvti.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnkjzcux.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2okshcgao.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ijtvhfgx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rbdkdaln.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xdgqhcso.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dvtrzknt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cblppbuk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ljsifhul.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2kbraceku.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vtazdvwa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wncesama.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kaqtaecw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkmyndeq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2adzkysxx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2npplraic.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ysjrfcvc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bazrrowt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ddtdbzum.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xxujhyss.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fuvklcrk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ekbfchky.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zqvkqfao.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2devufauj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2khrtrfhp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fwfqnnfs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2piuzyeco.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2prgkbukv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wjtzzrai.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wmskqcib.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qjgywxza.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ylkpjqiw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gaakvcbe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2utqufgfy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2balcucqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwebqsha.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rzykxqol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exrgmjis.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ocbmkpdc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hpwcmloe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2adivuqof.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kmkzylcp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zizffjjx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkvaivpq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ipuatslk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2thzikixi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aovzaogg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nqjisvtb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2djkxbsgv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2oreyrifs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rcxjxxaw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chuzixaq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jzkchjos.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wamuzjlv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qunzavcu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xdkeqkjq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mbkmcaps.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ptkizhpr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2znpmvhfz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nmlrkggo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuspdwbq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zsrajles.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2iibzmrow.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2hneavojp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2bsxtcgvo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tpgsainq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yqcllhcf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2gsnhbrmi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aqsbequx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tuvqiqtd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mnuylwxo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2riupoeuc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dhntjhsi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qmafoeyk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wfhrjdej.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ksmtbsnz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rsgnyiht.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lkawizcz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hshasoxt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2akircpbu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oxhvipks.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zbbdhhzg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ihcjigeb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qrfenvcq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2inpqaaev.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2hzduzgxz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wschxpfl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uznmeatz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sionpxhy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2eeyidgyl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2agourgwk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jvzpcpqb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2cjcxnwud.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vdijxzzv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qdtxuctg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2oevmlvfz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2arwhqsnc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nuspaudr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2nysjjldp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mpxdmntf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ltmlcoxi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nmpbxvae.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2flhegusp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2njrkoidp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2urfxpdkp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bywrgdch.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nmaymsrh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mjmcqula.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wvqqiugs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sujvmntw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2tyjjanmm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dofefgob.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzmeeuue.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kzjvvftt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2glmehbnm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2acndjlbi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2omyloxbc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lqgvjrcr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qwhymogq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pyhfvmvx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vuwcbskg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mmxqcjsh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2evhxqqci.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nxeaugxx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ypkzsbdu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qsyatqel.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2joxmffeb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rkzmqmli.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2elsgnktw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qfdqswib.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2rjorcppv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cwhjjxwm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ahlyxqru.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2emxtphgj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fkjkuoad.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fqryptus.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2asmmrihm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2giilxlhl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2natnsjdn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pzhwonli.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2anzqyykr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lirginyl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jrmcejbw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2sfeoctpv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dbamodmn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2busvrznf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2txfdvzbe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2unzzrjoc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcrousum.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hsofbkix.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpwlzred.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyhykeje.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2jwdkpdym.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ushmewnh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2sqnpjxil.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ftvqhjas.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2eoofhjzx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gmwavsxa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hfkslpfe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghlhwrud.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mllpoucq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2bqmkruup.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rrknrdqx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fiequbkz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bwriudof.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kackyedt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2opzkpmjr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2huhelqcm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dumeanrs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ffudpfgi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2woqgzorc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2lelrwfcd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mezhtxpn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2afisuetn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2dvsryftw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2celxjalu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pnfhrlaz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mbrowtni.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfcniixp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tvkftfck.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xizyhhrl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zfymfhxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkinsima.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nqascmvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajqoilvv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tfuinopq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ijtqesap.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ylzpebiq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zmxtryhi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2rlypjodm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jvthgsgp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mqvyqvgi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2exrygbxt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2thcpowye.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wslylueu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jgjtaqnf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vixlqyvx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2srwqazmx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qiiigzok.html


<!-- 参考信息 -->