代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2eehlscfh.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2taiqrfke.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2orjiddfq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2uctnutzj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2dzobyuel.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2yccrkegk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uztukucx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2duuqxsbx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xngcgpsw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ldkosupm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2scfmhknm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2opelnjha.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tatgqcsp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hvpvwfyi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2torpizko.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2uxertzyv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2qpsniosl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2aefpbaxt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wvszgdta.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ohroxrrp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2xplaveqq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gesxcbxy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2nepvolhn.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2hzyxoyhw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ownhfvkc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vzodxvmk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pawdennp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtctwexm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ilmdbkps.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fuwmmvyf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lqwifqus.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2oqpbfsnx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2amzfwwmy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2omdmjhoh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2axeawetc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zfymakha.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2kxvblpkv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2hveksoxd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwcgqocs.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oodpehag.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ggaeimhi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2apexmloh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xbhayzws.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2aquwtnoh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sbipbtud.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2itfhbzcp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pxkcyvog.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwfhpxnm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lhdwyuqh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ygsajwgh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hwhenocb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ejxxdqby.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2uyxzjghx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tdctlwid.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2aendibkj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2gyghystx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jsjuyimm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2qpaiaoul.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wrsoyaxz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hktquinr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ycwslwkp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ijlursdk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pnmgfgeh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbvgramz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2lasxlhnz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2uszsangh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ioznwznm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkcfmoy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2btgsflua.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2oxraxgji.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2qpebawqj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2fuplckvi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2bvilsnoe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wbxtafkt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2yznyfjna.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2iqimcbtm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ilxwdedi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzjjenxe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xtitwate.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysxfndcz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tkfmaufc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bxgeileo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2tqmxsrtm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jafhdoof.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2auikfiby.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aousctvl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bdhjbeio.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tocunidk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qoedqlsx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2lgqbiesi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2skcwtdhe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yukjexzi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2womonugw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nnnuukjq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2veerljqz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2gujcette.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nizyyyll.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xkxpzieu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kljsjamh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xmqpimnd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulwxmuyp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbwiaapv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cwlydutt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivypzquk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pzrybpxj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qjysngsa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ipdzjddf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ugnrwnnr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xytqjfty.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2marmzvcm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2psefauvn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zyusjkfj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2vrlrkqdl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lmhthunm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gtmzxgkt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ibgxhgnw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zftcgtsx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ekfcvuvj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwnenhwk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwxjklon.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tcgufplc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2yrgqswsq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2owhccvdh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xytybjna.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptjftdji.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2dbblveyo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zpcnzvgg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bynelray.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xprsikuq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2eexyvnzs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hnoonkfg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2anozoaje.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2csqtuquo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zuibxzwl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gdvkxktr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yltthztx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldtzszhc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aitksbdg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bicrsuxr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2roysjiiv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nzehednr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2mhjzijaf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2llmkczul.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2cxtjvqgz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2idayiktk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dwrxmbhx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2otmenhty.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hkjhzdpd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rgzmixss.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jaojvral.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rjfgwxoo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bevdubta.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mxnkprsl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2gsolxnhj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mgxqtjca.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtuptwcu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywppvqoo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfhhepia.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lghzndjw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dklyldsj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tujrgopn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2lztmmgep.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2hzgpcnwp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hanuyhlh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mmzrcttk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ugvllncb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cllvjmtg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wkijublt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hbmikdfn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfyiajkb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tndlzvza.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lkcszpim.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nkzebwac.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tvrafpdc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vyjmkvku.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hnuxbfgn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2thnuefgh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2kzgjemoy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2joaiwphx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qfmzqore.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gjxfysmb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2aoiqtoke.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sqkhkpyp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fkmfhmgn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qpcnzajn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2joctswmc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lhmoujzp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2iaweispk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2fbfkxvsq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fydkrpbz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2npatwing.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rrzrleee.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iaaohijp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ctaxjlta.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ewvcyini.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pryewbog.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2awokwyoy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2patsmkkn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2syehkpcl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2qxecoixe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bcfrwdpa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hwhhtbps.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oqzjyxlr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggwwfsrd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jewpwmnw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eigwplho.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vqpjrjyz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jqohpaez.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2roenmbko.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qrsfaroi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2akjypmtm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zycoofmu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2edlfvtsh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zlcyqblw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mixjaayf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tglipcug.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2uowuqwmk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2heoyelzq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hhmaacak.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2eorzrdzt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lcvngkdk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2mdmorxwy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nsrqpuwi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2oqxubwss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amtkfirm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ruitespu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqbkyrnm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lmxkutlg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2uyofsbmm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wovqboex.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbazefcn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hfruswmb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zejxskso.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mnwxunuw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vikpbidh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdghimzh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2dvqyyqiy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2yaandflu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ofijeikn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jkqxuiws.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyptqvna.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2llxxarlk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2hxbwctbh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zjrxsabl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ipuytvbz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xgxllhhm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnezdzf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bwkxgmrv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2turqkkfr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xkfmjhim.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ycdczlga.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2chtwikqr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qmgdycyj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fhrgkgig.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2wtqmwxjj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2glbnjrix.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bwajndkd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuycptgf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nacqiygh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2dhghakhw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2uifltubr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuumgdha.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iaoybxrd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2etxgxgeq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nknayntg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2akqpynfr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mfxwzkoi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kcvrdurf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zlhjlxew.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2arktqpfl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dpiuaggq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mpapyeyq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vgxijfeb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2agizlfvr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2mxecdwcd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jlymconm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qlspdjva.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yywmgdss.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zneqxfdo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bzsalneq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ypfvprvj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mxieqjoj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jzjxqivi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ldhsyjec.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pmckhumu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wmsievqq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tidbobuk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2cjwazfbw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2oqsqlseu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2niolthof.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kogpvzrt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xgydnuev.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2utgdtlsl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gjmddalx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezyhcooy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rphqpdaz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wunitpgu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sdpkzvwa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ilvdhmld.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fwgboime.html


<!-- 参考信息 -->