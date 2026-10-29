代发 wailian999

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gbbnmslge.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gwddvadyv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gbpxxeqlr.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gbdvhwjzz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gtaeslwkp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gqlzcavdd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/godnxpsja.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gurqtgwkc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gfkynfgso.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gmdttwpbh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/grhsjvmhc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gtsbhhyhj.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gdrcopqvz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/ghaygcmxk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gstpwcrhd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gryxvjkhq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gcdeewghe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/goqdepntr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gzsjhkfcu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gbkcugozs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gljqojirh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gqfbqyrkn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gblxlapkn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/growwyjni.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gmquslwxg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/guqgnvywj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gozwhdnpi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gjbmaclfv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gkrvbwqxx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/govlgnujg.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gxhqnpyeb.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/ggxljxqks.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gdilocwgi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gmjjxrhcg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gxoltbcac.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/ggfgcuiva.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/giczjhxvc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gipffwiph.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gvgczltcv.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/grsblyvgs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gicwajmhu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gtmhwsjoz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gjabzvvnz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqdtstjwp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gksubilcj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gxtobcprp.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gypqajuat.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gxxppbwga.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gpvjbjphb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gbhsfhbvy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gdhuaqbox.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gxgofafvc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gfnvsfqvv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/ginuwgyis.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/geucjdxjq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/ghdgimclg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gjxdgkiwa.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/glwpcskvq.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gbrvesrjw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gqzdkdhbd.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gccvdrbrx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gewthmmhh.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/geqloashw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/ggdopksqs.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gtrmbeolu.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/ghkhsshba.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gtwqkbgby.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gdgzkpspd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gqumvbbse.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gepylfcvk.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/ghsctcofc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gwcbpuoyd.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/guttvdvna.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/ghyhoynkn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/goupkakmu.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gitoujqne.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gppcydvem.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/guagpukdi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/grfbxdesl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gxrehhyio.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gbfmrgnor.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gcrhdgbgr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/grlbgnkvl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gcijxbjug.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gnlkjtdbm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gwkkzbpvm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/glvpzklkh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gppjyekej.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gvzzfzkao.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/ggbszuycm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/ginlcnmsh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gqoekkoog.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gzfhxtnww.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gratefnis.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gnporrivs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glxrekeqr.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gdyoewkxu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/govwderjy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gkkfipdyo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gflzpcrfa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gsrjmepjk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gqbadsmlm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gddbowzjd.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfjmojhuw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gshlxpbok.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gjroutosr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gdcmcwzil.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gynkregjs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gdmcputpi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gekhaxzbb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gdserqxpd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gchqcvjdx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/grmicbuly.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gzrfevefi.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/ggninldrc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gulzhgsdr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/goofykqre.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gyeqjines.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gzjdbwbrt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/ggujshaaa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gvdatmwna.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/ginonricv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gfrbfzrpd.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzoanokol.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/goxwkbobw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gqvoaddsf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gjoltzikl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gwihutyfe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gojpjdwjx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gjlutljju.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gopzygudc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gwotxywuj.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gqjbdolnk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gamxqxqhg.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gksufspyb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geqnnvzhf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtmwgewcx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gpppeyyfz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gdmgwchhs.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/goahllesl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxlikqjwx.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/guzlrxbtt.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxyuvjprt.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwmdnhlln.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsihevdki.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghkvfwahz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gxpkpapta.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gahtijuid.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsqhzgexa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdyigwkjb.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gvftxzlve.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gpyrgldcx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gsfmwespa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gkcifwgvq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gdrofmtvx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/ggsmopoui.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gooqroyex.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/golnugxwg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/ghxjafjwn.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/ggewjtjgm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gexytzvci.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gkdrkttwa.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gdsszlqkc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggpabcdxf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gymviuntb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gpjvypafi.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gzvpgypog.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwonrssba.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gmnndyowu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glbhgpzbz.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/glojuytmf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gntprqqye.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gjyhtegue.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnyokedwp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gkqleizdi.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghnlypifw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gjzatzcnt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gucquwnwv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/geecrxaxe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gycthxffk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmtztgqne.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkmbncbch.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gsdsfebbv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grrrtkiwo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtzljhvix.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqxqrgjre.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gduqgzqcv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gpzgjrdbm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/goinphpeu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gqivgerqa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/goaupktzb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gigcmlyfu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gxoyovxtr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/giwyflusu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gbzhjxmym.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gtzvzsxyg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gdtztogwl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gksvkfsmf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gwwpqaqiq.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gusqsxnkv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gkovqchuk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gcrcengku.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gqqoyzggt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gyrwyuzuw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gublxkxte.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gqyefokdb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtfhismyk.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gnaespsta.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gklkqmjen.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gxbcfmdlu.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gsasudfow.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gxualtgqt.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gfwrlkqkg.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gqlynlvyb.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/givgawybh.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/glrgkueci.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gpyoywnye.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/guwtohznn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gtnmrzkym.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gkphjnfku.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqttadbdv.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gtdlgnaeu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/glakccmsu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gkochpapk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gauwlfwjt.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gkzrmxzih.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gdgfiezhv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gxxqfoglt.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gcnjhltig.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/ghpizunkw.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gwjvbjggu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/ghdttvzbt.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gyheeahmn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gihjzknmx.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gbsrlahpm.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/geqawyrzk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gkoerwlzs.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gtsecbwnv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gaqdoykgt.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjnograki.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gbycglrtg.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gobztpohi.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gcvagvrfm.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gqdfzlclb.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gvfiveucl.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gnctrfbqu.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gfneioulx.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gyotrysie.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gpeohwmwu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gqfpmhkge.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gfzpkszvy.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gweayrjpo.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gmynvctos.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gouwuxgck.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gvfnyxmkd.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gaatzymni.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gcrtkavbw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gkhbgenel.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gbuhqntad.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/geajynlub.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/guzvwhwxg.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gicwcbcsz.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gzndbclsl.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gexbhffuz.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gdyzjlsmx.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/goifwnkmm.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gebuobckg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gdownwzin.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gwapehelc.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gaydgqfua.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gqtzcggvf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gopuwzwms.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/glicbcqat.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gsjmqebdj.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gwanlpgmb.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gkgfzprvb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gvhxkfylv.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gzszbntcw.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gpmyzwcav.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gtsjhyjzd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/guiahmjye.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gjhqcpjns.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/ghkvbkphp.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gooeaslsr.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/giqvfdhze.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gvtnzelcu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gjefenakd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gqpetwnsp.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gwrgpqeyc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gbumivigg.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gnxqhhqdf.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/glrwdjqfi.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gqdkfxyrl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gldjcshll.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gmdsxtwax.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/grttgukmh.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gtxdogzny.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gsghcvhmi.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gvobxngpj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gyknzyvln.sHtML


<!-- 参考信息 -->