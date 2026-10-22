代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ewplymtf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2odnpmlgk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2emnijocx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2xmsngcbi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtnzagkr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nmrahxmk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dvvmjlve.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cserubfp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oestbhvx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2shlfklmg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xsaiuihy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2unlgpuah.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2suplwtua.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruzhgenf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvngipss.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2asnnucbs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xurnkgtr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fsevyuvm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qbxaxvrh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2jsifcixt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2obwippro.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2tngwwbin.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2qzaypsbg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pvgwnnbv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2wzxnroht.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2phaqexbm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kfikofls.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ibzcfyom.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vcjsvwjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxoqtufh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ergszbwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxebmopr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wsiyjehn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2yjclzzbl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djhfqdwv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bbbmiuqo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bxtixopl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2scswvwat.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2fymysqux.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kdnszlme.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qyfutavy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2poyzcnya.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2eudpuurb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kinjxcdw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tjpxrjnc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oigteltz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2girnguvl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2licawavf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dcgchhgs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2heknbfdm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dkeedfjt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2kfsbnsyp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvkipxeg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gtvgizzg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxtjsqux.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2byczoxqz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jafvowan.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bbfbfrzf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lybjsbje.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ncrjlxdp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2iyupnfmc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvbznzll.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qfnaaseq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyspgmjl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxtkldtt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vbhphksp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2btcptzzl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmbcanum.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xmfsmlur.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bnggkrou.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qautfton.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dzruqdmy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfulhkyk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gqddnlot.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2swzponnk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2nizlzfsb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjuqsdqz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ghivpxbi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kciayvtp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwkqdlnw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhmfczho.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgdobtau.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hkigrejd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2yvsvunqf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uxgvxqbb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzfvsskp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jvvsezzb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwkwknhu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2stoxcoff.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqlwgldc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ojzbhvov.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nijiylxz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dtmncksl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wkwdolgj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2spxpesir.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qvilvxbj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2nzfnpotv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nceecqxp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rtuiwsju.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ujecuvxv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mdivahmn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rmdzgttt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jdjrqkyb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gmyvmlyu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2lknwnuck.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2easyswqn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fjynxykq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrqdwihs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vplcblaj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxwpmlh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tsfcdiqb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fnjqfczb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zssubaqm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2uxkzsfad.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2yvebakkf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2syjlqpnp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hpedcxpk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2euawbojt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdlthcwx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qoqjdhat.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtmyxzi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2emorngim.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2neaklsrd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2aiczwyem.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jfjmmmxm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bjmtxggw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bsisgkxm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2lfmmzdlp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ywylcdwf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ldwdtoov.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jsjbzytk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2rzkjpjvf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2wzfbkqvw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2xicvrthq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tasclxxp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2eiuarmrp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ugxzhqra.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nqoojetm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pvrrfmqj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nnevmvru.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vdnegkos.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fqhtkcxc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2enuzsnti.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bywygeja.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ninpypgr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2aaopzgqv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2nigeutli.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mmkcfooq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ywgjmdcc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2bfzqpnbj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2kjgxtrgp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2iqhippob.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pnkastdl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwymlbqu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2feptcraz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2freovwuz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2obkkdnhv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aerghizo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2dcdpalkx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2haqfnrvf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dyfuonjw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eeukroaw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kburgzmh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uyvipmek.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dqkpzgcz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cafittlt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zfvkmyri.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ykmiejym.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nxvbuizb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2crxaznpy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nzucljkq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2avuyfnoi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nrntmmks.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zikepymd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2owwhfuyr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lngdzown.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptkzomev.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tiimosuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rutzudan.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ijjfrsnk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2leeybuta.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tcispfnd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhntrbvc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpsepjvj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxuswgoz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ynuynepm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2bmmzsxpf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gsaaxmcu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kdihjemt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2okdfpijk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2velvpqrj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uatlbdyf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2brxegret.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2izninxmx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2tdtutcjg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ebyuqdyl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nizyfuqw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2foepwauo.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rqdzkbvp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nybmskpz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2awwedskk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2svszcdwx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ukojgjlg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gidqdhgq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2hwetfddw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wvfmyaxi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2sqqcmqeq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dkzpeihz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fwfmimzv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rmzpafew.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tmemgkco.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jzxrtcsz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2quuzaokt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zbznikmf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwnlbiiv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2brunwekd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mqvnylzl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ncehnbph.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mgujoerv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bsnynabt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lvlxmryv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kjkkgflw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xtqsmgzr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2cgfjrphv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2plajghnl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rfrxtnlc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ojkaarhy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vjjqgpts.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yhzmvzcw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2btsesfun.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mnvinuiq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2szhydjxb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ruugsvkh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yrezdnrr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2flhcbaid.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wkjnimay.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2wsiozltt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2agamjcyp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ktezhiew.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2nwawbbwz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mfviffqp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vlscgiow.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2frsoisja.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rvpxxwmz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2lrapmhax.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2erzknolu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kfqsatxn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2yfelexzn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xbuokolj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2eyjzcjte.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocghscij.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2uoksaywk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2omueexpn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnzzucbl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kbreiizr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lmxvqkpj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2knmbiyyu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2sivplthp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gffrralp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tryvjzrf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gwhypaiz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mkoasdxm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ybitbiqc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zqzlarbk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jrsxnrka.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2imhdeoxe.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bqstpdpm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mggtuxue.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2igpxgxhq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dffqxess.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2zyrqlgde.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2yfleoucq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2neaqcbbb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2msagcduk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mxkhcfpz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ziygpked.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rgebhbbz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2flaxegiu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2fqhkwupr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2crevjbtx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dougmdgt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gzogeqja.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hujmgvgt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lehxyrea.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lkfpzxgz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2kohoejoa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ryqinayt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kkuxabet.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2bilraqno.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctinfitk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wxpcknky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nwlijcuh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2karimjgj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nvsknizl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2eohssbhq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vhfhckbd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfmuchze.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2labyaefs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xpigstzz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vbmujpcw.html


<!-- 参考信息 -->