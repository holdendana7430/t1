代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zkxqionf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fyrfydoz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qqtjyoux.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3msgxdqzh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3jrngtsjg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mmmnhjgw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mewbnifg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xhitbvfp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3odvgwljd.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3yzhbezhu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3yijiyawq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hcdshhmg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3uewgatpd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ahfoerry.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3opdqmxio.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3uovrokyk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uxkrozix.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ildhrfwl.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3spljedjz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3droycwdr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bclearks.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3wmqeotdy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hlqbromb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3uaxacvdr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3bqqnntus.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bksbafxb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3lrjqybza.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3wllfnpre.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3jjskodsz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tiwuzspk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3rtpopnpf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3nldrfawj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3fymufwfu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dukkoofj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jiynfkyl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oytugueq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gstuzkzl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nfvnlcnc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pavocgjj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3pdzfmscv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mmeigedz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3sbkrhlke.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3xtkafvgp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ahyuojxs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zhmipmgl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cnjdniuu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3wgcbqdfq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3khuswnpm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3hsjeriqs.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pqkqugsr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zqimkrtc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3sdsgmaoh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pbxpbuxl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kknynuyy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vnrdnygr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3cjieejyw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xgpkwbkb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vtpuekhs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tyhkpywq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wrgstbyu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3esswotcb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xajxfrpp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3oxikijwu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ffcehmdg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3srlkndkt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3pdjqpmtn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dkjllhgh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kcfhpxoi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jvzanduk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3rgnomfnq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cuplvqay.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hldeempm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3flnxygcd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gcaakbhz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3dnqwhvgt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vukgpeyg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3yxenkyqz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xryiwmqz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ksidwdlr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3vdpiggjh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ouhftjxx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fcbdichm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3aubqqzub.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oyurtada.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3raddrhba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yldbwytf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3sbgswdae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pznfngfx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hqrdqdwf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3svtcdmpz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3matighqd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wcttdroy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ldqppxeu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iczwnnoh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3nxqrypkj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3vnspkozz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hpvqwixn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3gwifvkmm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ruuisurg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3cvvpwdgy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jlumvyho.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ebfryghs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3incoburq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3cptwzbkd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xbymzeba.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vqqvufkb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3awrurjpb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3yvrnvpgz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzlvbriw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kvgrynyj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zytguczp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzpucjcq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lfsyzyol.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3cjjvqgki.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3inhqtwvq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ydiwngjh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bxzncoxc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3cegrbvjn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxblokps.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncmtjnbk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3yjrjamqn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3tynkontq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3kadadhei.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3pqmvkdln.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fphvrmvg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3icyhdcgw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwqfbiwa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tyoeyjjk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsyemwps.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3unokzqpi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3dlbcgpjw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3eoxoyfwt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3phrvawqn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mjhipkil.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3skdtsiqy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3tejcwotf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yflfllsl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vrrqcili.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxamyaqi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pmqhsdvn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dknnjvjs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ygqkvuok.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3sjtnvgol.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahnnrxqs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ljpulyvu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bnjiuhpy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3atdnsnrw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yfllegks.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ljkwcxrh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tixqxxgz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ldvjmlej.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3yenberos.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jkvonirx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jiryktup.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bhvqdbjj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pplyxeax.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lnkujiqw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mgssumpn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3przesaxj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3synqxurv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dtpefjxk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3iaadvtlr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3unznupca.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntomelpt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3akwawlxq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3suyextih.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dpjjlpcz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gbouoyqc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3grzdrnps.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gmjcvukk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wnkyxgty.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbfelvgf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yvjhldjo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mynfbpkj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ojbajoxr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cbzcpqda.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rfhnhfue.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3haebfmbo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3amoavrlm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3iyydkymn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3whfzzqyi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oiusxusk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pjqzpxxz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3obepteby.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3acilflxz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ybueuapl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wjrntvhs.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ajkjlnql.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3qfgklttj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ccdcvhhi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3swakfdhc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mtahispo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mnbtkegp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3spznwueq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nbqgjvsc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nvuqmtds.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mjolkyrn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3resvqhcp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzuvhlii.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3djvummnm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjgiejrb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dvwwrblc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wvrnhrju.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lltnkiaa.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3dmdtpqtr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hfbqkvmd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fskymcjz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3asshtqqi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3miwljabn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eiojphum.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wyjzmjeb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3liezhcuz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3okiqxpsb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yyquqbmg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dvoxulek.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zymxjyoa.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3pgelhfty.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tslxsbbf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xpxyvcjq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zrdrjnyz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uddkgsfs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vvluksxt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wndlfjrw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xfujzyiw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ulvzbeke.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhissbyl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jrjntcze.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pxtljurn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jrsvkwzt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lgvwbkvd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cwobkilz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3drnpvwsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dycqnrtj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yihdyhkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swsgjddm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdfmuegw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3koeemiqx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3quwsdrwp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuxmnolo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3shioluiu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jpwvpmrq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qalrmklp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xhgffqdi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhrfmulf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3yazfjbkx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3scknaaqe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tcwxqkxe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzwwjdfy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwfiztyp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dplvdxqd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pdhklygn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3sljjzvbh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3avgtmcmp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hgcdvizj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3diwitrco.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmjjojtt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vagwvvhr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vpzoppot.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hswddjsc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3muqicpsq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3axzexlhq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3cngskuga.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3soolasax.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zwipxllo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3yanvfacw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ckwplmls.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tdkqnbfv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3atikohpw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qupniqfj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eafqloqn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xcnbaqbn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ppntirec.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lanrhvvh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3edlqthlh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ucuifhpk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ajgoisid.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ljzfyndu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ystoqlsf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3hxtakicd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3czvbrccf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3oquvvdyw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3zqtdzgtc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qorzjnow.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kespysft.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mzxjrwlw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mapvrzkh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3lstpdywn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3qvislond.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nqkqeyho.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3drkxnfpc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ydxflrxt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xvaqfrza.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pksujcth.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3oszcskux.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fomtaqvv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3szyuxdvy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3bcvrocvy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vrqgjyjr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qujcpolc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3nsujcdhx.html


<!-- 参考信息 -->