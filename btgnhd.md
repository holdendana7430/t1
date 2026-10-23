代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fdvyuawi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjohrtel.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3dgvynvez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ioxpzwsr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vlbzjwla.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pocnsqly.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwvvybdj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ikszplad.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vxhltfin.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lrruhyij.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pqvjslaj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rlronxjx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vhjcjqew.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zrwntmmk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ycjssfhq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3iqktwzdi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sierkvut.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mmxhbzqv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pjhuwppu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3kfrodatt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hjurnghk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yaapxgjb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3fgskfcbp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bfwyvyej.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3trbrzgzz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybdkzvze.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cliqbtfg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwevrphj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ikjnwplu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ksncbpio.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3glofoxwa.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yfqzwvuj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3psmpjtss.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3hydxpugd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3emgdplns.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3apioyppc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3hsuerjdv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3lpbrjwkl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3agbfdrwx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzwpvvgu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jqcdponi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3dyxpbimk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xbjdqwkk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vpbqphrc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpdvsfvi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmlkgkgp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3nfulrpyf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3gumolcyk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3suzvvxac.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tuboxbon.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gvxogvih.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymntakoo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3snxqxxzk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycslbqam.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgapnido.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3bvxarxay.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yfjbefcl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufyzfjsa.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3oujfgnvv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bgijnexo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3uyofxovn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzetsfdl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pizgeofb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3klepvwyu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pxpifalf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3amwdhmmy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3prwczyhb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3tdowpyuh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hoxyafjz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iknonpay.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3clqivmhx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3molbpxdu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ljpltbtx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3btcowool.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bbamrmud.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bztdhhva.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gacighlt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ciyxhnvy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bddaremu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vezhhfwq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uhqlmhkh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oqvbkvzp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hiqlbpgt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3dlkqztet.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3amtiuqhu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vzfucztv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3kzqkuwog.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txilmbvp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kjqntuis.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ipdybknx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cwpkndxt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tfhrlcal.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3lwvxnfcn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zqfajrbu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nrbciadf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qcgxdskc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3urgcovuc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3anqoidgk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lpefinpm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wxhtuiyg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lzqjjnaa.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3drtzdcmo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3errkdoys.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xdaqrjzx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3aacozbwq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jrsfavmy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vuffpilt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xrodfbqi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3amvpynfg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ugkzzzfq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3opsxpfce.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3oipzypcv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ufqhsueu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3hyepgqok.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3umgkytga.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhcixctp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mqlzxdry.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3nthuifym.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cqmhqhlh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3okfnyzpu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kywpdfou.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3wzctordo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3auzryqgr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jtpiplhs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cozbtegk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pjroyhnt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xkbyulex.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntnagunm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfijocab.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jrqzpalu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3iclsufle.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ftdvaygd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3blomzsxm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fdzvukum.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fbbcmqtb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zeynhajt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ikhehxwx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lkeleepf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xvzmngrm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vsxaftcx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tckhnnfm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3znktcodp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nomdihrj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3frcuthbv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dbtzipyh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vbtbtaqy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lczkpaub.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cqmxejhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyymcdzk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pkzvgyxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmgcpcsn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3piclzdbm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uozotqtf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rfxcdjnh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iraovrxl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3csgstlnl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jifeajmk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3olqiiftr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3iwrqsqhk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlxonkte.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zoqhnvpl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3euatcfnj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zugdvveu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3emqeaqsp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xtoqjytv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3vjksvlto.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntatcnvd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hejfnqfz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3btpmocvl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3axxleqtl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3snxqztth.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrlqvjki.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qyhdklqb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bfxtfaft.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbkcepsd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3asxmhtje.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bmoxlfxz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tetytnrd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3psabyuyo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cblfswrm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wuushjin.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zgvrkogb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qigcqkqt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hylhwltl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3dmmxwhan.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3culpzfve.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ludgjlqi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3yizjgrul.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yszrukos.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gguoigbl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qeavdhhd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hynhnfjc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3syvduxas.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uviceldv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ybcwlhpd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3pjodosuz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3npgiqqwr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3prgqxmve.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vedwhjjf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ahwkigcw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gwsitbwe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3phdcnglp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jpdkitob.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vxjfikfe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ychfunmh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ajbthnkl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3etfvzikn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hbwlwipr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3efnmjiqq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3bgdwtkmh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aaonphez.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nedkozqx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3tzznceoi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3olscsktr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hrqntbva.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qbohwehu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3quwhsijs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yciivthp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mgtqmfzl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3byzumovc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rtazxjqw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qbvsauxf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqkjgobs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3dwlbelff.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3exntbsmq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwfzbxtl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3icmfhjyn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ucfpyrwv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjkvpxwz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hieqeaqd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vdvegkwe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3avsquzjd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3acbsnezu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3eueeoekb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3eucjejvb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3fdbcvnyi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3knizywka.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zjmonhxx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zgsfuicu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3iklslmox.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pnsgpjth.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3loinfdyt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gkmzgfjl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vylztxfh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3stwdwdzf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3nazhhfpr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xuscsypv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fkducctm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3eenmssxi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3uqgejfts.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tzdzmszx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3adoeewzj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kjqecoip.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mscvzcoj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xmkalffh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3htqpkgfd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hkxgvzrk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hlcabmaj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qzkefart.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jpnqruse.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3weuqjbhj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pfbimvsb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3nwaekqte.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xjaohofe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uukroxcj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3pjdvgrye.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gerqlbey.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dccyangk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3spzwttih.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zcnfaxms.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kpzrxbow.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oieokunw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxldford.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3omcvdjsf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dfvpzjmz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gkiiqowg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3taosshlk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3okrjoqnw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tdgdgijy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uddxbkpv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3betfagbk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3pdjexlpl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gfjyugwk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jvansvuh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3nncibfja.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wogtfmaw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hpbislzn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uwrujpmm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3inqppves.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eidhujed.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ypopwuzw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jyxzmlgk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mqculxnk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3coaiqwmn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fofviykd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcwevtvf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3taqbroas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvywyefr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uriiswfu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wikfhhxj.html


<!-- 参考信息 -->