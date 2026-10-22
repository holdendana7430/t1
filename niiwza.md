代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2enmhawwp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2zqtpsnyn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2zprwsqpc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2lvvdntdw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2mlvosshh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dzmoeybj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnogkjvo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qsbiapgi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2swhzavkh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wojbdqbl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mkbtkqoy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2amywunwu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ttftrerg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzeleyka.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2cksiffgr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ruzfecml.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qmljldmc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2krjbwcul.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwplncwl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zyawabdo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2veeuwkwq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wuetlstz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2muzslcpm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2hygkvxwy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2htpkyrug.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tbxmcdtc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kvdrlrfp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xinebnir.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qpimolxi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vdhukpdp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2aleijgwf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fgkyaaeo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojsjktqw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nkquhixh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qkiqlqya.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2epjdajxf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2orgmunip.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2omvjejbx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ayhlecww.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ywtlufin.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2nhzzytnc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2gntiemqw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wcfynacs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nzgmnrxm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2smjawuqn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xsttaser.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2eawllrao.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2obrzdwqb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2kthxvwsl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2iuzuhcon.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2udulnjyc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2dqfdjzej.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2yjvtnqul.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2doizepfy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jkfejmbm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iogugdeb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tcwiwqiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddubxgdb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hepbejpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clewbteq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qwyodagn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nszrwxtr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjdmxmqf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uomyftjw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2obhftski.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tyrjpopu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2jspshdsm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ktirrbxd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rfiwrzke.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vryibdkj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2giwnvuyy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jieamgsd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qkmmggvf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oexrtcth.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fhjcvukk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xiquomlv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2iyfaiozk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jnhouvyd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2xhtovrki.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gmudzhrj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uuyqarub.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ewcnvepy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuiwbsmt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zvirlohj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2foqaambc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ssdolyre.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rbjmtidr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dxtcrbmc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zghljrhj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2etfspfuk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2liangccf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmzcbsvi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2flwtvlpz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rezokbzc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2gerdpfsb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2jlxjebej.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ljxbwicr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xqwgqbpp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2knaelqrd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgutmygy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mbtpjofg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdocdzut.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uiunggon.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ykafoiyy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zkczarlk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2prksclir.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2melfeyqu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2aqeajhfr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wxfpvfhj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ngekwuvs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2khgabwii.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ppxgtebt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gwuazrky.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xotbspio.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bhvswwkk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wdeypqxr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlsdajk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gtojjcfl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fvhafpbi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvrpvhlv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zybavmra.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2uoklbpps.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bchygnhh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zzpwhoml.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qpdbdsbr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xsghwbii.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2andwnnyz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rjhkatyt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gbzivort.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mgynxldj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2xfmrylim.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xwcvvrhn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2jksuxdva.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2uxincuas.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eqwwmhou.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yymwkytw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zosdqebh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nmzudbvp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fcxwlbmk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vvsokxro.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxvkqfhr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ycgymbds.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bzuzxqfk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ujczxpdk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pgijcxtw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rpxuexut.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjjelmyf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ocziczuh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmqhlght.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2siddgkpl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tbvaoxul.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jtwdpbyz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lvrarizq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ypwjaoxp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ncqepwtg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ctdlragy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zjlsendj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nifmemjz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ticjwjja.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vnljojyu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2nmnypbre.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qpwkxtmw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eyhcxzrd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hbrzvprr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qkncvlch.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhjcysko.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2jyhisjqj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2plmpsgnx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2joqnjlkn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2seweqyrq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2sdegsira.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oswgvrmv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqycqztb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zcyzuugw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zzwsiczr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gnndvxym.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ggixcznf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2oewoozjd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2vvovdcdm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vhyvffct.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wlbpkwlr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymptfamv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wewykgcd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqcwiekk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cqnbnvbd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nntplpem.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ovfrgutl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dletuqvy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2stuuaqbg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tbpqupgq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2midcsorb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jftaqbdp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vvophoyf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ymplmekj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ixlmcorq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2kftocwca.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zxicsrub.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yqjstlfd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ftrftovy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dswghlef.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ajyqbdqq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cyvkdaqj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kfmbxboc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2aqlktigr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evcociux.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2lacdmjut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jobdttsv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vlhnzjar.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bqndtofz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ifpxcowz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjzghubu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zfbnsgsz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dxsfpktj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vnigpgxv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zcuuzeuk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyevovpx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rkwwmlog.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jsdgrbid.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2adjxowzb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwugxdmx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ahapdbmm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vhpvugue.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2olgrcgoj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vhtuibam.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2lwktxsnr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2gankhour.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2clunlcnq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2xyjzlkxf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojiuwbta.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2llxldael.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fcakaaxc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2upttbhvd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2cejvlgcy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ofigvkpi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ktbxhuhg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ukvmixrr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jpwrjpuj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tzgrvlzg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dykrukod.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ivcnlbnh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2yfknkoho.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vrvxjggy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wytgkbhp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lzgysfvc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xxeqpmod.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2uwrlafpr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2auvmyvtx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xusqhaya.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2otnksyud.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2owvrhmtq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jokkjjky.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2gkalbsfc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cussmulr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2twjcayqp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ouvghxqd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sgpkyvek.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ekvxhlup.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2qzpzcrup.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2aqtoiane.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xdupbubf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vpwnyhxj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pznwskkp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dxdkrdhx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dhzdermd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2yxmgleek.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ojjfrhcn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cydptmdp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2mhqispii.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jpghkgzc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ocbqnrgy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zsjrbqgw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2bzvizbcw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiyhietm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lrjirsny.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2viuxmqru.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wmznxlwz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2gsjysvhd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2lappxnfc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mqtmrbth.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hienfhap.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqaxrcpp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydesidkx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2sbvlxplg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uzmzrxns.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvewjgiq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lhmcljxu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qdnhfbia.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tgquzpey.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iijqvkpv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2pcqyjjtg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2sreiapgb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2urrwdnhc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vmxmisqd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sgyajcgl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xxvwvkzx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2iwnfnipr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lhqhemso.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2hanqlper.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cvvbsylq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kshmeqoc.html


<!-- 参考信息 -->