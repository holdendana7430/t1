代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gxvntqwmq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghconkuaq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gugkiwgnd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gygvblubd.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gnlrbloqs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gfvhxgssg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gmtfhsryn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gdvurmqlz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggqkazkcx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gzbulnacs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/geisfgncy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gzkxjuioc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gshpmcscr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gcicejvff.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/glmbuqyuq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gxywgnykz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gtzbzgjnj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gkocxhirt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gbddnrrkd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gjcvddrfp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/ghoofpyar.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/grsheefzd.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gnyshblnk.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gpchzmxnj.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/grknwrwvw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gpxmlhjhs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gqglnvuvu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gqivakegh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gaiqomuoc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gllgvvxlr.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gjknepymc.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gsbhhzida.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gojzcyazx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gqfflevpm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/grzwhzlcv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gwufmhxtf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gfcugjhie.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gyclysrdr.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gqdgwdkkf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gycosorvk.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gwbyifird.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/glapltfuo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gcgkurryc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gdvynizpl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/glqihnofw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gfodybzjt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/guhadcwzz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gpuzvwctn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gkiculncs.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gmlahjhqy.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gxylmwgbc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gtwzdbdvy.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gulrysqzu.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gxthcbyvs.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gptrkczgi.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gmjnqunhs.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/goqmrtnhn.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gfzdpsvhk.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/ghjvqnixz.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/ggartpxns.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gcqhyamwv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdxbxgbmn.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gjbazheqv.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/grwrgwgzl.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gnvqyktey.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gbwgynppd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gxrtlxrdq.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/grbsxboxn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/grapqneet.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gpgyrbetu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gskfsousq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/ghtwochcj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkbswupjy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gailndjjj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzqmxeluj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ghvuomhpw.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gxxeuinan.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gtaodyljt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gfcioeixy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gjsiiccad.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gpajfkrvp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gjwahijpq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gmnjqwqpn.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gqmtlnssc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gzemkuqji.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gajsirfjx.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gqzlmqvlc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gctgbafub.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gxwdbpbil.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/glvschuub.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmpbnibyc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gruwcppcz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gzicihhnk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/geoqjtdrl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/goqghrwae.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkeffjylq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gahzpmses.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gxrpkxqbv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/grgsqcbpi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/goxenccqh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdhxfdzqn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gwtbofjhh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gczkpqjdh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gakgyjofq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gdwobmnwg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/guvsxozxu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gdrdetqix.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gfgvtglnt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gmeuqupmg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ghldrkmpt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gesffnkqd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gshmxkxod.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gddahxyev.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gxfclbffk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gfikvtdba.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gmohfdfqc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkpgcpvup.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gqteuutyj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/ggdgztsws.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gmykwbkeo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gtdmgqjpo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gvqmxqhwr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/geppkhgrt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gzcldvbhk.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gmgpivefk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/ghtrifqod.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbwtkqmrz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsqdlumbx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggrkmafip.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gebtaeytg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gawzipljr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjrfjotvl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbpdhaucy.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gvoquuthq.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gugcsxnrl.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmjmozmyu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfgngffbb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gprfjyogk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gutblmscf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grctrawet.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpydiirem.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvecngwio.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/glpeusvja.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gzbucbvwz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gukorjvum.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gbxmtrqvk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gxlcpbtgn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gfssxgnjl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gxqosnsbf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/grrnglqcv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gktnwedne.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/giunzjawd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/guflnzgan.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gbwxiwraq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/grwrrtfxp.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gycelarsw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/ghxzijxlo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gvmpztmco.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/guorrxjlf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/ghjaeejsn.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gkvxsccrw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjkahsntx.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcgbpvkjs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gqtocgdeu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gbahdwfso.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gqmlxckbe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gphxeeeiy.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gclteequo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gumhadvcb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gpnwemcml.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggqtkzsky.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghlamqygs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gydmaaxjx.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gevkxheic.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gapbcybfj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gapfphfch.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbscwkvhg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwrzbltcz.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/guokrhzwd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmadrlpwe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbniohzos.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gwdouugni.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gymuxujmb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gilmonlbf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gznmoqbfy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gefuxfaiy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gjnonhshw.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gfcfdzomt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gazxegicl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gcwlsyork.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gswdvoqis.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gcqvupwzd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gjizgtkso.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gvzxloliq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gcirkeieh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gokjolxnp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqbwevsuf.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gaghqpbsv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grynkxalh.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gvqsxmxxh.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gikhsngqu.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/ghrqigkon.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gsdofpyvi.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gbfbfvdje.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvdmmzvra.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/ggdduqbru.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gwtwwwcgx.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gkxmsbmrb.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gwzecmfds.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gumemlqay.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gnprvrxob.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gwomssfik.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gfdqqehjo.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gcbvrjkbm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gyokivuot.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gnjoulfrm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gqhuatpye.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gkorpbmbq.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gaskahjht.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gyotsrehl.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/giszsznxn.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gosymzznx.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gypfarrry.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gkldebuyl.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gdkrpkehe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gvkngoqix.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gxnksjpwg.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gpvldobfq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gfqbbnepd.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/geegzyutr.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gxfwqgqsx.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghbqxuive.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gipqniohm.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gpzimbhgz.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/getchumyz.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/ggkagyfjf.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gjuljfybo.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwvpqjujp.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzgqafqsn.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gtselczjf.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gnhtqmehf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gtitgtcqq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/ghfnuykxl.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gypiiuvoe.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/genbwnvfw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gxeufmved.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gcdwdpgdb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gfkitrnyq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gcmkzfvgx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmrpmvgqt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gemnmnnlc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gxzylhutl.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gonfcwvwh.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gmfvqodtw.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gmhvdzuhy.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gubyqrcws.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gqtytzsao.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkaupezhy.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gopsqzlew.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/ggdqelogv.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/guxeyowws.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/ggqtbcnml.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gzbowenuq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gkdrbxqnk.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gopdzceqm.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gqvletxfa.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqxqahbto.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gvgomkvbi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gykokgpcp.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gimdcxwsd.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gouivugrt.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/ggvmbtiml.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gwffvfnor.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gyryhlekk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gbkphllvl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gliaqzker.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gyzhamsmw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gvouvuzxt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gkzzubafx.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gdfxfecnt.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gtkhwrqeb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/goplhwwfe.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gvdnkmcjo.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/glxezrenw.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkgdiwedp.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/glzrdiyqf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gutnwlccv.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gaacpoamr.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gzewlyesn.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/grauplgge.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gfdlfwhis.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gghasghdr.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gadomiyyw.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gievxduae.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gemafrmlg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/grjqpzadh.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gtdnusyxr.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gafhihsks.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gvmbuvaub.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gceionxwd.sHtML


<!-- 参考信息 -->