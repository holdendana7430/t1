代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2eblmncbv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fhocicbx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jhalrsxy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2owjfathp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2cabuqdyj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2bigcddje.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2jypmetxr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ohkxrthj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2yqrwhojv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2lccxjxjo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kscsnaky.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bmjrwqsz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jfmcqhqe.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2vrxrvpxw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2dqtxoovy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ggenstme.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2pyqoqxuy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2gbdepuzd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2xgmynmhr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2thcrvidf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mujfulis.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qgsgvooi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mntlebid.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2mpyqicur.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2anuayeci.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2saofukyr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2prdfrxlr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2frtjhwft.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2rvurzlof.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2olhtzdhc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdehtczj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2abetgaqp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2blgtwznw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2inyqdlkv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rrovlmoz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qctehcmp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bixsgxoj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qyvubfbq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2mxvfwhmt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2uvixzzzv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2gbgzwpqm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2tshylbic.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2flhqvyil.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jdmlrgea.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tqynywad.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2okmtuycs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2bkvxqqmb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbgguxvz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ptkiulxd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vujptfta.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2njcbbvrd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vgbqbqya.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zltiutmb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zosvysrc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2drxygilz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2lgahbwbr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ahyaeleg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lwtskrna.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2daxheoub.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2lgkltdmv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ontzgrss.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jzdnlugz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2numowgqt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jcblianf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2lhhisdpl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kmoeuphg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2uvkypnyp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pmvemhpg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xzffcklw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ofomtcwb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ieqetura.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2sdgnrhwf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2moppiyno.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zdgngiwk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2lvqmmbok.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2idwdpqrx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2badfdbzx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kzfuxdzg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2zmvsmjoj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2arbobgws.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2brouegtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dptwzypw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2kwwajmlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvezjazk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2hwaddjrf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xpfttlir.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oupcchjc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2grmmnlws.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ivsbtkyc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2deunvchi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pnefqjtd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2hhjpowln.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bxoamtuy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xkdayaor.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2qxbtfynd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2idyakehn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ntcfogun.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ngkyfiqi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vqctbdbm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xqlohxwt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dbnqjgbl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qwxsmdgv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vlsuznji.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mcynmpre.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2brlcmsgq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyqrjyys.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ovsewhuj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvxqrdxs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ufmkidzl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pjxujmho.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2knwsakci.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2knutquav.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hxibxreb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2yemzpavs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tindgsvo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2chswkdhz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xyxwrgek.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2cshbeoon.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ffbtcayo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dpnwdotm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hnrtbbcj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2boyapzeu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2uovcgova.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vudkvhxw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mihukqcy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2flvifoqj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gbvlnwkp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2czowvvxi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bskuegis.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mqbcntmt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kicawoet.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wiianmyx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hfmaloir.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mepmvqgr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkojolox.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nfsgdipa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2eseihstt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wudfaovq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ujhudfde.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zkpswhgq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2afsgqrnt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmdjaiut.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zthelkba.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2drgfxnhc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kjdvpezu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2trkspffd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ydfwkitq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2cmogjivt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pnwabkep.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ntmyjzru.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qgvrcarn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2naniitjb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jnyjorku.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uqgszhhk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2lqvtnvnq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nlhkibnt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2yaszuxua.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2simkfosy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kgrdbvig.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eslmqiao.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hdpujyme.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ltpvnfco.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2taoqgbjy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gjrxslwg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ilztxikp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2amsxfxbd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zxgkaciz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykdbizzl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hsbpvojo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ufgosjed.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2esrjfbqb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tjppnilp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2lwrbzabh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2aamyaowb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qkipzprd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2udhffehd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cdnilpin.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ztezspcq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zqyhaqbl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2suogmhdv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2mxhhgxkc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2iphdincb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mneunnzu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hhqwsook.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wdoebzdp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qqdrnrhk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzufjiy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tkgtpgut.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yamvsdii.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vysydjns.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2atmrptwo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2atflblra.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zheeoknu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bnuetafa.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2cszhnwnk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mkryzlht.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqvkjmoh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2hyyrruqu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tkwzfduv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2cdwstipo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ptkudgrf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ikheqvvy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ncvyycnu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dinfmjbs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dacbdlhx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lfeygyeo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jsvyrxko.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2oohfqffx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wnpvhyry.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjjgyfsf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2fcejhlbb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2oessbwkg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2onsswuek.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wrfcfccj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ymantpmi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mrkfgnji.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kzqcgcwh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sydzzeub.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2devvwnkn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2serotzhr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ukwwuyna.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ayjcmzbv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yteeodcb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fazlvmol.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rqtuiaoh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vmkdzjnn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2bmdrhssj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ugvpduan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlimhirq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vamplbaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acjuwuig.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddpknixo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2kpytdbte.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vlvdfbxz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vijeacya.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nlqatmlf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjebooci.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pmcvdpua.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bjnbaobu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikrtwqps.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xnodlwav.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mkbcgrzd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yrttbhjo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2suqjzyjb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uklwgygn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jnxbjgqo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xprftods.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2guspufuc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2bskjwhrm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2remjjtoy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2pgeeiqtg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kfnireue.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksgmjaru.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihcbwhcy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tobhylnl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2eduvpzne.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vthhldwj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wekdtjff.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rzkajrie.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rspqftnw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2iiilgqji.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2datcokmu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mapccjhw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vawtlzzn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ykhekrcd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfrummy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2udroxwrt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vslzzrhp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2eqpgmefw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2sheiijbd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hhafwvbk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2crocspdu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2edsxsftr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2racvddnu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2cqdycobl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2eqxbaimc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kqlrqbjn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2omigfkos.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2agcxxoyk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ihlwzfit.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dzpddilo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ttlfahdd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vlbjjzzl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2fpvkmvbd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rfgyszzx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pnuczphg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rwnklbdf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vlgkledr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2crvfescq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ikkaotnp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cwtslrqp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mxskurcl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tzumljpx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hftfrtas.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pbyccecc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vmaowzxq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2pidofmot.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2svqzhqwm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cagfcsbl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2osmntjop.html


<!-- 参考信息 -->