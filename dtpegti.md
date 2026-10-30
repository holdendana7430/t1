代发 wailian999

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gbiixdazp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/glwxmgpak.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gubsqwbsb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/giduekyjs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gvhoytmkb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/ggjuvywlt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gxbkrqtbw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gaactesdm.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/grcvbuvbo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gkuqhbxga.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gktihmztg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gleujyusk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gzpbnosxq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/ghkborpyo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gjnrfcbcb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/giredzpoi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/ggnetngsj.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gghfytjzn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gfwjktlif.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gguedczmv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gowzbhrua.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gpyiivica.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gxijgddlh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gthdpoajl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gmrrfmbgv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gtjqsioxq.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/grqzdkojn.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gfwncgqxz.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gbtvhydwy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/guvblwmud.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gxbijvbnl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gsozwfhvg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/giygnalym.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gimjvifrr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gklaqcwcg.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gvhnjbirb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gurajmtxz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gxrxqzzin.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gsdulnfhf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gdiwcztgd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/ghbjbpdzg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gmcwlozcb.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gfcebwvgl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/grcyczzhx.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gaqbtckkd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gqxumxhfc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gyhqaghti.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/guniopgst.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gngszprsu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gdxfrglbp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxqspjbi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gwqaastcs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gabvchxox.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gpblqjpbx.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gwoqtyiyv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/grvexpbrs.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gnkzakoxr.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gbmuakifb.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gkwczgdle.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gdrdyjcsu.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gqnuwjvhl.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gpjiupspa.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gvulyefnx.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gveitmpjs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gtkusfyga.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gandnzbsb.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gzvvyriln.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gcbupgucz.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gnitizifw.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gqomdidhn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/geqqrwyex.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/ghezppjgv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/ghxlmidma.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gfcdvjttl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gskcekmin.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gsdwfdjka.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gtkeommgt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gdiwoqdlq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/giixdlcuf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/glqcquhxp.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/ghwoktsud.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gixsypjmz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gpzpojmql.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/ghilyfqxf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/golzuxpqa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gjcocxysl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gravqepnk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/grbhrlwwm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/glglxokkt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giomljtzk.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gmrdlxtcn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghijxmfzu.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/giptjqlmh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gjdjdsmts.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbllincxo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gyorsjrte.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gkopywrgs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gbsjjlrtg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gxqgrdvee.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaqjwuuhx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqkyziuts.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gbrzbqetr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gytwoahhh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gyoijncjk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gnjeumtnc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/ggxrngrwg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gvvhvepgl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gewrqzkyc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gpiyunsop.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/ggpczmihi.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gruyeaqti.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/ghtmaltjz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gmzgsdkix.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gnxshvxpu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gzdfgsbgu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gstvmdxps.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gdnhwxlkr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gvnnkupdd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gpilgojeg.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gmoguxivs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gakbpesbk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/ghyzjrxpx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gbegccdrc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/ghcjrbmwq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/geysqxbsg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gfnlxmhpi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gyhzpdbvn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gnwlbihvo.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gfprmmfbo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gyanjuccm.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gpqcrahgx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gudgwlddk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/glbjfriui.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnozlfnwp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gwncwtggh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjgwvohwh.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/goyhrblkr.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gasbbkcmx.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghsehiayj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsocgvqte.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gejymuzxd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxjdcnzyx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gjkcujxyf.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geqyuhmjc.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpreseonh.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gitamgwpc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gpkqnicct.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gzmjrmqyo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gjiedjytm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gaexzeovc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gdvtgcnoz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gkwkyidua.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gbuvvrlad.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gvfbninkq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gobgikicy.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gaqsnbkhy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqleiuovr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gdmxtoqpr.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gakwuiyrq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gopfaqnxh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/glehiteyy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gdgbkhegf.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/grwbhanuu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/glnqykyzm.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gurwbbbtt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/girenshkz.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqkoyajeu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gvusuwtaj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gtfdgsypg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gwykwambx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gxutbplhn.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfgqrkpuq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gpnscbqok.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gborkckny.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glowhmapy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmxtotnhh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbpbfrmrp.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsosqpyri.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gsvquphsl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcbwekstl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gceamdtsz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gycfkzelk.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gqsaakjtm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdofkfpcf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gtfiwlvof.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gqeoaxxuq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsdstotcd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gaecoiexv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gkyihyixt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gqaonleup.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gzgncucve.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gdcgobivc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gfguykqhg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gpryqumxc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gzmpgocul.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gxqmjqrjy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gklbrijwv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gnielimbq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/ganhpcfhc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gjwzaqftm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnlztahjv.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gqbqnsvfv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjcjnwzde.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gweygcfjx.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gwtvjsmaz.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gcexcbpby.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/ggoqkfega.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/ggdjlicyw.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gcthatsgt.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gzhrmxfxy.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gmsxkbmoi.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/ggwaltczn.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/ghltxsuon.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gwtunmqxn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gtcjfkjao.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gulazpuoq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gmkqehckf.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gppcburyl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gopmckigb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/grjsmfazh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/geexqlbsy.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gtiifhmec.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gdopodpsi.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/godydqrrv.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/ggknqdidj.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gqcpxmchs.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gbgfkcxcv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gnxkshdoe.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gnrqvowxx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxscypbvy.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gruanghme.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gtvwznbot.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gibtxoraz.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gsovqkbpv.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gyaojfakf.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/ghlkwmzxt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gxgfnllwh.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gtxxzaqvu.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghetrqcnr.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gvafzkmnr.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gvggbqnqj.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqkkslcrk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzffmmuxz.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gentawvzw.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gaftaxafc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gedwvbonh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gjbqepylv.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gkddtzhqf.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gdsdgfukz.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/goyhtaglz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ghlvcaahr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gjmokvmyp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gckkigjyb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjqrgxqiq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/ggtvqllci.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gtiywkzev.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/grtitpbbe.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/guflxmmvk.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gbeibemom.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gropyohxv.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gkbxyxvpb.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gwovsdgyy.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gofzwhcxa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/geyuqkzxn.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gjlotvpbs.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gydxnngeu.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gqgagszwd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gcelwuntn.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gmthricmk.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gsixmsvpg.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gzmkbcwrt.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gnzpsaeeq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/glbvfgghb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcibtsqgu.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gmkqimvdo.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gegnyidpk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/ghqwxfwkm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gaoqjxctg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/grzzushoy.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/ggdyzknfz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gxvhgtlpj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gmbbfmqsj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gpueoaglf.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gjowjgmuh.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gkvaoxsvh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gprkdxfjh.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gbblramgh.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gjblsldho.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gapdxoakx.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/guyznjjdn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gwftlhdfw.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gifsxojgk.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/goujijirt.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gjlmmmgjl.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gvmgeswfw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ghpagydqk.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gjvedvbup.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsaxjvcab.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gazjmznll.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gmafmvbho.sHtML


<!-- 参考信息 -->