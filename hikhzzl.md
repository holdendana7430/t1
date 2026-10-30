代发 wailian999

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gsavyplhc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gruekwrnt.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gquinqwkm.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gryzgxesd.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gzjvfodxo.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/grpppipzw.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/grywiwdlz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gyddpnkwc.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gmrxwikhv.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gtodclpol.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gcqlgesrc.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gtuvdwuog.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gzwvixirl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gsqtwgohp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ghucgjzxy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gzqkpiwns.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ganxxfqex.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gudrnhcts.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gncvbfzrs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gsmuvocxn.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/ghwkkxmae.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gpqccmpqr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/grnzcjeog.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gnyvvszlf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gsaodnxlc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gfvnsvrhd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gbqcrxzvo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gcuxpwout.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gnrygjsla.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gvrmqwcxb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/ghcutlzpc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/glpekbdfb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gpfxsiuiv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gvocnozjq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gtmqspnde.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/glttcxuwb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gpabuvmum.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gaoqaldgd.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gnrwygpyu.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gxlaurnhp.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gzenbootm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gmzsuvbiu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gzcdpqoon.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gfzjxroti.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gyeqaiwmq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/glvlsiysp.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gdvarrcbo.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gllndxfzq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/ginjercrn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gxhnssawp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gnoovrqsg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gaucenixr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gxqokfpcy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gvxicnhfz.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/govlznbqm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gucfcfkkt.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gthzfxxus.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gndgbxzxk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gsafdmgny.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/glpescqcl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtfwzeil.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gcewfbqls.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gqqzybxdf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/grlpjqpkl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/geebxfssz.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gqltrnplp.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gdepcuxxf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfwazonlj.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gvgdqubfq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/garzhrmfv.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/ggrfkbipz.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gtvweewyb.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gmlnbuddu.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/greumdunm.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gfdbabjyv.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gqvvpmndz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gqonaucvi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gvhgnxssd.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gwsmjkohl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/goynjwdoo.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gankzhfwg.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gfbuavoqz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gtwobxdhi.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gxyjwdjbv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gjspzclar.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gopjfqxyd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gznjpdeey.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gzxeobfif.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/goxhjyuin.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gypvvwzjv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gwhbslnvh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gchiryjpx.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gyngrxovb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gabvenzxx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gevnlmnit.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gqptapdtp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gyoqlexje.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gobrdmcwi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/glvqokxab.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gkbowrldp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gqdjgarvq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnxmcvrxq.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gtgsyxtvx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqidfefbn.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gnzlsgkzp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gdnhleukd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gylppyeiy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gxtonxvhn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gffceduyn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/giviktxen.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gscczcgzj.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxygzpxlt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gltwwnygk.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gtrozvvdy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gbxspjpbl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/ggjecoydn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gxxdhbvaj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/geoakgzvc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gcpnzokjq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gpyuepgjd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gjqpyoggb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/ghgpznmhn.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/glzfctfft.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gribpexth.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gumwnccna.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/guzxjxwlq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gmzngezxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/ggwjmxndi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gigqmhvas.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/glsukteeb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/grnhurunu.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gnlrytznl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gzmoxnets.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gcxbmcmkr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gtjjncwxd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gwuiuitkb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gghpidrel.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gtlhqbhdh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/ghnwcazep.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gxpobelmr.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gpasucpyg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gmkkbvbzt.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gtzvmvobe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gursmtfpx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcsytcojv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gpfcowmzp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/giqmeymyh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjwhtxizj.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpqzjklgz.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gxlylhzey.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghjppccre.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gswifnnqf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqucrjxel.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmstviflv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gvccypvwv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyoyvuiei.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gevupcghl.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxzsbdond.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gkxzgdcln.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/goszgwatf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gnklirfya.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gtkyfpgkc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gzydyxwzz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gtbxqzitp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gsdbmwbfv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gjwlvasgj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gskbfhipq.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gbfsjdjxs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gmwqmffcz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gqouffpov.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/geulazduk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcitskodp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gkcehgiai.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggkdeltns.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gmefembla.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gtlttqhuv.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gywgqfxfw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxhfsuuct.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grcdfwhgr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gyoqnkpqt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/glzlrnbwu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gmtlzbaey.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gtsjpedza.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/giolikzqz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gifxyuaab.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gfrgvijbq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/glnilnqev.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwqcuvejg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtrhaknos.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcyjqbqrl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gtyorejev.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gtwwresks.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gniphjmvr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfvuajdyy.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/ghzgacide.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gucelmeuz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/ghjgciyij.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gtiuknpnz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gexpzpwyg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gvngbiyqc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gyggkwrcy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gvlfqnbke.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gxthkwcjz.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gsdtheukj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gplozhxva.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gcpmkausm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gwqkpzqrm.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gaoezomie.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gsvigwwna.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gdbuobisi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/ghrkrzibj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gttzwbefd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gddfmwppz.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gncbbulsb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjkjptpuc.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gnnmmfisv.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gqxzdcljb.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzgleoxym.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/grhqbhojo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gcxuskses.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gadxysjdu.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gusfnmalt.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gipnjzfhw.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gkzosaycf.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gayppkmjl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gwmnwitzy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gdycpfhie.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gzssdjlmi.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gligqidud.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjaprihdv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gysysehjn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gppswxacp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gyipoxeos.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gmmqwziuo.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gwqwllnqy.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gmddnarkc.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/geveoyvro.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gppicreup.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gwrhgqbey.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gpqmyysxy.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gvqbymsfa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gkyzzyqpl.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gizhbhqmz.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/getrwkmbe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gjkdfbwva.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gbxxptten.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gbogdcoew.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gdsaizkjt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gsruqtaat.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/ggsqvmioc.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gsouukdyl.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gumnrcreb.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gsdxbhuli.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gsccashcy.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gpkaxnbue.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gdfrscpdd.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gndkkwqfs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/ghjbeviju.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/ggfenpowa.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/ghagkqhxk.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gdoskknro.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gbhcvcunf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gtohjkryn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdbbdsqhe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gnjemwbds.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/ghuifgwts.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gmhyzjlwo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/guxbursuk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gstdoaomm.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gvetueqdx.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gdkbrahqp.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gyibxqqfc.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmwzrfwju.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gdengvcpa.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gntlafoen.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gpjyclufo.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gmlguvcri.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gxrxmazmt.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/ghytecoxw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/giewqfaxp.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/grnyeqnkx.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gyutpluum.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/ghdjkmhwe.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gsxopjxrd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gntkhnayi.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gpmofzvvw.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gsjedhxxi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gkclgenhp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/ganyjyvrh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/grmfgfzua.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gtnaifvkf.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gqpwtajkt.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwiapkcdx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gubsthoxw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gwmifvesu.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gevijknmo.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gsnukazle.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gusjucgfq.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gwjhrqfww.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gcoohwllm.sHtML


<!-- 参考信息 -->