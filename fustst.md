代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsprsxcu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sfightix.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vbwqvydo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ngwtotne.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3rfeqhyjf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3sqndvvnw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3uajibabn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bzbdcghy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ldyotzwq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xdytlsjd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3cwscjgez.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vbwuxjji.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3yndynweu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3rocbkwvx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ptlpfzwa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hpyuiudg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jboddsyj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zpliflys.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3yfeltttc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cmeprwxl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ytmidwwe.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3efeepgor.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3zbrwhwuh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jwzhgtyh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3tawmyzjn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3sspkwzvj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3otobojil.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3rxivwmup.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ldnwvjce.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ahcahsuk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3swgwjahu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3acavvuel.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3inrvdmxo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vgiguahd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jcrhbhdq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mjmecmzx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wudjghnf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pgupugyi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xqexorso.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3giyutvtb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ufkvtpuq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imdxafbh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3oqodvxly.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3kjeqtbzg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bwwwbplk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qxdpjhrp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3rrhhivnh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aiuxkoaf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3cwhfxpbd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oddjuohu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lasakyev.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgwmdzpi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ekhatzmx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3froarpmq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zbkmlefk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3nrzpviqp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jkuyzyra.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3tcstcolq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mtxgidnk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3acddojnq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cyhjhgzt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dxmsqnxt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qcmtvtkx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cpetqobo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3paifwjbr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3nnmmdhcq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gebwpabq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3guervaiq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3wbnvwirw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3evociqof.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lfughskw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhvvbdxm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3luwkoste.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gpailyhn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3cxvghvxp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jukkngib.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3brbzzzei.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qyxqvoaj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvzyzqp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jqobpxio.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3duadouic.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tvcfqkza.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3cnadgfov.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pcikdpdn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jmuwgyff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etowqdxv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3aharzpsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csqpyuwd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3jekpkoco.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fbjouiku.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtuqqlkn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jyvjwuds.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hlzmewld.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gtrafrkx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3vfcxaccq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tmrkprpk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hsxaypuk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ctwqkcem.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3igovcpam.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsbuudki.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hzbwyqcu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kxqupzdk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3saoyawgp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3elxqlhja.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3sqdhokli.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dlgjamiq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3oazajiqc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hvwwvhqy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qndydoei.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jianpfze.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxrvoomn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgrigoto.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ufqeratf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3eejrploi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qmkpjkad.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kjghfhsj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dktopjrv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bjgwnioa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpfjqsbn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgjanjih.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3aqanbyuv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hqudiaee.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3dffkhlcs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wegawxev.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bozfupyf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bqweukpf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeesjywl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmuuierq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjxvguwl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dghgkojz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ulqqhrgq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qijvegkt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3taaeepde.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ohjlwyxa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gaaybykg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3azccwdiu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mdrfbnxn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmdndjke.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfbtkexb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3oforhvla.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3cqzazjit.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3okgqtqch.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xuxgtqkz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qtnbiwlz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3errauiwm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3junvwuho.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3maexhjho.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbutoebw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3sioaiqbr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lmzrvjtz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ngbzyozo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lcwispnr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3odioyjnk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ivvjeqsa.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iiuaqwqs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tbdkltoa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3svkfunkq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cpbchupj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vgczilru.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yhtdliro.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lubuerhi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3qoeogoub.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbzonpmk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yloiorxa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3stkdwjqx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmxlmoug.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3foyeqdim.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3kllzhfnl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yxaoplfc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ubwtshoz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3jhjxykav.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3pnmshbpq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dinekobh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lypdgkjj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcvbgngf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qofajpat.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3glsoxlaj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ggudamlh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nhjcqbud.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3hlbusfui.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nhnesind.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ekzxgxbl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lbgfmdby.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dxmxfkhe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3flmvvsfi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3baodsufo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3mipqtpjz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jsmmtywd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3krltjgbi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3chbinhku.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cxapynch.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zwmcfogi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hpdhfjjg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvgfzjbk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3gcqalmwy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3kjxkgehf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3famdptvt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3bnjptmgw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3avctlqzz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3twvbodvv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3juarxnlq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ekjyzuoh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hafibyfd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqgvjma.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xncxxxkl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3jimdhzqp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jyfcfwrm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dlnxsuwv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cypjzcvn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bckiaxuo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3geczdxqn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3siohnacx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tnlyqvip.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3scylypgt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gussxajk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zbxuputf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3deruulqe.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yvkqjcws.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tjmckmpd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3quahrkvu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hbmzusjz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ikgalowe.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ewmemual.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3sjcekmpi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3mlwpibsj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ukvobxra.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bmsirjna.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sbqrqkti.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wzxvnkes.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ejonxwpp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ofknljpb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bhjxyqzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcotramb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ecxllfnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djoqvjov.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gzhqvmvc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dwigezkj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ioossglq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckbzxtfs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3psfbnkul.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uphltnvk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fqvkgevi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hrfxmkiu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtuyuicy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tkwkueuc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3olvymuco.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khyopwrx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kdcsqxuw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mgqbmfct.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mfkykyzj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3voxxpbrq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3vwxvmvsz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3znhmxdxy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3xbyxjtwl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gtoiidtq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mjpyomqu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahovqgrt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jzfmwrkp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tjpdekvw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3iqkdwkcm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qnkobogx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3losdwssq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tbuvtwro.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zsqfobmy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xsrqgqeo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bskwgquz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dvfglbag.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3yrjnacfx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ouyqqplb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iechzrzd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3boxejlrz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xiizfylh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rwccetlx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3goaxazpk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tugpboki.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nprqwonw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qujvnmkd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ihuoxvsn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nbprvwlq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ueanaqes.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3klukmsiu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fpyrbsml.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3neixsqcn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gvkhdbpw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uqvwabbg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3typmstzx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3byovzrrf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kllzcgej.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3onckwkkd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3skhfigwr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3uggzhbfr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zqxmtivq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3knxetpui.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3foauxusc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fpgmqswc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ujkxknzb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3paeheitb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3nezibrtq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3nmnipcvu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3iyhnllyg.html


<!-- 参考信息 -->