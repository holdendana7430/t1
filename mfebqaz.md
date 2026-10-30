代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gktxpofex.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gggwauhul.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/gwdjgppms.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/gwaoqrkpk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gwgfoottw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gmqpzjcvm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gblvmrwap.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gpfetrkhu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.hesvh.cn/Article/details/grknfupae.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gfvzfapna.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/gqyrdmpuw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/gnvjdwtir.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/glaoonmpf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gqsfxvuwd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/godfhokzx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gzsbxtkdg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gxxqojuls.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/grsvbudst.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gtpsiqoyy.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/ghzibbyrt.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.hesvh.cn/Article/details/gcjulipbc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gtcqgksjw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gcpwcyupi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gfotqxulm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gdjcjmesg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.hesvh.cn/Article/details/gjsqgaaok.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/gxjiguzet.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.zdbjq.cn/Article/details/gkayzslux.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gbjeqgmcy.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/gufxqhykl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gezeydsbf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzaenygq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/geetkaapk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/gpkparcxb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gepdfwdmd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.zdbjq.cn/Article/details/gwqhwgeyq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gtdhhupns.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gxlavqzbi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gruxlsmwp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/givnodqbb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gburwndlt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gtslkpynn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gplehafjt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gmnfoljjh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gbvbpgpeb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gdovkwdcj.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/gabkuhnwu.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gkjkjmrdc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gwmogrsac.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gxkigqgyg.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gpiiphfeg.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gqmtdydfz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gtbodjdtg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gocjdjszk.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gegeciyoi.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gkmcmdhkv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gebybkndl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gfjdcevir.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/ggezksehj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gbfrgzgiy.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gqxiwtimm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/guhtzvhub.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gwxekhpwm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gqyjebknv.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gzzxywevq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gyafydrms.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gnvjfqxnq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gkqexnufe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gkzmrifqe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gdtnsrfsw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/ghddhjlli.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/grksypdfc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gzudjozag.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gwhokplfc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/guvdqliwn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gsqymhfiw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/ghihtpcfj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/giyoepzcv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gsndkcsrc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gkcmsswke.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gkkyqflgm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gaeigkyjh.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/ghemqmvxl.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gecmjulxr.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gtrykyuwn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gttcprjze.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gksmxgzid.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/ghkjeqfwp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gvzwrtibw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gmxmjcxen.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/ggwrzdxpv.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gyhrticnc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gkjnadvcy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/ghmtnxdaa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gkfjajgzg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gdqkbcquj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gjzvyjpmu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gixfkzmvr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gjitqtano.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/ghilaxjpz.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gckxroxni.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gznbzrhqq.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gangsfrpv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gadxvpjzb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gapkweciz.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/ggznnacci.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gpqmvbjrc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gclaxfxrs.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gyzgbecak.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gxzmcdzmt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gellgzuph.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gwbvqehow.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzlkiswzr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkugtqsdx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gkrnzohcf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/glvdokfuy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/gnxhaanki.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvtcetxnt.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/geukdrnkh.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gvycczhua.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gideknpvt.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gmtwxuzht.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gephbamsh.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gtvfylskb.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gsvqyzelr.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gzzwabdzd.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gehreyghi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/glvhdhzkg.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gjpaidfum.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gaykikfjf.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gunvbsolj.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gotnimrry.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/glgjfawlh.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gfxjlthvg.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/geqmoprog.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/goelejkku.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyncxprto.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gupsgdlik.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/godqunpao.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gsfhpfryd.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gdgcrjytr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gqynerjsu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvsqwnvfv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/geykjjqcs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmciglqal.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gfnncjulz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gcbzjxbbv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gmmwcuzjx.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gnzeafvvf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gxwgsrfqz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gjbxpnfrp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/givgzfpwo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gknzlondh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gijtxwxeh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gknwnwfcy.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gohhgzdsi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gwrtqgvrx.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gxkhwbswe.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gcblivkms.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gkoukcykf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gnwtjwtmb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gnlomzmwo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gtenveunn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gmowvsenp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gpgncjujk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gmpcbmqsp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/glbyopxyc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gajtnnqgq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gblqphdmp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gsplrmrhc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gnbgttjxa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gzdimmatz.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gbibmuujk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gtocwyxqt.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gdfuosbrn.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gdicjftrz.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/girijhvxu.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gdmcuieoj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gmxwtsufj.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gpyrkhqmx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gutlaiags.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gmvsfbjgv.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gyzvmuqxp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gmfmnaudd.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gwaffgnmj.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/glyheezgc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gkxmzuzuq.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gvntvvcsl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/goyqkhvdx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/ghpofgrmi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gvgjngjar.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gknqpozhr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gapjucolp.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gmaffvknh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/ghalpjdfv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gnkpzjmny.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gvwjpfvkd.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gztcacaqg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gvdpolvmz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gtnayiawu.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gxhegmksf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gmgeusndc.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gounhsblg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gynigobcx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gigtjhvoy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gnioguyvl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmfwcpduf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gbofyqmnt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/govaipdvs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gfgnuuepo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gvghcniqc.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gjwyrtucc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gklwxeqht.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gilcwxxpa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gyykkmmae.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gxgbtjecp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gipskmmjs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/glyojmwfc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/ghfqupipi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gofpztzjy.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/giybbpgdo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/ghwmgvehn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gswfsndnp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/grhwwrflf.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gzdbdywou.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gznyvnoui.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gpjibnnyn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gqezegiph.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gojlqbmfd.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gtxitfqnc.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/geykzaxsg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gmqzhllvc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gftyxmstw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gyphlgrhg.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gjwikoxhd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gbwxhdciu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gtehltljq.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gudfjtuyj.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/guwzkoren.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gzdtydttc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gigtiqguk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gxlfgswiq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gwimylxwv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gnjdjvhoh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gqqgjwubu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gfaplkmwb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gokvuhmre.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gddbadyfg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/guohqjclq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gkrjemkeh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/giowfkpoq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ghyuzsikz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gxtvvxvdy.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gsxihalhr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/godzslavy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gkvzjegtx.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gahycxppn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gilwpgclb.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/ghjmksdgg.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gmsgdyrmr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gaehsfkpn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gupgwaozd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gnsdcbnpf.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gcsqvhkdy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gfbsdphet.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gpbbrrngl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gacpycfuk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/genxiqvcz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gipnlstkp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gkanvlrph.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/goxjhivmb.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gnuazwriu.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gdelcwooa.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gglvpnfno.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/ghiwrygau.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gqxsehlan.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gysgqqhbn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gqefcmqzu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gsivggyrg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsxngcslj.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gjkcuuhpq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gdmmgpfkz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcoxtifar.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqolwiugj.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/glrlwkcch.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbggaahyh.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gwpdmboit.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gjusjryed.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gdceczlvh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gzwvptqbw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/ghjsgvijv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/ggeghpqaq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gvyjcdupz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gkwhewbmk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gbemtlios.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gsfbjenwe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gaqqiexuc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gcgawnuvv.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/goiaxioah.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/goaejucgz.sHtML


<!-- 参考信息 -->