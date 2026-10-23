代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ktohxxof.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3gagjqcfp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3dutfvmyc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3vrfqqmif.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mwmrxmfq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xtyaegrx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zehohdjn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xqvpmzwq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ihvyeajj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzowbpvf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3asozliwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghddxpvx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xozkcwhy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mcoxnjvl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ompntkqz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pzzvbbqe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ffqufflw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lxmrmmyo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3fkzxyagm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3degzvagc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yenrhapb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kyzzeifd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jqmfdmgr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hlymvgas.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wxwmdokq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rzbmavax.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uqarxdfc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xskvdzrk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xxjxjsad.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fpwwlerv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3mlijramg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3wjdfadup.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nubleyrj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmwcnifi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hqpjteap.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pzxuhigy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzsaaecs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3dfgkjkpu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xkeziwus.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ktwelxfk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3osfoelgb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3mfpsciqg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qybrdwur.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpvhlfim.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fwzeoerf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3iulghtoe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vbesvipd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wdkpxgjd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3duwpfgcp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ummiubaz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ythocqtl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cckeyglc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3awmryeeg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnxdnlko.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3onucakvw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3rukfqqiy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xivwnkli.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kdolhsqz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3oeolzigz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qrsrfjly.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebgcaybl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cctovmru.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljvjxyck.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3twkvkxfz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ucypzhwj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3leipeavm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ivcjryzn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3znclvzbz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvqzurzu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sxjlvwgm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pnabxilh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ovcmxacu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3mzigocha.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vozhwtgk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fbojfiil.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fnbkzlwh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3yzajvugh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hxijogqp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3brglbkrl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3otwntaao.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nurpawwe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3waabyqej.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zpupxmfi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iczoezbb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3daiojzdz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lktfvjfu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvpndwoz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vjmmwjgd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ceowqejv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mdavpvzf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xcedwgqd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ptmzrhmi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hbahstaq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3divegyni.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3iwlqivgp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shqzufpt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jqbzgcwj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pmnmwmrm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nzquxvpw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbjakfjw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3szcecypx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3dhleabbm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ypgufotv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3dyvtcmcw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zxwonirz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vysvswlg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zdfdtbei.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oqjtdhrx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ifeqaddh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3negoohmh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yphgkxvd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3sblfxdgm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3lkrftwoa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3refodbjt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fwqmvcwj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zzwjyjgf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ixkmebyp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dpgncped.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kdjmadbo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3szdhpimq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lqccumah.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hckkqtiw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tcuqsfiq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kjycswtz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xitdoxmu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3iqqysggo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vefzeutz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3pjgnqnmf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3uqbvhhis.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3nipjizxn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3zgqdskrj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3btjuxzja.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3faeooiri.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3naqnxqnz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kaewgfly.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bilkmrla.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ttinaqyp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wpapaqmd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3erfdxqco.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3aqiroguj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ulickdlu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zhipccsg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qqxunciz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mmedchpo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3govmgxua.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3npfmpjgn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qrasltlr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ujbdrksu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dvagdyis.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhgzhgvl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jdigzkws.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3efixyszq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jkhudtpn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kterwvzk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3udvolskb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qbdtbgnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmslwyaj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3tbsmjlpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzbrofwk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qwxpkcms.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yqcxgwfk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3awhlymwf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xltelpil.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsmolzrc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyjqwzwm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ggxkwodq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wxkmmmif.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjtxyxyq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rfjqmwfa.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xkujzrvn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdxakawh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3srvxrrur.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvkaugqu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3njarwudi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ckmpbkca.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pytrdgsf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qeatrunp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tsbixcjd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ljmqkcfc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxhqlwlp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubnvproc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uhkuxmih.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovqovxqu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gzujpsjc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kmuunsep.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3drwpulkz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hdujandn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3uacieblf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ltpnkirv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rxyiifwe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3efwfqvtl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3aredyeea.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mkgctpzn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3krjfvdzo.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cnrqbpeg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qtyvexto.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hjvynahe.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ivolsifl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zxzeiqqw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jguweeoi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3shdoqomg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mvpvwnwa.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3kszlxlrk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3eerashtz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3iwechszr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3afiriter.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3kmiuriqm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ewqkbpdz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xiuzirdo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ocuwjrui.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gwpbysct.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hrapnwpd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gzhcslgw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3emckowlq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ironkjaw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kgsoqcct.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dhzyyrrk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wcgjzknd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qdqthrea.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ctofmotj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rnelmydq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3zwntiobz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3tgcrgsqy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3nrhsnwup.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqsutdww.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzxzbxon.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bozbqhxo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dxzbifed.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3unwhkrnr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3elcjzjbc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bewgasdp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qvtgqrbm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvoibcso.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwgokzra.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lxcnxrlh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3muixipah.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqpfnpxe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ytrfqanc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qvpgqwgu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hthyfijw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xsyefcxz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gaglitfb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wlwmehbt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wldvasfp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3szkekgqt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gatfqddr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iopqezac.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3eoepcvfl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dkvrrpgn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vyotwihd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3czmuvbqs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3znlzzrrl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sdkpzuqg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3btlrktry.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wmmcvgpl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3drbogcdd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3pimswajf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3akwhgvvp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3idrfxpwv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3rodvrqfv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3bpdwghny.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xbzkegvb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3didgabqk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3dlhkwefl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3anpglxba.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3bzmpwgpa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbangclg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3cvgaoxaf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bzicgisu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rsfopaan.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3hibmakzx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pdmlsfqj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ctcspugj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3rrzcocft.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wpkeqfvx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3juzoshbu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pqbyxsma.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3whwhgnyn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bwlsfsqs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xmafilsj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvuemtyf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkkkpbvx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ihattwmm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rjiojmnd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rqdjaewm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3oxulyxny.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3fgztzqeu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pcxofznl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3urnittry.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dosumbkd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nmjwxmds.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3veeamcfu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rdmdvwzo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ptyownuq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mchafxsa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kjdnpcff.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3uncgaylj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3shuoqqhg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ljugtpus.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnmhikrs.html


<!-- 参考信息 -->