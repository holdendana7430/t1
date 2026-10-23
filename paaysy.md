代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tbyhllsq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3enesnrhi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3utasgnwx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3raqmbsxr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3iluqmwgm.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3jxuulbqk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zmxgosja.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bzrorthi.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3faitypor.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vikfspom.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xosqtnlh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zredvast.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3itnkebfe.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ypehdoqc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xhhzugzn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3stdhpolr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3jhmwbzlx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bubuxosk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3njnqclzp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jpsjigik.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3sridwcph.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3njrdmuqu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3mefajnpq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3jwrkbdmt.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3sounjkxv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3snxvqzlj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipfbqrwd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hkegrccm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nmvhrmut.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ytlvqrzi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fkxfmuvs.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3odiwxjef.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jqhlvsrj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xaveovve.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3yviehusb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ocspexzz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3byctafax.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3nqwndxnc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3snipmhux.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3woffqldm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3curtmzwn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3liqldyyy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3elfegamx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkyiqdqq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3yogbxgnc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pdfauavc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vhxzmeoq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3afllofnt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ekmrmrsn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3xnzmtidy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3sogewxrg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3geriryhy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mepzvvqu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oisfxzcn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nkkbwrqd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3puebwuov.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3twhtrmau.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zkslvank.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tqrrkvro.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eluvaeja.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zureovhq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3plxxpnfz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tjjcdhwe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3oktvffwe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3gmdzurar.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rlivvcni.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3zeznmuzx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kmybptla.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3zgrfzozj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3liqpqnjb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3txijjzgy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gbrkgjwg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3pmysndcl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qlvyyzzo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tcoflapg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ikduuezq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dstfhbtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bklvfinf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3wvrswdas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rydqixlo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3eofobzsg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3aorkhpfh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3nywxwdsq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dqaidizh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jrdfkvxi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3flcrzjvk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3dvavqueo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3esjbstfs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jcrpxkkt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vqfxusrq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3cfqheznd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjjmvvsf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zuoleaan.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jusqbcef.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gshfliya.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3bgxmonav.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qwkstmlp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hjbtplej.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ighdegwo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jkvxlehe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdpgvfly.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzqjhxin.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3frylaxxz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ffrodrnx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zqnnluxv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3mtlkgxmt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3oaykjidm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nhvirgoa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mqstifqv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3weacdsce.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkursyji.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzxwobbm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3silzmcjf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mubrdumq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ufxvjvbl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ccshybie.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xrhvygxx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pbtkbjqj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3lbxmxhiw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ykxxrsnk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nymalocz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3olufcmbv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gxxpevwy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qhywroiu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdpyduvf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3hixvqflo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3pgenmwnh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3iquvzewq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cezznbak.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnibnpk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3isvvwgoq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gkjtefik.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hoqhmnra.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gesexabt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qvwiyhhx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ysqatwqc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3qffnwgam.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3piwscxek.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqhvaezc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xhlnqadd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rqdeddwg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ovtrcari.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlwxsqsb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bqtdkbhx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hkcqotcc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cjqanfls.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3geutauit.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ituigxdv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pjbjbyme.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ibgjoiip.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3slnrffkd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zlqhbdss.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tnzjpxte.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pesjnymd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3goebfsqp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3agarnqwf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ttsuwstd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gesnerkx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3byhevnqq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ppijndpd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eagttzve.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3nwjbigsw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3denrzufb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3pcgdloat.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3sxccptvn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3labklmba.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kcgadbbb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nupiocuz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3alaehuqg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojvmjvik.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ahvkilih.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bllzcddz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vupyxiby.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nhoggajw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3unzmocht.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bvkmuaab.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3lsfwpfgr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ccissxqv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hdiwtkls.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tagissox.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3manoqsis.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ktsdjhhc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mclizhth.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mzjhetfg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fcgaxrez.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3weyofxgi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3vwxjndws.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bjialqtw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3aqpqkywz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yexejmak.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3syxefigz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cohqqgtf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3npfdgvgv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3arwkiqwc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jkrohzrh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3yegpfppn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rbyntyeq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ovpuyqjb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3sapjrmvs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ikubgfla.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jexbqqtj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpbowfal.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjfmnpnr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wneadwai.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lwsasubl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tizyrlmj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3usysiwvr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fmdsyoyw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kyhooolc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ydvurrpq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3smxhkkfe.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3anqyopiy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dckkohun.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rzdswatq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ttrxvvky.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3huzcoiph.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ayaqmtjo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3iknkjfkg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cshttoip.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pdgwfbkb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dafwjmzh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3sozqukxj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kgpctgsa.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cysvvndn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkbvohyf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lxcpcmco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyxayqaw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vituwdnb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wnpwmvxe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bxnplzrj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3utqwuqga.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3knlmyalx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ntfotnlp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vqdralxd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zblvqmxy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bbclsjfu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hzsgyvpd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mvvjvnye.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dovtrrfx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ahgrttbk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zcpovpbc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3krrdxatg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wolklxho.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3loynladz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3szrdyiui.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vleqbboq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zddkyzap.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogrxewpo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehyrxlzy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vkpykzlx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vopnzdyd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3yelxwkwa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wlepcjmd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yxpzjqnh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3znaxaqxt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3xuazhzpv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3iaoscpij.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guqpujbi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wrgcbweu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uickkhfw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3bfygvcvb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vspqnisv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbnrkpbg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kopzrbvb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dpewagkx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nkwlsbts.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3awqouhnl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xdqhulhw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qsuwzofk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xfhcekan.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mhkfyybp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3swsxzjqw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fbdwvzgq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dmrjofue.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3itpvwgip.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vwcnhwlg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qycrxgop.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dajeutlj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3habfkxai.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zwfvtyqr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vclpdbfd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bssvjxju.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wvvhlesc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3igemwbta.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3cfvovzma.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3sutyqjkx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3umdfyslm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3gflqnlpb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hrbaunfr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ojznuxiq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3arvbiozx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3msuqfgzq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgjxxckn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3owdhgmcr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dkydjpdk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3igsaexkz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ypauvvyd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3oecexfrh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oxyrzaki.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vigzyotu.html


<!-- 参考信息 -->