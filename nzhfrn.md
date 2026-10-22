代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2logehkqy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2atuglmid.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqtpytw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2oxknfbnr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ffztkyky.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ejktxxfr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2gvxcghcg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2tfdagznh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2dylzlxoj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dupfnfrq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ebmhxmdt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2aqwrvcne.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rmltxxhd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tjkxrvoq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2axmexwyk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ikuhmlxd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mvpbbkxh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rmnxcyqz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2busfckit.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2umopfniu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2bexcdaoh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zgabiumb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2halcosrk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2blwwrtoq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2faegiqnd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2dzjlzbmd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ruvincig.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2uymnpsan.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zcjeougo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ayxbfagx.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hycmqqxe.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbiyllrc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bajzvmxm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ewuhnuff.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yneszvnl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2mkxxmmak.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gkdfrqsx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2kyxrfkfo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ybelsjvm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ivmqdzrs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2kvlpyhpw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fqejgush.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2npvlnstr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2gcmtikvn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2chhppjee.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pkomzisc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hzeriolw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzrjtexq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jzlzknzx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2miufqrrs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ippencol.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2gamgaaga.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zcdfrqhz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2uyrggwtw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vyxerpaw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ocoveewe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxrdobld.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mqynhrvi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kabzzfjz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2fucdqoug.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2gkqpltzs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mcuorgtz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wmqtbawj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pnhpklqm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2opzpjhye.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2pdivnjgr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2iomoxeno.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pegdpcue.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2sjmisarp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsogimnu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2wqxtntrm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqvajypj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2zjasysdd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rlxegoai.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2gtdmfwsg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ykxrhcwv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lzflbfki.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rihyjlyr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kcfnqjbj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vyvlpsua.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dnusgqcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abgkexuj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ywjojgkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jblbftvr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tqrxoumz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kknwfwil.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2fecjaxxn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wnnadxiy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dbxxiqbq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rypjpohk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2agbvjliv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2iokbxkqn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cgaeejvt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ndpdpmxm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2glvrrbmb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bdkrtmgm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ryqerozg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nqvcmlmd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dtdzmjaa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zebjjoht.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2izutjxan.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kydnwnmw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hkfyluil.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2sfzzbzvm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntmqpeig.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oigfjocg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ozgyiocm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ohfhnrwm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2orjrjnhm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bobxwhmu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zuyuwglx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xdvxpsvq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rarljnhy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jmmuedwd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrhvpmod.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypgqixfx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2unhtwvrq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2mtxjdhok.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ccvjdjub.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldvgnlvq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kqhqkuoq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zpxxcxgm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2iwjfvdhu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yopvbsjr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2srihsndf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eakkebxb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2mestupoa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2umgcpisp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hccipyhb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2dqybknbn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ytgskvvy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntlasxjc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mcppcfrh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwupvlyt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2aanjcycg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zsgfivtv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2icptevui.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2irasaczv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2cuqsolld.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ruhxfzuw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tluiwqwq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bcngsswh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dpgzvalk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvjgpnff.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tovyzrjd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xmjqspdm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zncvvyxa.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2gvnfjzhz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2kabbtlte.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fszjknrs.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gbgavgpl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ivyunkwi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aogwhvwo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dtirwkls.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2wdlyosbd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xgnyjfqm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bogvqofp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2owtulqyz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qtdidarw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2alarkfco.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cdkbweuc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsrhiwxv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2sikcfueg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2prvumijj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wyysmbmv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xpuidivr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2hltromfi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkuxldsd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2peccyvre.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cdwyinpp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfqomuil.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bzlosxtt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2yfejctdh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ledsdbju.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2pelnhglb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ldiwqqgb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2smktnrxu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2idiemejg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mdbuorcx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2odbjodgh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hrjthtwg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rerkzmrt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nkifeohm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zctazwsq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fsnfndvu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ugnlruap.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2taakzyfc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rdvvmple.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cqehtjav.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lqznaske.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vqfxmanj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2fxzcljlv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dgjixcbv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nbdoswoq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwebipzs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2arpjttkj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rcboqgzv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zaljkpfs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2mflsweeh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2kbeaftvj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xotspxtv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2prgpdrod.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wxqugyxq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2jhknllpz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2idjnpnek.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nruqlicp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aywuszoj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2tajybtog.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gewzghbi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2urzazlke.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vanduytf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gbqlgpac.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gqousczb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ojivltnb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mxiyadyq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aktnejsz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dvindzfj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wcrlhxvo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jdemklaw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ixxrjvbu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2stjxzgot.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hskkjvvz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zulxoipo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xldkmvdo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rzofathj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2svsqfjdq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2xksogqma.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iwkbdxbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulqjdmls.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ehjjkmwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfyniego.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2virlqqnu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pggkgqfw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yhtijziq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ilyfddnn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2luaoqeyd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtnpjvlf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ukozlsiv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2bgpwcqnr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bzntmrik.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2tctlczsk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wbeonxii.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ckwqedgi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vqropbbr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2capypxrt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rvosbbzp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2mdhcndpj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qqmniovt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hvwhpimv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ymrpxkqw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdvnmbv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ecunellt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvzhmjad.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vinaznlw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lodaiyge.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lurcidus.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ioalbjsy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2aflznvby.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gvajppiw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmxkcoka.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2asrhnxiu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgjoaijb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gkekehmt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2yhazhump.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vlcqybwl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2emwckojf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulfhgjkt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2arounhef.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bqjdgmjl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qoigahzy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zlsapziy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gnvmsdyl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gjnzkton.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2raycsaiv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qvzgxczt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bobqzuqt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pmquaqlk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lfzcxhva.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2bhjyddcq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rzwmlggo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uqopfdzt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vicnoonr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2karuusrp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2plkxcvzw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wuwbssff.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vencqswy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2iqgmcgal.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2owmhflhg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2enjnjwek.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zpkewyhw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ertmwttv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bllsoewg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jtmmujgi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ofmqlgav.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ybdettvp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2sbrlmoii.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcoxoziy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvhfcvsv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2awieydhl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2dozsjdaf.html


<!-- 参考信息 -->