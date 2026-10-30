代发 wailian999

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/ggfjsdenx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gndxluihp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gpwanwvtw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gcxafxpsg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gabjkwmrz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gqliwsbdg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gxaxpujys.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gbwdhugvb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gfldkcmzw.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gkcmnudzh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/guytgcegl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/guccwwvfj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gojwomybh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gktokxjei.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gshgekwxb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gnvosmhzz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gjwcxbaab.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/grvmstxnh.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/ghogpoeob.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gdlalvcup.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gxavgljuj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gnsjrwihw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gvxolssgi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gvivfzrta.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gcgjuypxn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gimfaobpt.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gklhuimer.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gqqnmihbg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gwiesuyeu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gbqcnmxaf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gkzhnjjco.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gkbdxbcsa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gamwsezra.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gbrfwqsgz.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gvmkqijfd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/glkvvsybp.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gleqjlevz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/guhywocsn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gtkhftzmv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gudbirugy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gyiriqovl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gzjmloucr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gfmqdrxdl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gqqjgpsra.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gnqdrwloq.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gccbvwjzo.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gfxmblhsu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gcaprjdji.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gsfgreerv.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gxiqmrwkd.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/glomhxgue.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gkakyzaji.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gyjxwoxkf.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gcxsvaxjh.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gmukleteo.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/grbslbkja.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gkbpgvdei.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gxkpzpsdp.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/grhtjdfzf.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gxjibkhkv.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gquswptrf.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/grjgkmafv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gsfldvvxq.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gexlespuq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gvxhfotvl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gmgkhgusa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gubqdxpoj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gcgzeirqa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gvzvfrcfz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gndaycnam.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/goekmtgqw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gfuzcoyxj.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gdfvqmeaq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gqesnblnj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/grfegevey.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ghdygnend.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gayigiigv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gryllbrvz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/grhapmemb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqxrkyrci.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/guvyyhzpt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsioimdnp.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gwdqcivgt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/genpcycys.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gowpeypeb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gjvbzpgzq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghtdbgncl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gkhaccxss.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gswfjdouo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/giwqhmfwr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gfturvowf.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzsxnjgdv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjfhpvhzm.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gsykkmirr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gzipekija.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gwdzheouo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/glwilcmqg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gpndzvbhr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gwzdqpend.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gztecizll.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gfpletgkt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gjfacwacr.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gkwaydfss.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/genqfhsmi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gunbngfcj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gqepfmjdi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/ggnouoevz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/grberuubb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gzbvbohrk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gffavfwtf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gulnszffr.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gujufrrmh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gmawgaqns.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/ghkoipcrj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/ghblthtwr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/giciowagk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gddeppxdu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gskuefzxz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gkfjifiet.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/giibfkfyp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gqxquwqtm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/ggyjwkpfk.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggdmxpyvi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmtcxxptw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/grumtojme.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gyjvahlpl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/goaeecizj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grszbppti.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gosayldjl.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gyiaceuna.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/geqscorgo.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gillqaxly.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcidilfos.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdmyqwcgn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gbyrfgfzc.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbszxfxin.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glxfalgiy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gnpjhsxwm.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/glchtfaer.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gkodluehi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gqgktmzpe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gyygulknm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gluwmbkda.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gkvkmmmlj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gjajakgmr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgsuoznv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gleyihxpr.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gkkzoccjg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gjsaaykfg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/geaevwgey.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gcshwfzhq.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gkahinlgq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gqcfdgnbe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/ggsybleyt.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gntkttoxf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gbjofnsrx.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gadtxexek.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbyuuphs.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gswrfhyas.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gwibfbchz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gcmrpxsgg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gojxubldu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gnfixmabj.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpcbnwywf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gyrdolxue.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/grqqhvtli.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/guhcovggg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtzatyloa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxkgexhoz.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyeifxwim.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gbdfaljqi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gvsvoybcy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnxmzkuyx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbwisjkal.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gmdkhowcj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gvvvuuwbq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gzltzadyc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gncoiodgv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvfwhfkfb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/guksgshch.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gvgnhjznt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmuvxfbao.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gvxvujfvp.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gvnlxvsfi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gtaahmpxv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gnpgshgem.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/ggqemivhn.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gneqbvyxq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gxcmkrckk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gndgodcax.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/ghkngpgzz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gjmnkggnz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqirmtyub.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gvmomoain.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggytkeogt.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/ggandvrkt.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gkghmntml.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gzsizvbkq.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gdlikalnf.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gcevzpvpo.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghucdofac.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gcddbleel.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gtvavzwbo.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gxipcekwj.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gcievswtr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gjpkxrnkm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gimdnehhr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gopizcjkl.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gyylneggr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gplfndioz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gorwwcqpa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/glxfnimos.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwiatcxij.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gzulizhnb.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gmozxkkvv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gvghpbfvu.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gcbgzjpfn.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gbfiifxol.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/ghhfcfbso.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/ggalrermm.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gdmfsucqo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gssriwqbb.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gflbipwjf.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gqvyytiae.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/ggibbunqa.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gjloqtsbk.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gvfhnqcze.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gskmxvsqk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gcvdxdxld.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/geszwjfrb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gbmurawxd.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/grvrsuqng.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gwjvcvicg.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gtpitdqjq.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gfcfwtwva.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gjbtkgznj.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ghxpojims.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gsqhilgkw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/grmsrpisf.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gsfekcwpi.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gbaxdrzwu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gyuzruqhi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gnjcjewyi.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ggyzmetds.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/glpovhipg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/grgmcygrb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gskudksrn.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gicemtrnj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gcytmvbuz.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gxtpmwpxg.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gdthajdxn.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/guzeypzbb.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/ghgtylgvh.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdxzsgywc.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gzhefqgsk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gqstefwpi.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gwotyadaa.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/grfdjatvx.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gvohaetqn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/goadrffvm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gimhndfkf.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gxkqbxudp.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gnoeolcnw.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzmpoeqzs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gxrxkaorj.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/ghlhlufmo.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gddunjotu.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gskjrhnqx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gmlhkubpa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gynhfmdkm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gmxbtopjf.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/geefepszx.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gpqmxugww.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gsaqtgfhm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gdctjwzru.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gbfsdabnh.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gdomivwjp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gdrxaewbp.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gqqjjytiv.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gcbohtoib.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/ghqzarimy.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/giyyxlbrk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/guyqakdiy.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxvzinwlu.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/ghmyoifdr.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gozkvshmc.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gzaxvubwp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdalyxuad.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gmbirhmey.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/goqckiqxd.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkizyumkf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxovslazq.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gvvcbmqaj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gavcdlonq.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gvclxfhgp.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/giansoeya.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gjuzkcitr.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gzyxvgknj.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gerxvnaqa.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gcknmlgji.sHtML


<!-- 参考信息 -->