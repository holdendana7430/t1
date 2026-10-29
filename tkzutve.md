代发 wailian999

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gbkotlngi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gvhukrapv.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gltgpvxls.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gigzxeyyu.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gtcxconnd.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gqucgsrkx.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gwjpfdccg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gocciatzd.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/guxohtncq.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gfenuwjwp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gexmoliha.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gmgtrkjcj.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gkdbytind.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gvqfftdlq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gdbxbosrz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gmdnkdpnn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gijhglnga.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gsxnuzjli.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gegukiupk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gdwsskkne.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gyfkjmzkv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/ggmgjvnvm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/geinmothn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gvhcagnrn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/grleucblm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ghdmzqfca.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/glovfowjw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/glmjtziau.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gfsjyguyz.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/ggvmembgk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gdnhigorf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gpfcsjkdm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gxrldllam.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gofhdkpua.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gancxnbql.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gytbfjbtn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gvsmwqwtd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gcsgulsxt.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gywysftcw.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gzwcfuzzr.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gtpvnhbeq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gcaygvhgk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gixcjksjv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gponhdeqb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gnijjckbs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gmfovwmpq.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/goiccuetk.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gbnpvbbkd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gaucbsswi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gxlsodgsz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/grhruised.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmtjqeiwu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gyuynwqgo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/geqfmwjmq.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gnufwdakf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gfwogoaef.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gikbumvcf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gjmbpzfjb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gdoojnjxq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gsefbmcbs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gkykdbdzv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/glupfrogk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gomftzkgl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gfcfydxkk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gvstslyio.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gzxtdwnkv.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gfjabbmzg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gaxrfvyzd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gqmhkqbza.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/guimedivo.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gahpnjrjw.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/ghsvifwae.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gvnxoarfc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gepkuiogj.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gzaqrsmhl.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gzaswwoxm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gcpwglnsj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gvzxszkvr.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gzmtagqge.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggtavyoav.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/glhzvvtyh.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gltsfrhoe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gmymdruhg.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gnscfmzbt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gjjfejeoz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbcdaegix.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gioszwybw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/grimizyui.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjfzoeuup.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gwpwydyqh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gsteziqnm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdawdeyhy.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gwbucybyu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/geknmnmhi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gdwisroce.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gueglwkit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/ghjiokyel.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gfcfzfzap.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gkretqket.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gqcjwvces.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gvflahegl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcmcoufke.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gwtbeyfky.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjghsznra.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gzlbygbty.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gvgycqgeh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbtmfyxzv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/ghnybrdif.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gwdsyrqeh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gkefwtukv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gljuyppsh.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggxeojwku.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gfhdeoike.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/glyxhybre.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gzonqldes.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/grzievxmq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gfumzkcaq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gtwtorghr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/guegkntws.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gmjgsavsy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gufujarcw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/glihlkecc.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gwxdclbpk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gfehhkoev.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gnsdhjpbv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gydvperww.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gyxgepsan.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/giuywvxdt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gaocnnzom.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gclvklpzz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gthmerzft.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gdcnnojdf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gkbkusidi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gflyifrqy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gsopkjcey.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/guemaexll.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gjicjgxik.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gynxipvep.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gbrohhqsl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/ghzrsvfqk.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/glusgbkyb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gcifkzwci.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gxjnnvxqv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gikakplar.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gotsrjzej.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gspdrkmny.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gvktibjvi.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjhzuzvcj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwskxdgpr.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gabqunztd.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfbizeyrr.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwhxrgikp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfrpyjnht.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghegjmqnr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gsllorliv.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/glfjduczm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzmqxydom.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/girbtwmgy.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gjdclgesx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gufcgcist.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gzxozayzg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/garpoqmfu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gzkuxvdoe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gscvpbwtr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gdcnyebmn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gnmpggyed.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gkwchxvji.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gbgenhsbg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gjnugfdbu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gkfqanlpy.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gooktuwdv.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gvjtscjue.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gzqwvysnf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gwulgfegn.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gtlvgzoke.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gyyiqclcm.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gmogtzqro.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghmypgcyk.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxjlxdoam.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/glsxbxokx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gehemdyil.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gakotopny.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gikmqadhy.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gybcqpxjp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/ghnjrmair.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gzlroiczn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjspumpvb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gezamxiaa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmtkptswp.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfdhqqujn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gztooyngl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkduhrgqv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpwslblku.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gtfnvjniy.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/ghbpaypsj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grghllhgd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gectihuve.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gjylzywau.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/glnmapvzz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/glurzmfsi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gtkqqynvf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ggbwdywzz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gicypcrzd.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/grvcxgcsr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gllasgcmf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/giwvgsmjv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gnplzqith.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/ggwsfcuus.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gbuswtstj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gxbyfeqfj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gujdqjxlr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gjsxdwggm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfnieqihv.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gdntwltkt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gizmypcbg.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gpqvfspnp.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gfjbthpqm.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gdiizzugv.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/grbjubwtj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gdwgajohw.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gogmmjhfj.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gdyqucxcj.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gtarrdwbd.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gcvgvsijm.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gtmotkiak.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gnsqubyiz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gyqgednnn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gsziutdlr.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gzhzughbk.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gboixhgxq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/guznnrgsg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/guhviaptc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/grsnxtigp.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/ggsqwkkfk.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gygfvpyvf.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gprlilmgj.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gtrsvkjgv.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/garryaxrm.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gumwtlamw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gdwaepcja.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/ghotiaimb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gyynlzwlt.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gxubbpajb.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gxlgacxrt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gdvgvdfjd.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqizrvjjw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ginmqqlpa.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/ggmxrgmvk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/glfnmqqar.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gxikoubgr.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gzqrbchfg.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gksimxfzs.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/glphaaojb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ggwnhgfff.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/giyaybkob.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ganmbjdra.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gnxschxpu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gdqkhadvg.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gyigbpedu.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gkxpkteio.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gcpodimdf.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gzangylon.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkgjthmic.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ggmrkjzqe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ghvedbasn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ggjpwzcou.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gdsscfzaf.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/ghdlgvhou.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gimpowmyd.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gbmomgspu.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/glneztazy.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gvysevzdk.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/goxcrihbc.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gjoxjmytz.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gbjvzwdrm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gvfxrdthv.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gdeikvsby.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/ggqbqpsyj.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gybhlapxo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gkwilivzf.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gxioxvsos.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gritmtehq.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gmpiytgge.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gkmynfngb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gxluentpq.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gkvuldfav.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/ghtzzwhdb.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gnmfqqdul.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gywggjvfe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gzfupolez.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gmozabajh.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gvooluyed.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gnecqzofr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gzeqfwxkh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gcacrgxvj.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gludticaj.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/ghjqcfydv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/ggesbvngg.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/glnksrtqv.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gelgopctl.sHtML


<!-- 参考信息 -->