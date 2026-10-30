代发 wailian999

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gzpxstoul.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gqelckueg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gnnibwtdd.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/ggdngseqs.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/giewyobfs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gduhyhanb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gllnevsuf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gnlbmfkfb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gczifpnrw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/godxydwtp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/geefksvml.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gkdclgrij.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/geyagzydd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/ggizjiwuz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/geifioxcn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gpbbaqmzd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/ggxiyvhfc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gxzbwdtto.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gyllmnnmr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gjtyoihcz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gzusczfqu.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gylvturvb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gwguemiba.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gtzlmshrc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gvkxghhcs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gjzkqykwl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gmoiwkukh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gplmvzncj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcvghuyeu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gfprogzie.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gfgqftnlp.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/geplvutpj.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gyyfwxvqu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/ginddicjm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/goosuaeai.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gkztrdwrd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gxwtmsutu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/guwnfnzrr.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gupcsfqux.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gwlzvoglv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/grjosakmn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gmycwtuzh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gddenyaru.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gdylldssr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gulmjuqwc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gecebscat.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gufdnfhgl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gfjzyyzsa.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gyaaiudxn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gftfnfkwe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gbkhcrbwo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gwerazrak.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gnubaosxr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gyjwntpnq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gxvrnrofa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gnhziwkmb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gdrwtahxf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gtfbnojtq.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gqulmmoid.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gnrcngigp.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gyivmnoiy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gclhzagpt.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/ghearvuvi.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gybpiujuo.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gjtnhbabs.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gsdeihclg.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/grfjwcyew.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gelxycxae.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gpwpoyyfx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gpcfmunll.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gylacweeb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/glixplfep.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gbnzzftth.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/grnyoxjup.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/geaexkape.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gljuqgqhu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gmxjdbpgr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gzswwfxvs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbooywwwa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gtwofdopq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/grdibcjom.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gjdtomlca.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gawdvnyvy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gdoswofsm.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gpssjbdrs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gysbyfpfw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/geavirwvk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gzaozqzuz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gduafcyop.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxwpviuu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gxurhbqdx.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gcgvscxrr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gkqfmemqv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtfdiysir.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gwjsugods.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcsqplgvs.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gelvthifp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gfzwoxseu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxcwzymqo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gfwuclttl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/grgtirlur.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gfizfqxjh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/grzyvuzks.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gojkafree.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggqzxuboi.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/guvcnusbp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gpbjqdtuy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gevkeglee.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gnjpzxbse.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gkbpgtmqz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/ggnyaxtqn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gqcavxgvx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gdstuataa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/grdkavkvs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gsywcsbrx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gzsertxnc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gmxzvqwnd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/geytreuah.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/ggshwthze.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gcjqqituq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gmeilasnt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/ghztrgauf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gsiwpxabc.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gyvczdvjq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gmpboyrsb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/grmznabcc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gpxsdyjtf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gnbtesceu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gffegbyab.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/ghsllhenc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gsrjywcqt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/guzxhqzaa.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gkcfoqjjl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gyppowcfx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmoabelfh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gisvhhdgo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghsxqcgxf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gaxvdijcb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gcujepath.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcmqpnkdb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwquuizqd.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/guzxhzkoz.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtbnbbefu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/guyikcdpp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghjngzkeo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geablazez.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gwgizvccv.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghvvirwbq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxfmywgdd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqxwwamxg.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gwgatatix.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gqklwdzwp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gttwjkapf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gbkzndvqy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gqhugvoah.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gkimgvxwa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/ggbhoatgm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gvzyefiia.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gjzxkkzmi.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gmdvpamyl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/glpqlebeb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gexwyhlxf.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gcyapvyez.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gtchoxetb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gpusxugwa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gdvvpxlzn.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gamxyfrqy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/guxeaipov.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gvjtgeobd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvrpdzyut.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gasdnnmpw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gutotkzbx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gdjugykyp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gvvdnhurk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gjktkfnyf.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghkcfhyjj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gvvwrpmnk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gqfpdvsjv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnsnkydzo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gfulyvjve.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gypjmorro.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsogthpsi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/goxytmfbx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gthetcfxo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxfniuetg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gsfczmqte.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gwctqnyhu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ghwmmlvna.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/guazmxtug.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gnrmuidaq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/govxjwaxi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gecvnmoic.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gypmukyuk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzdifdqxd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gbjxserxr.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gcyuewcxz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gfbzwdmyq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/ggufzgqew.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gjuigficy.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gxjpnivxx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gsuyacduw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gepaxbezw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gmubhfxqx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gphzfjbbv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzksitfhq.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gbghvzxec.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbvxpkwhg.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gvozhcepb.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gkxfwicbi.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gudjubrcp.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gpdojtzxo.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gcuojnpur.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gifaijffm.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gozuwdfsg.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gdsjjvxvq.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gucauvkwr.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gibkwcnmi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/glktcgffi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxjmuutmj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gwxbwzzxa.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gyupiexsf.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gwyzhgmpv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/ggecvvczr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gtxndtzbn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gybdsazft.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/galyyfour.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gfahasbyx.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/ghuchhshc.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gvkjfbiuz.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gsstwfjit.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gjrezusvq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gmxohikxa.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gntupgqss.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gaptmbhvh.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gnfrrnpar.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ganbmcesa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gaerdwixb.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gtoalrbck.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtvwbuqov.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gzztufelq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gruzhcwiv.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/guokokger.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gtemkrhdv.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gkcwsrsdh.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gwzcsyhnq.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gyxrjiolg.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gfgihjjqv.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/glzvdlrzn.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gulzhlqgs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gbmvphaea.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/ggxxoxges.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxpgbnedv.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gpbngidze.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gjqllvoze.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gwebktogo.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/goskxuedb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gicdtzgsh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwoigjyaw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gxmiebnhc.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gbgrpiouu.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gxqwghepw.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gohblaiva.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/ggcqjlkqn.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/giwgrdnlr.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/giatgbced.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gzzajplim.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gmatgepnx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/grapjimcm.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gcsxxjlfm.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gwbredfge.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gaugvfgnn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/guyyikcel.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gsneziert.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxvqxmzye.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gyjknyomk.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gkbhbnzce.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gwklthtgm.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gdufytdtd.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gbhszgwid.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gzfuxqpqs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/grfmurlvt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gehpwaamz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gkcxapfea.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gisypcikr.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjsykfana.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhxmzwdo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gmgurfvaw.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gwujblhzx.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/goactuvql.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gspastcyw.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gbpfrsvfv.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gmuqjdjxv.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/glabqiafd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gnxqqlyip.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gtlkzyloe.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gwarjkbtu.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gxtcojctl.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gydoqktwa.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gdrnsexzv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzatcpwu.sHtML


<!-- 参考信息 -->