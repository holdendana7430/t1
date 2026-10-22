代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nxtwxjbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufapbunx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vqrdewsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnesygcr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2jkcjhbhu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tgrpqcpf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdzguidb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tkeunqvj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vsraxahv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2phxfketp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2npiggaak.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2cjjzwznu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cbesgivs.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2yapbczrm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2oduexvuq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvhahtiy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wlhkmtso.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uyyqylgq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fjvjistk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ijlfupcx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2zewfucbv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gqwajprv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2otyvithw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2orgsoziu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ubtlwngg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2klvjzpuy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2psmqxdmj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2etieugvn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gehlqqzg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2itycvfsn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2awduzent.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2njbriktc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mlzdlewn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2khmftzaj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyenbphn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jszyzhhc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wfxmfeta.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2twjzlqvl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2qmyfirxo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2pvrpwhqo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jcxlboup.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2yplnnutc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2zduqsdiz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gquwrxuk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssosdkjv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2oneistzn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gfspubgl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qqmngsxu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ufurbpzr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2tadphxfv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2esnpccqt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vpjytfpp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jioocoin.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pyzrxwsu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2kjpyrbes.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2auourlpt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2tfvyugvf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgrosttw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nodmydap.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2datkmorr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2osgdcgrr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsnmttru.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqdbitsg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eprzacao.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2bcfmgsum.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2oepfrfkv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2osopcmsa.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ycrplhmu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pyzvscyc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xizfuofq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pemaakhk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qwtjfrfu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2imqanhup.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2skfzvane.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2grotnlcm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2srppblpk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wzbbxfur.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2incqavis.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2slojqobp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvwszyrz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2opzyrxca.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbhcrraf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hxkwoehm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rewgunvo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xixefzbp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gsuksopw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2yifjjnil.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yhdkjrwj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cjouhukh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2udulwvav.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuojseyt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sbpppvoq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nyzyimpr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dynxyvsi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mvsxcqoq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2witfnroo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wjblvdey.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pccxxjsp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lxcppwvv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mzgaqvby.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2npodniqs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wonhzgpd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmweepm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2aakqhzgk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mxogzjvb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2niigoajl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lhfmfzuk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nzjxpyal.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oxxpiyme.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ahhtkfvo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hygsnjqt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ujuowzfp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2baxqttox.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vpnjmpmo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2qbjyokmu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2twpkkgxv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2iknfmgfh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zunhbevz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2dvgbursb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2xqmkdnmr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qvmflnsr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hfkawpkt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ckgrrntg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2bessnrpz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aktiwcnp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vmxjpubf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2klidwklw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjncyyi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxyaosbb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2semcjsww.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yrdxgxwa.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gjvnkwtc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ohsgcbas.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ktwwjsjj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2myaizuac.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2todoutnc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2islacwld.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zkaolzod.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uchvmqhj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ahfppfva.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2durjbghm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ufptexjz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vbxnmxhz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2istvpdnr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qkqpwkjx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vlmjmmwj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rtqfffvk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vxqqlqsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuomurpd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yauriumc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqwwygav.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2obnbiqnp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zbsqlxkk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcjhtrpb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2whwtdwyi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jpeyinyv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wosxovvc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nahbqdld.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wonebrlr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2otjklceu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ldkkjxfq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2pkawmddk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2guoxrsti.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cdtykucw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rconthnn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2djtlvgkx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2btejicaq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yqjtrcwc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tweqnhms.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2brswzear.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tzctefzp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvmswanj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2efxlahcs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2afrqcncr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqbutoct.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2lszaukww.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ygbtrrid.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2imoqygez.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bcdzvrcq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pzcmutbc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ztopjhjb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lsrjxrcl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zqtmlgib.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tbxwurdy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jgsyvfwc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2amgfdzzu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2snmvutnv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dzljlyrf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2aoqhzmrz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2naztnqtd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ooypwzck.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vlofylio.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2dawjnjil.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hymugzac.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2muvbufse.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jrvyjxvs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ugixntjq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2shdpphlu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2lixybgzw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qyfcmziz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wpmnlgug.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2scqhcwyu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2joflsoxn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2clicutkk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2flpbzkqb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2sirqtbyz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rwswwzov.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qniejxjw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2goubfqlu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2bvetceyc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ukijlqom.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mibuuuyg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2enbejlwe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2uxkhljju.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qeommpwl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2futzwapu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oxrnztwk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhqldfzm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2onvwzkxa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2avxkrbde.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2jbddjbwf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2uzsggnfo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2arstklqk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2fjhpfevy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2czziudvt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2beywhidj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2anxidfyb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bdicvmpa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2diawfmmo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2sfbanguu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqqshzfo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2afuaywhj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xcucyywk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ydvjxvuc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2iveykucq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rtlusdil.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zzdttuvl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sqtgqixu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2znwhexyr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xabugxfz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qgnfispn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2iomdzwor.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mlbulpct.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tayjpsfq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kytlfxsm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rmorhkso.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2sxbqppsx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2nvlllfes.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ubhsmahm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2njbnhpdj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2qsvqesvt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2yabfrjhh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2twlitqfh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2trsjytqg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qmzvvenj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jrsfxgum.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jzzfkzzv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qcyqwfoa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wyaxwkti.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qcxelznq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sxvgsvov.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjuxndfd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2igvapseo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzcqlmpw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2suwsbfxb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2dhogtovp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xjcouuno.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zofejrzp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jtkogntd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zivioquw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nyidlujj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lkqeuleq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdqzexze.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2plxlriwn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ehezmcra.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2orfzapfn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2eqobuzys.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vxkezhpi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mdmftsxu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qmssrmqe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qquhhqmi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2bfmivpma.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hwcsnbti.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2asfnypeh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cnsjurda.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xruflemb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xqnbeyka.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ghthmxzm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2sfzvsamr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kiprmirf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2brsunhxa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtezhlad.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uelwdust.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vngpvfee.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2warligat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzefpsyo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vnfrbaqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbchuhfu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tiofprjr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jqzuagks.html


<!-- 参考信息 -->