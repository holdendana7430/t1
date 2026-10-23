代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ksgvrqlk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oqitmujm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kppqmlwa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yokmiedf.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3aopisgjf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ivtwggpz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nxxqklkb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ebccwsyw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yjloioty.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3rlugfivm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rgjonicn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3razsvldn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3gehayiep.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mmjfepgj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cprvjkkg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3jxdnhgqq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qdgqqhpm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ytymfrhc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3zpaqwfpt.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3buwpfsuy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fsmoyemi.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3upkplgxr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3mpzcukis.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3jlcuhynt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gsygbrbm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hpatejcx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ekmzilaa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3kyctomcd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3knbaaavc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3pspkygiq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3jknpuwla.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3cxmdjisd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3shjmebsu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3grtzldym.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3woazbhuf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dyrvmtcg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rkxudnlw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tuimabmw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3czommney.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3hdmadmkk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gbfhughp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3mcwazgwn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3qourzyzv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3vcbsfyzq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tqttjnoj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qtvpbepe.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rnkbukcl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qbhwtfxl.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3csltzmvp.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gsicfrrg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wibasrvl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vqxgrnvs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3frpjveda.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ozfbjfyy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3izrcgjob.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3thitrzik.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vmhaxxyn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3bherpswr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3mkysizmi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ozbpzplo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3hqkjhzze.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oekoislo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wrywqtuu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3azvnmaap.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3qoqlpzdx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3opzldmvs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jgynenua.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uohglord.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3kwoflkba.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fheuaurb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rpwugjwr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ayhoovhb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3kuffigum.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkplkedr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ukxfblct.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xokhvtrm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3esonjocd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3egrcmtcw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3uklmwzgi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3wcqhpsoc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3nnxvzqmj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hhpvjysf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3wopenrff.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xohmsbtv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3anhekluq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hshlpxyb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3gwhsxdqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdeednxz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gqwihgob.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3hkictbyv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrxtijk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qjtyuqyu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qsbukiru.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ydfitcmo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pjctqdim.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3aqfrhbuq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zctmoqso.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vcpfdwzv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vfbgxzho.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3sdhvvdus.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ewgdemii.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pjyrfhct.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rgkibpjq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vdprgkqn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zolzghaz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ifkmyjuz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3iiqwlfur.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ktedbdxf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rejqkbkj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fepwwwhx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfhpwcdh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjqjtnlo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sovvxgtf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yjrohqvp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wfhdxwbn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rtuaisnb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3gueetebh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnruiaag.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ydkvmnpg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuwoytsm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gnwsyplo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tncrranx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pjmizqkz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3xnbpreyf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ctckbxeb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mwzsmozh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3gelfqdyt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bppnprjz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3noqfvgsp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekqtcfwv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rpbhisak.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vagckmer.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmquzwlw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3cjmeqtvz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rhfnadus.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3onrgxfpm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lvsebelb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jisllzgd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuaygntg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qopystox.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3usuorkyc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsznavyc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hwnknbxq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3lmiwpisc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymfdrdkr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3azozjvmy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gpkdlket.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjmbmfse.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xhfkklcj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3siyjuild.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxpbfmff.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3rdcogosr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3auglfugi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vzuaztpo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lwqnnyvz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fkoozbvp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3karmwhjl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lxnngrhk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bmhnpwxe.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zkoqpnni.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lxzsomxm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3eyyhluyu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qsdgfkxc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeeziazo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lhiqqdor.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3najuckml.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dmvefhua.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nlwpgtjs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3quvsiyif.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xebqfazm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvrxryi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebavmqzt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3plrnwgbi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hzwlggqh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgkjyuwd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xvrshczt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tlgtwuym.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtnqtqet.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ympyzypn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qrbvmmsf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qewupsbj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zifdeshx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kbwaiear.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3acdbyxiq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vxvfwvpl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ywlsfxzr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sbqdcmgb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ourqfurp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3enskbjus.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3kixsfhsh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ttuyjbjb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ymigflff.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3afycbefr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3xkdtogcu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xoolflvq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3lmcqxisq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3naiuyvve.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3asnxwtut.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwxeawix.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekrjeasb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rbmhgogi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vohcubti.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yjqwwnvj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3pglyibvf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tiypoldo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jdfhshkc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3tnzzgxaz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wjbjixvh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qijpsqjf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xyeycrfo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nqhuzbgw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3lpnfsbzw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3twkogega.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnrxvreu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xtlexgzg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3keleqsvc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qiimthif.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sjolxvps.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3olklnguv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jljcsndu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xlirkhyo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bymataro.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dwufuwtf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jbodfgug.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3guxhfivf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hebnrlem.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sobwpjxy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iquxghlx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wejtfzur.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kgnhvjqp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mfxloxjs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mwogczvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytbpbqax.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3czwgcveq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhvaujso.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ffjagtco.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jwiswosk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xgbrdxsy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdzxnmey.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfceodbl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jpehxxib.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lanjgyul.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dffteuaa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwlxkmpz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3pykhwtbc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zqvmozbv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sekmjwrs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfyctvtd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwdwlylr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3upzskrix.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxcvbiey.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hvrykglv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wytklwkd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ogtdciyd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zpnjyoht.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfnlipit.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ysvemzdr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hxggdqna.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3avxtqzbq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3vbiczvet.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gnvksxpd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3koplqoad.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3iqhehttx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tqlgxrvc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3lwdamamg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugnrbjhw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rkuwelci.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rlalnmmc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3cfpcwfan.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgsksqzz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3obluxioi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pitimqxh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qqngevgt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3rmevuuij.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cnqjsieq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rdvvmqbs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fhqfsufz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kkvziqxw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mxaiysbe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pghclokx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3egpoquza.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3jtfpciiy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ykthldsk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ejtczwzt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3janwmnsx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3atztykip.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fqemtrvg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cuqktitj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gnuuhkvd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3eaurkczu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hcpagvua.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qpgupsrk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3iikjbmhp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3vsisjelm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3csjclcvz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wiwfykpz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hxrbdygn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3btgzrpee.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ucuzwmqk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jjzxskox.html


<!-- 参考信息 -->