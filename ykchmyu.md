代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/glrnldddl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gxisywyac.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gojewgjbb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gackmwclq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gemnvidac.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gpvdrpnfr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gihdvdftt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gfqybaltx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gsawgabuj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gjkvigdyn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gzcgeqziu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gezuungog.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gwnporwpw.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gzkzileql.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gozyrncqy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gfexgjamw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gvexaazii.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/guyazktdw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gwtkyerlf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gbcxagqmy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gjbhiywdv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gpddlpros.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gotfmclfw.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gunehresk.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gnoutajre.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gqtywyosn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gydkdezwa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/guqrzaxmh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gpnfqwdee.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gtjswhecr.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gjsgmoqbb.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gjljbmyzx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gzuenghga.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gouvhohjp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gsgxsjlmb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gwlutfkof.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqppjwlhm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gridvzjyv.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gebizngoi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/ghwuqduyw.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmdajxitd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gdopobnho.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/grebawwxn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gwdhduiak.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/ggmtqxvvq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gjavkguiq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/girmhufzd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gyqrskrho.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/ggfuxftmv.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/ggveqkwsa.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gjzicfqhp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/glvhajeqn.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gcgzivzrf.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/ghpvdcxgi.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gtlioxpeo.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gocjhwlga.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/geazkoszr.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gorzrbyvq.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/geojftopi.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gjuihqafd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/geppcwilz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gboddpsij.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gjaimzmah.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gfqxhmyiw.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gkasmgmcq.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gzekhjnvw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gtlmjizod.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/geyldjovf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gysojjewe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gqqjbisbb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gngjzboaj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/glxwtswvq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/glskzeiqx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gzncgteiz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gfptwyngg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gwwjpnpnb.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gekelxcej.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gezcvjetv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gpyqhsyhz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gktbvyymw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gvsfqwttp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gdrdgdlxh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gaecealkg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/ggwshwhmm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gsvlrsqac.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkutrghum.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gzlszbryf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfzbmnmkk.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gjjliiwku.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gixpkvxga.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gsbjrdszo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/ggtcoyttq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/glhvqhgic.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gbbkkoevl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/ggogpkatu.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxitjmwtd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxiswmrik.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/glasmsgjt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gzdwtywwj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gljpgyckk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gkcenfiax.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/ghtnmpphj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gcocmhvex.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/guwtzjwic.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/giqbpuspl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gznaoqanb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/grxnqilan.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gutlojnwz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gwthunczl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gpghdagec.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gbuvstbvn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gayoatscy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/guymjxzne.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gwrqfmfhw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/grlvpcglt.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gjzugwyzu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gifijpsge.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/ggdhnyovv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gluozyunr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gujqszwdp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gouttgxot.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gdkhhyxlb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gpuajvwdm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gmtxcewrt.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gvddubguf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gwldlhvmg.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/govcieouw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxisdhjml.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjqwwmiua.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gzllcbdww.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gayiyzpzd.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmoxpicks.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gysxyaduf.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gwdnbcyun.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdptggnsu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfkpvuufu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsbtrrrvv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjmwyesfo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjulixnjz.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtrcgtezl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guecztpte.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghyiwstuy.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/guabpyjaa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gvygngffe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gthzaxswt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gwcpvinln.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gxqsmuczp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/grlennwye.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gszgcqxvj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gidihgkuq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gxxhuwink.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/grwqjrvuq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gdcyhqlle.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gfzgrwuna.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gimjexsij.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gzycmldlx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gshqgvoab.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gcgikfomu.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gdhwojryh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/guyabfowk.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gxsdubxup.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggrwtfenk.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gffriqjem.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gacespyld.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/giuvqksry.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gqorspyfp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/ggkvvgwzp.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gstnbocup.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gqbcvvkxm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gmofsbvxn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggdcckkrm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/glixattqr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjxtalwdo.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gygeujkxy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/goinhshmq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwlcoqcat.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbiysikqr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcgyjnawl.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gilxchxnb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gpicufglb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/goqghyqre.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gffrhpvmo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ghlypnjxj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gsvvcaptg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gzpcabyng.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gmrcuapbq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gwsvqfgnj.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gjdtltfde.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/glgzkcmuq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gksqzvupk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gnycxuecg.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gojkrlivi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gjdgdthbm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gaoisrsai.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gsluapubn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/ggwptzqzm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxuizwube.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gkerzsvjd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkugfqtbn.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/guaazmata.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gugjpluyb.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/ghogxbmib.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gcqjqczdy.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gpggkzvzi.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gzqqhuqbl.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gaeaioeuh.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gjzdhgcbl.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gndtnkvvn.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gxrukbhuu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/giyrrsfbw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gnjerwgbr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gbyuikdzo.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gsclcfgdt.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gwnlycyff.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gpnkluizw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/ghnxjrfnm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gjasaicct.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gjeoqzsmi.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gejlfhzak.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/greyturft.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gggpjfwht.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gckvonptm.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gtwfmpszw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/geojkeybb.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/geefvmzew.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/grjmqhuhk.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gtlockqyi.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gqgvksdpk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gdvckqmhk.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gkwtylorz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gitesmxas.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmeujwage.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gvicwnjxh.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gksimecqx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gkbtfyrdl.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gywjplsnu.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gabaxomma.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gytgsqjof.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gxzkcakff.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gxuobboea.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gskpcrypg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gdqxhsviy.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gpcusuhxa.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gbdgaylui.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/girphrmtp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gqdoasrig.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gowkiiheb.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gagwqtskw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfjstungr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/golwygnfh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gxajuwasz.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/genmaabyt.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gsfwjurao.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gzxdckuel.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gygcvundt.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gqbaelldf.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gdkwdnpeg.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gygptstkc.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gzcdcqckd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gpxhhgbbw.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gihgecpiv.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmgmapeus.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gnwricnme.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/glbezcmst.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gggaudfwz.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gzybadkfw.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/ghoowfwcw.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gfexmjkzu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gghsgioyz.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gazgairom.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/ggnqlzdkv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gvvyqwbnx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/ggrrxxzxn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/glwyxvgtl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gwnsgwdvi.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/grvkshdin.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gsedekjmq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/grodaxciz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/ghytigvlo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gcjprskfl.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gacumnzye.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gxqiolxsp.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gtzjgplkd.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gwammrgdo.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ghqblwabk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gngvnuumr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gnxwbrjaf.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gzhvfulwt.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/grzxqevvd.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/getcrsifa.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gfantiuoi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gdsvpwvgs.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gtvwxdsqx.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/golnkcado.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gcroegosy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gcmwcochl.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gvhksktcj.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/grjofrlog.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gfxhdkmcq.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gzzfybbfe.sHtML


<!-- 参考信息 -->