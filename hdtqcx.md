代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fyzrtbdk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3snxkwtay.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tglaasjf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3yarebywh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tybocmrm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oirskpfs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3jacrjvgb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3fzuqowxo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bwnibedi.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3gefaqlsu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kilfnrer.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zmndiqqt.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3uavxxhdo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hqceuolu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3lpafnwyb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhmeyawd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nogtgpjf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bmzsctwg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3alhhzvce.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3muoagatt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kwlvhqpg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3gpmzuxju.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qpvynuhc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3iogqnoyo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yfuuxztw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bmrvygqe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vifzjfzn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3bemacqph.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3oukqampu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ehogbcpm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tkigqdyj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3outoszwd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3iuywaqcb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3imohixln.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3akuxcfol.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykteqxwj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3reliprfm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kiiptlkz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3zzcrnibh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uxgecrqa.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jkgkdrht.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3hvlhwnfz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3lzrtndgz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3fqerizas.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3dryzbsex.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3blotwiry.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xtyghbka.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fxyxszws.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3oddzjlpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnhgspzb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ixxjxgni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxiylmbf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xurvwunx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3njcuofwu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3kgfaaqay.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lhrjrjfh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zlzocvpq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oxewpxsf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3oxkchacl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3kyhrlcwb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ykltxbyl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3bvczgyzp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ktbgfrfz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehnwzanm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yugliekg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wnuxsfyu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kbvwnynu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3zlyvhete.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jabtstme.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gbshpcbz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3onxmqokz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3couoxuln.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkxdchzn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kahxkfdd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogoyjxoa.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mqcbtbwp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kdhugxzk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ncwyavwr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3clztteki.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nskieizm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rqncxfvk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3idkbgnpu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3owycqfyv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wkrdsyyj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dfdqtkjl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3najmhoiq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3fsogovzd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfpsvdfz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gtuoftfo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3eprcrqpe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3vjvsqvjm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3urcboumf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3anzoorvf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkrzlbhz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3siodbzzs.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zbwueped.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqdykzao.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jieznoup.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3htwgdeci.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rpibsemf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjjkfrgj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcfzbnod.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3cwllgimg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rxbzyvjt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mnsnyern.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bhxbaqjm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vipwmadm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3arlarnvx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3meghwiin.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iyfnjrlo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bymtikzj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yjvrhxbz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tmirgrsu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gobibnaa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pipghiwq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zallohsj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ddecoxhe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rpvvpwxq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zimzbwzc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bncfeafb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zrvtcabo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tswjlorq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3atbtccsy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ggmukexb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3aazgypws.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3gwdauzxt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnjvqvxx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3adzznnmj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzyscbxz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ybkkwkfw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ltdjkvhs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vlfpkdoe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ktujqzag.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3qpxmiiti.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lxddezfl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3eysinsmx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qebkcvin.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3poyukzjp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmhwujri.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xmyglgzp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kdsltwik.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltbdsiyw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mqqzvonw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jzxecihr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gfwhfltt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clshkpay.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3aonoggib.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lehqsund.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3aetvxeex.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dwwvnpor.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kgaibzbg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mytqnjxb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3pgteszkj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3oicfqzfa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pothszgb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ncchoykt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lgemidgz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmcjtcot.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3znxledau.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qrybozzr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ucjuvlze.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hrjvxkyd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3eikptonq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lvsriiia.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nyeoxafq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gsqbwziv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bdnbpeco.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jlqrfzcw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wwsypqmp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3nvpbevgi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3icogzehc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gmarvsaw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ucbnrsnf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bykhrnth.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aowdtxag.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3glcrndyz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nohoxygs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3onlyjwws.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jsgwwxgs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3aqsfjkdk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3dlkzitsa.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vefdpzmn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pluxewqb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zziqytvo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kegndyuw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xirplffy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kpizwjjv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3utvrrtfd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ldtbkvfc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ztqmbdvx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aabfoehk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3icnmgzii.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3twexthxd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3eyygzvvj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gxykudnw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sgtnavxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlaokufz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3euyqbmnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aafzmfar.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmjvbtlh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3todkntrf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eefmbuog.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmsjmqev.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uefvectx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vgsxtavv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ulehoiup.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ecasgfwm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tklukjrw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vkhmrgiq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3phbzhrnv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3boozagea.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3exzebgqk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3slkisppl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3fhomjgnn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3eutaebag.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jslzpifv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mvlophnh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ihwuxkru.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3zjbhqkcy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3uebieimq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3goglhber.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3owmyrzbk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmslfhcx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tusekhyi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wrpjsrcn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3uobrcvqm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tcmavwmi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tiikgjdm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pfaobfrn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwafzgzb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ltjxsdfm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3twdcsjks.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hijaxcty.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fnlydoza.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3upjlllge.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ubielfqp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3khawnrjr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bejixofp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3efppgkqv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pmochgku.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qgdvccvp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uhekgofu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3plxvjbww.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3tbpcqgal.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bvutlvro.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3mrqlqycc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qyizzubr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lofqqstt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hjoknxif.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3mtuxwvuh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rpjkzxnh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3tbdqervm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wrlrknwq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3edxntokv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qpqfwuob.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wqspfush.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qpbflqwv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3drksoeyo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3icxzqybu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fykthucj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vkpljkfh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3krypwexn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fqyyrhjs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vzslbzgj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzjbjkuk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3iaoonsxh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ethxueqz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zdfuebsp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3oyimpnfp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3cmlmnfjd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gzzrgalp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3aozbyauu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3czjbigpu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymlvmtho.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jvbjnori.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3libnacea.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhtzgmsh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3oealpysw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qfbibnpt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3luoffgrr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3fugllqsg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zsmiqsqe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3cjzhaxjm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3okmyikso.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zuvrrdms.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ezguhicq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3srodkkax.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ouheidrg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3liltqbnf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vqnkyvbo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3cdsvdxfe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qzeopsmd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nuslcqzn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3monurlcq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vrenygor.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3feszvusp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3hvifiyyv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3uyfnpiwo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ytjpqzlg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3cxurvxze.html


<!-- 参考信息 -->