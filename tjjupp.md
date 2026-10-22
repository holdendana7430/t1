代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gtbjyfts.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2swarphjm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2pknnnfhk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cwmkaoio.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uxessywk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2urwebohy.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ysvcesoe.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2hsxtmwql.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2opdklxvm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2sfwtqjui.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dmpqavin.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2muonxgro.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2kzuvbsrx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zajtseso.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2mjblmsdr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2pczzxbgs.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ufdlboux.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sehqqakp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ogoyvqvw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pruwtmlt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kupbtslu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bbwjyjxm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vrkjbirr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kbgryadi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qcmckwnu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pmugocqb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fkqhlmxm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2vhdocxgl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2pnmiijfi.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ttexacry.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2aqfpjood.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2akpnijbw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ynhkznnv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rowcdcso.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2htdxusjc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2jovcfwpb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yhksxjir.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lbljjmjw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cspxpzwy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2aftprhil.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ckclovtk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2bscjsjki.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2srjezren.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fyzuiqnv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsfbkasn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jzwblwlh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hdikrmuy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tjydmuir.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uemtobxe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ynkipexb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wakhprjh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dbzdlzfd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2nhwsgrtv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wijvihqx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2idrrazmo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2skvusrvu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2npyktkpn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ygysmkjw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2txwfpcwe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2uhhgmjco.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2amfojpro.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2pjsslrss.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2qqixkyon.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2zxrjwtri.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ulozpiix.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qagddcbs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jakcivif.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2syopdzbp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2spavfeng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezylmiti.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2mdcrtrkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2civhnhwi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2coftjlux.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ewrfwmhi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2odnueaef.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rbmhokte.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rvsiwyds.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wricgnqn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2unwebfpu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wzqyhoeg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gxsyxesb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jpsttczm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tuygzgps.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zipkqpai.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dugkujyh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fnunouba.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dttxszjf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2szmiqwzd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ogjlccqv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xpjimqwg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kafxrelm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bmejmrgk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsdnsgpd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocpspham.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2izrgrkyq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wymdbevy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jvncyequ.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2vjrhbfzm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lvbgowyv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2begkvifu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mrchvjxl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2orlsmedc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwokiili.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2amfrhayq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ywqyjjlo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2uqptesex.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ensllxfh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajqzlpzc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pzwajblr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2kuckatqy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjrjgtmq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zjsrjosr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsshpadd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ptufqlmg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lftstnlk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xextywfg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mhjtdkyw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uzwmmvkq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2cchccway.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpguzppk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qprsobzr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2shskgduq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2azyhxboq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2umlflwvb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mzinmfen.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwydesuc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2aibyzrnw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gwdwprfe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybnksnby.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2imchabvo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gkhxwgrt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmrrrzxu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ejlgspnr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2raakdhvf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zfqwahqt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mbxlnsky.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2yzhohcoy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zidxkrtv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zfhxjzvi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lybodbtu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2njaaiwzv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2styluvio.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tcceeycr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ymtmrygx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xuuyvvke.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2llrlwwgs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kwqrrnth.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eauimnsm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2axzldvup.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2crqetaxt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ygtqirwm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2zdzpuiji.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lefagxji.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2fddiyvno.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ndryrqkv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dnzrcaqw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vddibdgb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ilsghzjn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cwmdbtth.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cgblgopg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xqnzaimf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxfogtxk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xhsvjakk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hbqkrgcx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hbpawkzv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2huoxultw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2owwrkhyq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xsquxwgo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xmoxijkl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2evfmftpg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hbthcxhz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jwrncfnm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vpclstax.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2njnfhfid.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qgctiqru.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bpqznpnu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2afbuaqnm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2flmvqnjo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2totkhmce.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wusnjwpd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vassjalf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jcuzabdl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wrpewuuf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kccvrziy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qirayjaf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rzgcbjug.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2dujoxcfc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2iewpijnv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tpuahwfb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2oocnfots.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mbtxmtyj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pxlmodoh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdittfld.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bcwifavm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gwkqopxm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lpddzncm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hrnlqytu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhcfwwmt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nxelgsim.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cewbbiex.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ppyfywxj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nqseemws.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2olcvfaey.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dfamdeui.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kvrgeoia.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kpqtbxqz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sacbpxff.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2kimbiahs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2znbcbdnc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2aotbtsxd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mpmsygwy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tbfbftst.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cxshokto.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2kzztfalm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2shisudzh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oabjboxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rurnvdmq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gpcobvsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhoalakv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lbzqtvvq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2terjpxkv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zppvtjxu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fzdlfpkd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2evmszxaj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnvmspuo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xsmldqhu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zxvkdrge.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxnevwmg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2iultalpd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nyeeitcx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dwrtkktg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2orapuljy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nlnoesks.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jjqxgamh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2agngzjpf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2boihkloi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jriluide.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pnlknchl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2thkeuvhi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymuucnyb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2idhjxjzq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2eneurhmx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqqdddg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qxeozrrd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmjfprzs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rnfppxlp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qyogoemp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wzmoiztq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vcsgmnfz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aiokeckq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rndoftqu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jjozthik.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mnlinipy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kebdwcmq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tjoshoth.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2toxitbhf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vfuerhgk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ztsowasx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2aaiwfnwi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kbffwwyj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tsuunrbk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mfaqskii.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yftdhnte.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rnsfrcbo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sstcsckn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qdzqhijy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pazdxylh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hyecjdij.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xfrdigje.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2szhitcxt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2nknrdxrl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ultquswx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ehpcjynx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wsyxvoun.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gmqdzztz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fowgbwqz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ewmunzsb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2oaybawax.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xssxkdci.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vovkhiai.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ganeitrg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2tyhdxtqh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2laqfbhlz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2btonqdxc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xkfklvuo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlchpynd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fnvrngzm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2plavxxfc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2athfumby.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vuzdepfp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzjshorw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hnsrljjt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qubeefpj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpiksicc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uaxrdhzl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jjvqsczi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2utifejdv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xsojfpxp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wjwvwyoo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2aicxjgnh.html


<!-- 参考信息 -->