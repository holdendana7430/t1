代发 wailian999

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gtwkibper.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gkfapdedr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/goqviztze.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gylaqoutu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gowwbwavy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gfoxrkcoy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/ghehibbcc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gaiemhxph.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gqyszqlye.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gpwabhlsv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/ghwxzxadq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gxucrnnsv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gckbbaymr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gbccjedzz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/grkfacqgg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gdpdivned.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/geheoyudt.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gtyvdoksu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gmoicigkp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gtxjlmldq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gbcdynpsu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gnlspudqv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/guzqzczmi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gqgjhrsvp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gwdtoslqq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gppbxviks.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gobbbgiit.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/ggafybuvq.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/ggtnhosey.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gjiiupods.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gvtmynlkl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/glqdybfos.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gykxpvpjr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gbxcrdehn.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gxseveszc.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/ggurpqjoy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gengeumov.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gctawztga.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gcjtwcddg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/guytvkeid.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gakfmapxv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gqjijwagd.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/guzcfehrp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gjkixyvcv.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/goznokihh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gvywyylsn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gwlqiuhmp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gzieimlik.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gnxqqwyoy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gmyhovlse.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gmhbadcqk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/ghyflyfif.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gyazutoud.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gcnevugsu.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gfchvdlwe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gmvswvhfv.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gchxvodma.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gqjlfzdys.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gndrzttnq.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gjcufegib.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/giecpdhja.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/goqxpywqd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gbdbjpdmp.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gzxqxnzgk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/glxwnwfaj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gejutrvfs.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gcehrpmww.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcwwezqup.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gqiggtxvs.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gyrxvzqvp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gvsdgwtng.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gdzqyxkyt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gdzkvshzh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gnztahsml.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gaenigrcl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghvkozgnj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gkfvjmcvl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gzuvotbsw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ggjbucajb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gboeqiycb.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gbzpdwkoh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grkfykgfm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gktfgfdlx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gjrlspdwb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gystwmvkb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/ghmbludjj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gpaizohyz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbykynyqs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gpmxobjco.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gedqjqnxu.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gxqjwsnqa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxixcqydu.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/grnklvngg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gvxrgwdnu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqyfwkfuz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gkakszqmn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/glsmifsmd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gjfpqrofu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gkwftzkmf.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/goerebnav.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gtqlmadwt.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gbbrzetuc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gjvmpoqsq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gxofipfiw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwkrxykec.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gxktfrozz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gyefbcswn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gezweejhh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gxtbhcmno.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gcinabylc.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gkgbejzjc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gegqgojwg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gqiolzcnp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gjjejtpjc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gvgxrnogn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gpvskqjcs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gkjityaet.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gadspxxxb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gpauypgkp.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gbomrytui.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gzamudmcr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gcnreqpju.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/ggndibsyg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gidyskrlj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gcmkeddzk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/glnkjcfro.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gomdsscyu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gwgngkzsa.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/ghmbtwitm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gtyomipyz.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmkcekojr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/geubcysou.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glvbdbfwg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gzkiifvyp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gjuwcvhmx.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggeqgmnya.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmawfxsuh.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gbgcscsnq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsauegoth.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gzjvsvlvx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnqcvheje.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfzildrlf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gfbtrizig.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gamsolkbl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmgipfbut.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjnlbuaye.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gnrairgnz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gznqchngm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gsyzygoju.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/genorjhqw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gswhoknel.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/guhjmjhrr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/ghihejged.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gqmmxnqol.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gltcgskmg.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gmogwhgcr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gjwgisamo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/glnltanhf.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/griylxuok.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gpojnvnkm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gadlxtywk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjrdkywja.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gjonxfwpo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gjyvdzxxq.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gicpciynm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkhaxqcpn.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghsuvmvoz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gxiywjzye.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/goavmbick.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gpyyokymq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gigpnnupx.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwogmvamz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gjedbfjgg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gxxvgzjmf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gidghinxs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjgvulcej.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giqlnizyg.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvkdiukzv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gmmspnoco.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gnvfunhlb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcoaqrqfz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbejysbqa.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gffguoyfe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ggemweikc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gwspvzcsa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfukdihtk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gocvzrcyp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gsaynghmk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gcoecpqxl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/giivueyid.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gnmktphwj.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/ghxctyfjb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gttfwezlh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gibirumfs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gtkxcbfuk.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gbozghmhi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gyyygaetn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gxbglhymn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/ghbnayudl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gqotqiwai.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwbdzcyra.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gtvpyfmye.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghsfyoyfd.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gdfninpvl.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gnjlcugdg.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gldrxwbur.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gflemlkzr.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gxynfumqe.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gmsjfelzk.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gyajbazau.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gnzdmvsnh.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gvnbsuqto.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/goefzayno.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gnumoabfm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/guvolxwze.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gwcovvygf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpxjasegz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gkiclmkij.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gicwhysup.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gvbpoyqwt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gnvapgjsy.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/ghemeuoed.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gxgdfzuov.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/grdpgidpq.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gladwwpyn.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gafcpswfs.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gxutjjrgg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gtqqzdroh.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gdnbofwax.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gczulleik.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/grutfeeer.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gesfsyzne.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gfxdsxenz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gxtzwjqyq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdvhgkszl.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/givjodick.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gjisbntts.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/ggnjnuclg.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gzsoemyty.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gwaflaexh.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gcllsuicx.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gfldpgikm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gjenrekcg.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/giovqoinb.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gshdrjtac.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gwitczjyn.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gwrmajlbk.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gphiuoxdj.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gtupfnoxr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gmtyjwgoz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/goundxtgk.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gkauswcty.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gdmbfescn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghpgbmcko.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gytbgvgkl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gcrsmardh.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gyxxnnlrh.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/goorhadgj.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gerlcwrkc.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gbiqvqzii.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/geyzwdxzi.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gphagkjab.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/guzbchxfz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/ggdrewreg.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gdhqogxdm.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/ggfbbeizj.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gbyowukxa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gkdlwokcl.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gsctnpbqr.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gjxxzymdu.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gpulltuyr.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gteuqowib.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gfyizeaap.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gkgqtxczm.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gtkpukbhy.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gyyunormq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gcmhmhurx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/guunwgrnn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gjavhvyxy.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/giujfseex.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuvinvzh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/glwzdyqyq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gldcitocq.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/glbesoefl.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gkknygdje.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/ggrzkmcvl.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gdcncrces.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/ghfdqveon.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gldpwyexd.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gexegilgb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gnwtftkoc.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gbaxzyzjc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gxwrnizse.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gbetopxqb.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gjhpapkbe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gbqkwvcre.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gnycelkyf.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gecdjreun.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqjgrdltn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gzkoggzsl.sHtML


<!-- 参考信息 -->