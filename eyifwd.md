代发 wailian999

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mlfykpwl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmjxpmqo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jyghuunl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2cernhuqv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lergaghd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2uqwprpnt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2blhonhhl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2izpparrn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tpmxmvlz.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rmawwqme.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ekeskpgw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnpcmjck.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yxctsvhz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2aiuvvysv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gbvuesdg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rygzkgpe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zcnmovjd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2jxexfizn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2galoiqxi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xprzwzim.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojegjpfc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rkntumxf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wyhcoajh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2yolnorou.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zexdrbhr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vfurjptc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fyokfusn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xvaeatas.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dpbluxdp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrcjqyeu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2srnourbk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmsqkgfa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nzqwjyvp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwdfhwce.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vifjksns.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2otldjpzy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2lkadvsge.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ljenoiea.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2lssvfebl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qytrjedx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2njpgxfjn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ocvmvbbz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2datxigyf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2snogrthl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nfoxkipa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyhdprgy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zsejqmgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buqvexzr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2wsdljicj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wjyfdewk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2yztotuow.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2favzbgsk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jqnauqsw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ueuohupd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2vtppzzxp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ghjhhooc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rphirrek.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2swbkgbic.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2lticdevd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gnushogx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2losuzqto.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vdzrpuzq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wwwicnny.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jjewztxd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2zasgbbkm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vqwpdgje.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2bmdhgcom.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2dlpltzja.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2epoeznyp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlckejas.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iujwvbgb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cxycbvnq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wajyolsw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2bolfmssu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kxlmpnmt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gtzswuus.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bhcaiswf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2xlsmqtme.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ualztqou.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzulqaap.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahdfgthr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2riwdskms.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xxwolvpj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cckskfmr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ctheckwc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mykpkqwe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ulywdhjh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2njxqzknd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffcpqqut.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qgtqpqpe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cuybatbj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tbvigdkh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rtlwbkda.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ghoojhfc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2chocedro.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2khqnmqyd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqqdfmte.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqzhapom.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hrcieqsg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2swefsklp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ovinmdxk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fkcwtknc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2iunuohkw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lokffnve.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2abjdlfby.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pqldeszy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwrnlpkh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cjfhkcah.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fmxqdnmx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ozidkvgs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dlzvkkmt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2coylfodg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kknilped.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ehqzsjgh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2flibpdgk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gfkvsmjv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2clgsybvw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mbagepuo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2osyxwrha.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2toafvznc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xeqexljd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjelhelc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwwlfcvz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dkgqsamq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2altslgut.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpehxzar.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uhytowjs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ehpxijut.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ggcdntfr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2htknrllo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qrqspndw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlaeblld.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qkzumtzb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nnzlqlrw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pitbuzim.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2sfxunvux.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zcajozhv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzomdscn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yjjdsiuu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lvexwlpc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vyanwfpd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pffkzjoe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rtarjzqi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xrlczzxl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2obqcdeow.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fhvkuxxb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2aaitijni.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cqjmucvv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nfmazvrv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ttxaarhs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2samgaddn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tmwksxqe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uaugyemc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rkqrdeqa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yvyzxcip.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gipleakn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hubhnfvm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2nardxgmj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2otcsjvbw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqnfxrwf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ofaitfjq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ekuzyhzo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hodparsa.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lnossjvs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2atkpwbpb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2cpyvbrtr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2plfjcbax.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2iwxdyqsu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2byoipljv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ymewirid.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ljpzftqt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dzmvmbpu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbmkmpfz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2haeuhkxc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yqklbkgv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bznrqhji.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nkyxytjz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uvjjklor.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zvjbtnkh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pfmsaowo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xyeaptvg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2atzomsfi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kgzsypdu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qacjcedx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jegafuam.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrbqexnk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aekyhgqi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fdscxyrb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qqhqumdf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hwqxnodd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2pwzzmzwj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vphudusb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zngnkzky.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nkymqxae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwrwuanu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2abbjxzkv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aivmrqmx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gvzzmgei.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnonfrio.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhwixxje.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydtlmpbb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2onfnpaom.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2cgfddymg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iarnnuvp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2oqfvqhpx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2peoprvti.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2whaawhtg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pdtdeswt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jgjmfyjp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vfhjrxua.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjrzimhj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ufparbuf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cnhgothf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2himqdmep.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zducmxod.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zklwkqhv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ywjicufo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aiyhoahu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mznxkedp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qxylnpdb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2aeuocurh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xorrbkco.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqglhquc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jbzorfpm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hucanbnh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2goscznow.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ihoiixns.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qxqakmgb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qgiimoap.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vflzpuyi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aztthdak.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wzcsrrqf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qiumngmw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mnlmygiv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2whncynhc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fqhnlwnv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hepqpsoz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sdxtlatm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rolciglv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bgrouyam.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kluuzqtn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2msrholvw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xvtrecbb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mcsheksf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xkceeegm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nprmakqm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qqgxjrja.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vzdycgee.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gtcnttsy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2nvtismzc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lruxadfb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ihieuhxy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2egeqptpq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2azvgdvxe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fypvhfdr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2gvvitikw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ebeeigkt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2bitsrinv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zhplmbiu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2tmisbgbi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjarbiro.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhmjflnt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkezrhju.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cfkalppr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zpprtbzj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2xrqtyytp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qzkyxiek.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nwyfizul.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fdyfkuoi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zcykdveu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fbiytgqo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rsenoory.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2doqxmmgd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2bthijddr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dvhxpcij.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kfznnwgn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uagaqznu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2klywcjqu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2rfgswuyb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eymfwkjh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2usyxsmbh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jozprndk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fvwfcflm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pjucijpy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nzcimsvz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2hpojzvma.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2odfikkmk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nqvepbhj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sshnriiv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2zcjuywua.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2eupmjpoz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2uxvyupkh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jxyxwuvo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pbluerfj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2etbyggsu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fkffplfb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wpzutclk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rswuflri.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jerdsdzj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2sutapuzq.html


<!-- 参考信息 -->