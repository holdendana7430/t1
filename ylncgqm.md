代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gmcvjgelp.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gmxlvsmkg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gjjpjsxbs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gzuuwwulp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/geiaijhhc.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gymybdntm.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gnmwlckps.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gjijlzjnm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gkqsuhyed.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gpfxvlwkk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvnvtsvak.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gqcjxiinl.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/guprlckmt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/ghddzsjvj.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/ggtfcqwyw.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gvtxczvue.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/ggblndvnq.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gevmuuwol.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gmqnxmqpd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gmgopkgkt.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gebpcosgw.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/goehorspu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/grmowrskd.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gslzvouvx.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/glbtctnoo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gcjbtihmc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gcscuhwrv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gorzjrpth.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gtiwqpmld.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/givuajatp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gtodtyckr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gsdlshsxm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gqyevpffv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/ggsfveeds.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfturyuly.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gxgekzsmc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gulrhipkr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gvagjhscg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gqatoarko.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/guiougrlw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gahjhmpwe.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gzdgfccvk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gqepzpytk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gpztbjask.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gkdkcvuuu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gmcdfrbsy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/guphcddxn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/goghrtjpi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glbajfnpc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/godvbbhcq.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gkydzkulp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gdqogcsvh.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gcgoalpwv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gvftkvdfr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gnjhydtwq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gbnoctmic.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/ghytcnpup.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gmqrprrhh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gomzuzvde.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/ghwudxyod.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gujfwnhub.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gbschpeus.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/ganhjyajj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gdqhtyqky.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/ggvwkbisa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gbgrhjyhd.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gihieeoer.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gkkbzjyfn.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gnovuuwym.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gvpbwlpkp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gzhaqtbnz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gesdmplnn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gxyhluezz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gnsbpuicn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/ginsicmfg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gngxjywyj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gmvzxxxqq.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gbxcijgnb.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gwyiepyzd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gadgvjxvh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvypylhld.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gsjixwkpm.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gihvatwwh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gluwhsvpt.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gsthrkmpy.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/guqjhnxxa.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/ggybxftpf.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gxebvzlvp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gfseuufhq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/grnqvwccr.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/glkdpplof.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdquhpsrx.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gafpooldn.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/goxlselow.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gcqvkdmbx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gblsewbid.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gplgdbsam.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gykmxsrli.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gnrhtcgcu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdyzgobjv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/goajfsqwn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gfqwjhtnq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gajillkhw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gtloarhdw.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gvqvmqajq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/glrxkxlgy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/grrsfzddk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gpaffhmno.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gwczvagpa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gkkttiwlm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gwiadhxhe.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gyhpolimp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gvpgatzna.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaokgbiep.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gxljwmhlk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqyukirpb.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/ggooieanl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gdafnlqpc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdrgnvezh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gvslnihqq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gqeeysyjy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/guxbxsxaa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gusmmmzev.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gctndqfnl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gomvyrcox.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gdraizkpg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/guvbwhwpo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gqtptiwno.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gjueejycx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gnrecrotc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/giwaxwcok.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/ggsocvnhu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gwbvbatdr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/goddhukbb.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gtudncigb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gxcnmgbls.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gdtseefqj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/giewqrwjk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gxyjlguxi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gmeiraftz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gndjvogee.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gczdiqnzy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gkukcxfok.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/glcmnowjg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/guuwjezxr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gsyxafzvl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gdqesaezw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/grgdhpssr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gsoctohxz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/glkthwdjd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gqjqngeyy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/ggbgwhowu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gqofbjxkj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gsfqqtstj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggpitakiy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gapwhmhyp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsxpxgfwa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gkoxumwap.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gkemzujvd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtopdjqqa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsdocbfod.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gsraesrcq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbfbuqhht.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtllarmwn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjhjjqvmb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggkvukodv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gwzihhzzf.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grpuxvugy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjhuwqfgy.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjujrxpfo.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/geypfzlkh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gtbqnpvrh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gnjzqqvwo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gmtwxpacb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gmvmwdoxv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gzaiylfwo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gksistqop.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gkkbbnrxt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gadqrqypq.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gcttjjkaz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/ggsgtaayo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gvdszbumy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjvpywqne.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ghxjohkmn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gndfxdstw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gkqyazzjn.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gwjmmcopf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gdohmtbfw.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gtefnxsqa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyvoumvll.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvyadozok.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gidfhpzvc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gztjqofir.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gniscwojx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/garppvnds.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcyaxqeap.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gbmawknjx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gtwywzqxq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gzddbdxce.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsavexvgu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gresppkpm.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghwiozphd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/glujwrcwo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtnbhngrv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gytzyuynk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gubivswhn.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gxbogwgoa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gvjhawmzk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfsnadzfs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gqqwabmpa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gcjcourdk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gkiefmfbj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gzuxujead.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxuvulfyi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gmjymvucp.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gjkuubxmr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gzgkmcfbp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gzjcqsxxh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gwcgqtucg.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gdbqlzgix.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gyhclbkvp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gjlznvoqw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gutzwazux.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gyoxeckwo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guidevwha.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gnbawxjql.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxckcbaih.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gfvnrqpch.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gknfoxpbm.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gxsfkrnuo.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/ggwdifsaa.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gtqtddulb.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gpunsyxbs.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gvroazjns.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gufpiucwx.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gwmisevpj.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gufubgrge.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gargitutc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxuwjqver.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gjllvkqmv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gqhomsxjj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gmavwlsrt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gllqsejrb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/ggxvhmghu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gbxdrktxj.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gmhwcqprz.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/goyctnggd.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gbeemoqsz.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/geaunklei.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gzcvbddcy.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gfyzdxaji.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gwietvaii.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gvhvzocnc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gvmtzxabg.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/grduntrgl.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gkdvjbfea.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/guzxojhlx.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ghwaopfhc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gqebssgzw.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gxkxirlli.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/guzfxfeew.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gbgdigpdz.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gtigdjlms.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gquyoxlyb.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gqburiust.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gvvchgecw.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtzncollu.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gooefqcia.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/glgsgercd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gsvwdlzpa.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/genhksokj.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gknurdxbn.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/ghdtzbumr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/giwhinlvd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkcmdcvgp.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gerzrrbwp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gjuompvhu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gwgodwple.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gatntrqwb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gaokuwfpw.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gcxtdanfp.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gzatssbgu.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gsvvitsbc.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gyblyjxbd.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gaocwzctx.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gvctjyqyw.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gmejewvpx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gtpxrjyuv.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gnyurretn.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gooatsjsy.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gmdlfhbtm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gbbnjoham.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/getxwsooi.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxdmeljlc.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/glvjtnjej.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gjiibdsro.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/ghnzjozzv.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gnabcckax.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gwaedrllp.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/giptkiccb.sHtML


<!-- 参考信息 -->