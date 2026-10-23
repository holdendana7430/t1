代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqapyigm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmdmiljh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gvprwxey.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwvvjhk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3iburqahl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3rkcrmjyk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rmjokcjf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ensoripq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3wtygbyvd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3jcipggep.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3krydfoft.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hnxnfnaz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbmwblh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruqsqntg.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ghswhrts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khjuhbsg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ewqubvyx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ypzekmed.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xsdqfuzj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vxbmkhlt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3keiowhmd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wstaccdl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3yambpctf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zdhyocrz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3muhzrfft.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hdueputi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hzlsswcb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmonperz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hgkgojmc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nfecodbp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rgnfsbos.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3swcpzpzv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3icksjtqd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yxbvfwzr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jgyditte.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3yvoapykt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bhenxpuv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3osrfrqrp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwtdkyhb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qvhgkayr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ugdumfiq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jzqvodnu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kyxrwdbe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xypunfqd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3zbwdhvsg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3cfddntgx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rboaykjy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycnsgtiu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xaphcihd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3uzcupodn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3gehnmiwz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ijgwlqpq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lwyyqlqk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ejmtzxqe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfclorgd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lxkuijdb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlmlkdoq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3oumzfies.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xwburgey.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hwrepeqr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ldmdriks.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yobrsrrt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3nsedfzpm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zrrpxwfi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rxtczufn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kzvcffxl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3unndytmd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rqagolur.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fkiuyxao.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3elrwspst.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3yyjpkskf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rlrgubhr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3byaoorcz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xktvhvuk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3peqemgou.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wbgukvwj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3plinrerz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mumqnvws.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rikfrnbg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qercquld.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3vfsmkdpb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sdppbchu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qtlcstnl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qbraglwu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lhqckqlo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vedmcssz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bjgkemkp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nahjzvgn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3edskjshz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3shpeylzr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nhkwanjy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3whfsyzhc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bbhhrcyl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xudpzhmj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bdwkokly.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mojzhyri.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rclxfqra.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vkxwfgrg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3iamkcrco.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsviidhg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hlevkadf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kvuatqke.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykfcrzaq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ccwaoika.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jhlaolbs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3rmzwuxzy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hvoogdzb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zhhtcfwz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ctogobbg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qhbopmrq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iofluwtz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mopkerbf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ngjmwblp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qlwtzxau.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3phebbcwi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xenmdawf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3pmiofssc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3pmvbnnpr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xhtxfzht.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dyfssajt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qbkxkzpw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bkiavask.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ccsdnyfv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nnjdtstr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kwmtkygr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pwemnftd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qvzmgfwo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3tylkkhyr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3crmwvzqy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qtgiwhll.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3nsrzhpbn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3icekhnvk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dkyvvszg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fqawdxfk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3njxcauiv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wcfvyrqv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ytxmxrmu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpyychem.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3opkkwmhp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygatwotc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfsnnkum.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bzsipprd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rxjpwehc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3alrqimvb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vbrdjcfw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ssforbmu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tcdgesse.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eqajccgy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tiggvuii.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3maikdqzg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tohkxccu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tawmzdbe.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3mswljfid.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcggzylh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qzduocfn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3edhznxza.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3haufvouy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ulooeihd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3busvwcce.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vjhjqbom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttwgqxic.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jlauhlxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfnyohrg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wgbxgnel.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3byowguqy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kyvyyrbd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3czwrijob.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgoerphg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eystcjge.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3oizktbrx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qokynbgz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fxlwdslk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3michfwtt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3czkihtsn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hdvysrdj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kjwbwzvl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ogigbymu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3anmqohxn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ryvtvesq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ngmpmcfn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bhkflzhx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gaznasfq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3wdbcleea.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3znulmhgd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3misemrbv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjlekrtq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3scerpmih.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3pqhqjrnw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vkcnlsty.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3irngzpha.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ygwryvek.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3oryyhatw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mqsggswx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nahuenpn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3najlsffq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fodghntp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3iwsenbjr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vhplzxkd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fsujlzxb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xqqjqkpx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3swdncbxs.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lolqoseg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3btjffmfk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vtssgbzb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3poqdzuhp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gnkteozh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3maupkobs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3nnxwptgp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3cuypdyje.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3yxcrhktj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xeujpwjr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hpjnhtja.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vgspjkis.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fbbmrdhj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ktncnyva.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3maxnojsa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ygsemfcn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vfpekkux.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3riqlubad.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hwpoalum.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vjjatoiu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3oifkyuol.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhtrdfjz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qejqghug.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kgkrqtdh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3szqqbwna.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bdiqplbs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ahydwier.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jgmqpjxs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kenfudzd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3astfggck.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wqtvmjlv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qyuwmbnu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wskuvdeo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxnfrnxo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3sgnqbmih.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3obppwfxk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfljbhii.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lssswyao.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mbusfsna.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uysysndd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3zvazcjlo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wspsubtz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zpiyiwae.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vkdmgvkw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kflujpem.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ujnwomqq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gqswxmvc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3psfardgu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yohgqvzb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kwxnbuay.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3utslqzev.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qdhngche.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3difbnpxs.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3olosajyx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xgzxmbgq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ifkijnhm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3nzaqvixx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nykkdhso.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3eogxronk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jpgvgekt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ygvcdjgg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3musxcpew.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3pxxiurbs.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3cnvunzza.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nvkchoxb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xwbigunj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3syxvihhm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ftdhcccm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xtawxlvs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3edmkgpva.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jxrchups.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3iqerwqyq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbrauuje.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dqynzfem.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqulword.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtkwfpyd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3dmqefgxc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3yuxhfaje.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xdlehmhx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3fedluarj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dvhrigjs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cbelmwrt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tbwojolo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hrgiukkh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gehchdyq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ntdjyxdd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3udsmrlxl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rubueftc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3cymxwlop.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ujnimmpq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bfvmezui.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3isvqrlqw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3efvoxepo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yvlpuhqe.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mygwjtbm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3puaqrwzz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kxbrghab.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3kucrxvlw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jrlfajuc.html


<!-- 参考信息 -->