代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hztmctwu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2atcrcyep.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vraswpib.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2deozlvjy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2tngeiugb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ehsmqqcd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hgfhyvdh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ohygdiip.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2rociwvli.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2rhnzsukr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhbuprve.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwppflob.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwdtkzej.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2aggucwte.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ihcvuqgm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mueyzwjs.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2kiqjpxxq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vtetbhef.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ynbhoduz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2sohurtxt.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2amluroar.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qzdyhckz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jsnsmyym.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2euwzsvll.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gvtlqiwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dukcqvxb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2edlpfonf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkkibpst.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ezyyecrk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jozvnqbb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvdtvuwm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ghmauhoh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2quixknlu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cpmecyxq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qlwapyfu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2betekchf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bxfqgduz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2oucbpjgm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zuhjdrfk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuuuxjjv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ytwjmlzm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vwsehlzy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lrgybkyr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mwgkusic.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2hgsrgdbf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2shtynddu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2golmxwdh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2hxjmvpyu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpunhwot.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2plannsmw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hkntqxay.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxmbiads.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fmmwwsty.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bjuogide.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hvnxyela.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jhqwhjtb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ogelqzts.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2lbtpwfcm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuyybhbw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2plzebtwq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofaqiuob.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2etcfvogh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mpdotilf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnnspfwx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2htnyshzh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2plnhcksv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcbpklpx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qzrgmfgk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oresnxfc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2lolwremw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qcdkhrdt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rzbypttl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sohjdbuj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2nfbyapba.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kkuivkdy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cviysvps.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ojoleimb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cufphjiy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcnfctqt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rnvxffmb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xgpmkcvk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqaaocmo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2tyhcrasd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dgtqesmh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixjzeszg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2igriohos.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovgrvnjb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xzhvzmeb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2mhmbharu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2srunqkul.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2reozelwj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nobvxfzu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2iuclsvpq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2baqlmesm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zbckevkt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pncjpnaz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xscwcfup.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tkhmytix.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2duzhsswq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xsbfawgp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2scqppihy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ibabrvax.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxvazfpg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nynwrprk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aawtzugb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sizjebhw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kywdfqtt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ajntfmon.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kpyawmer.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dddqqevx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2uhbazbux.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zribfckr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2sfhizfsr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2upyxzzbe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jmgeplwq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2welkaute.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2jdigbssa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbefmfjh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fhsuliqd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wwjkiwcx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gercfowy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ijerrfbw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vsubwqnw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ofrwczeu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jjbopehd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dbkpjgxq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2fznintpj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2powoxatg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pgiddnwt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qlpfpydu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dojinkoa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vuvcdzyp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fnadyeji.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hittjcdd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lilxutdn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hvunbhvn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2kceqcpzx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ytzjbeve.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zorumlfo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2euculgtg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzppcmtc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qhiwayrr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2nbydmmde.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nyvjsrom.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2gtgdqboj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2frwriquo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rklcqvcv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ibrjkdvx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vuyppckb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ztvhgvii.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hoqupqjt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvciwmu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcuclqna.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qnkfxwys.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2osorzoza.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yvtusqym.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tfsokhgu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vixswgbf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rjackafc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tdbfndqv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2owdqfaga.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qtkjjhfh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uloagfsw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ukfjcmyt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2yhqgxmja.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2obzwtnoa.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zstxmckv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jfikgqkf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zatbjvxp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bfnwpfmj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2njsducha.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oxziuavz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wookmgzn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mzsrcmdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzausxmq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2njktcivy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zqaeyfel.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gexpezcf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxlsqtrw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nwhoxawk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2urawittc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qbsydmof.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2zjjcinze.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2acfxktsj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qobivfxn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zgwjktbz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pqbhjpcq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mggewdzd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjkxtlgw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2nqkpnebx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ueutzjns.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ejfrkzgh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ujehbsyv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2czxnsxkj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2deupitzj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2thqvxscc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kyjagcuk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mylnuxqg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzqlkvmm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2weblxrae.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2dgykecnt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2uystaldj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fkjtwecv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ymkcwzkm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ghfsixhs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyikgfma.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2eftfilly.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vjvcyosv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2tdkqsozb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aofwplnp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bromryut.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ncbeunpy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jkxmvtxq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kryzvotl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2begphlhl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uvrrmqxq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hlxwcssm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2doaswyei.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lbxgrgav.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2noesgvid.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2thjlhjmy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jdaxfynw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dkmgwcyx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kejeenbe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nrbzljpa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2dupyqurh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fjplfbip.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lnanboww.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ekwvomfu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2uefxwjfv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vcnocelw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hxzzdoqj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vkkghzka.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lpmmwoie.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vysqzskz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zjwrdowu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nldttwgz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uwjtsxsm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2omwsgecl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2bblttrxv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2becvjxlt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijdyhzmc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnutcdcz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2uzumjpch.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mseinuxw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pnobzgmf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2npfyoytr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dauicves.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mbuznsmn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvbbpuzc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hyvvclzm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rlsrreqr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnytvkoj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zowgzrly.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ecqlypwa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wazdvqgl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dfarmapt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2lqprzkgx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hbkeysby.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2osjlhjvw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hldztijp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yhldrtdz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qqdiwkxy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2nwoizpwy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2isvmzgnt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2hyqtwgrq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2epqdyjbq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2oieuoowo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ubvugjcp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2akufwmzv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vqsokmnz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rrlkcvnu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2uyqyucng.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nmvzxfwe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2hazevszp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2soeyamvb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xpszrhnh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cmqwbvlj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iayvskbf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yxezbgnb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gqncffcq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2brdamhuc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ctuaglwt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2reiqlfzp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rricvvml.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lycyaqhz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xwmbrnll.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2txyoudru.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsljtvoq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lvtttcqm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tosrzezg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jetsjkpq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzvzwjhj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ohcvfllb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2luazdfeq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2puautmbq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mckishpb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bpnbltfc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hcibtgob.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pqquzvtn.html


<!-- 参考信息 -->