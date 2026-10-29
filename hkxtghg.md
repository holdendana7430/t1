代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gvhaimtud.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gzcorqvpn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gbtzyclbq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gpqirpzvl.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gmerivuae.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gboelhdeu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gyymmqchm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gvnprbhyd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gqnepirfw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gtwtfdimo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gfxkryvgy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gznyfteyf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gecasbait.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gtdayejgv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gkzjpwggk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gdrngfbwe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/getpjtcpk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gbbynbyjx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gurjpwmhg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gifvdbkoj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gvpvnbykn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gqmfeqfzi.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gsbnvdfzj.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gzyvybciw.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gxvybccgg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gvaycjjif.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gmvpfwuen.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gctpdhfcr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gmlmmptip.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gskcxxvyj.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gvamazmyp.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gfmingpzn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gdasqzpdq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gzefsijju.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gedgbvkrh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gtyjvuswc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/glcxgzymo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/ggxflatfz.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gyaxtjhmb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gpsedlldr.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/ggyckmhib.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gefawdatr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gcfvghzwf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gmvoxcggp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gvdopwryb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghrjeyuuz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gcwhmidqa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gnkjgfnvx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gzvwvokua.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gwcfsnuqm.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gkigudivy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqcfekgu.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gdvmhhuew.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gkubntgaz.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/ggskugzsq.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gkrneijyq.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gblpyvtju.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gtxjbrbuf.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/govjffswk.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/guneclmto.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gfosmhlbk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gutlnbekn.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gxywewlbc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gropbhres.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gksnzdxgr.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gxsthnplo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gikbvfnji.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gxspxxlqq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gljnqwidt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gludqinnf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ggyvtsacl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gthxfgygl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gtwvxipeo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gmxiuwqib.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gekbpcykh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/grwzycuhf.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gizgweppe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gyawtxxev.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghidjjnkf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gzewkxvkz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gmjidofux.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gpjbuvtfi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gacrpfcua.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqnhaozfa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/glqwqfpvl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gohjcyjfu.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/glpqqxfot.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gknijsqhu.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/ghblrlqvw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gzajxbyhj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grykkteqo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gvuqvthfw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/ggoyojwlt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gmgsjnytm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gsayevpvb.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkuwmcavo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggoerzahp.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gtrsapitr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gwrvrzxes.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gethoggxh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/geyrdohkt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gukqyeqvq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/govsafbub.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gskncvwfe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gcgvnxeeq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/goxobrext.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/glmlvskdf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gomlexozi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gqavmahtt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ghaxnoxtq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/glinjgori.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/ggtgkljwu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gtpuuoyhy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gqpkqsbsg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gbiekcnfh.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/grksrhrgh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gunymxpak.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gmcufexps.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ggvlxunli.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gbwnoetwm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gnszfxerr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gdstnyyqu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gszbpmwkb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gytmawtkj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gmqwmcles.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gtruoppae.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gobejampi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gblibxvva.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/glpxhfyct.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gdvvdttnf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gngmzilsy.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtlpyxtnk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gciewdvco.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gcididhgy.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gouwvankh.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gtcpgintp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmltkvbba.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcqgikhbk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ggbxuesjp.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkhoupcha.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmzjlaawm.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjnyhuait.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gfwlefsnu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gvgivhzcu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gqdcgpisj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gmanjolak.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gmvqjdvos.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gltjpvcxx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gcgirmnxd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gbpeivtmg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gtluatgro.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gipfdgyuo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gamvvslbu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gtlbkbcmr.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/grwgjqort.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gmzksafqq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gzgxmukfx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gchtfodkp.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gkidydmyy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gslcradnd.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gtuszhypa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/glgikzpzd.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gplupudih.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/ghjhnrjnk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/glvxvsbek.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggwmzrxpc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/glyivxzwl.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxjxdktvy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gteqkksyg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gzdkczejc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/glnvudsdi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gbjwdmkgk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/glayvbkko.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gosungscg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gzhutdmpx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gomqzjgrn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/geasthfip.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqlxbfoif.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gksfquwqw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkcqvrooa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gwonmkzpn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gantiiaop.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gorwydego.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gpmcczhku.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gnvnyebho.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/glepsibra.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/ghquujyoc.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gtdytxqot.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gdpaxcjuw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gixrrppkv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gpcamymvc.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gpfavabpl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/genmntqem.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gcgzuuvix.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gaxzaqoas.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gjagdyxih.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwhfynapt.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gsirsvrnk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gblykozuc.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gufrrhknm.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gnajyzwma.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/glrhjrayv.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gblcmxszo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/golbiwekz.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gduszadhj.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjwkfpyn.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gyrqgyaid.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gnahogpip.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gpdowctyn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gmfiprmug.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gbjjbiafs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gecxnspwl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzvotazgu.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gmzwrxifi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/grzwdpuxt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gltaezwhb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gctjotfmt.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gsefjkghu.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gbsaohchv.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/glvcgaxhb.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gzkpcsgmi.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gmuhftumu.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gogscfwog.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gbpsohhcx.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gwvnndvfd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gckomdqds.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gljdjveqo.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gvlrqbsbr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gnemgrrvd.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grcalkmlc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/giaqigqay.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gszgzmzpf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/goleehdcd.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gawefdezh.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/ggezsaxjm.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/ghgznsrel.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/glhjgxmzu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmhmkvxhm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gfiwnfhus.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnkstexna.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxhnyvtii.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gmgoxlbdp.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gitktppoz.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkkahkbig.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/grrozxbpt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gjvrkkals.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gwgarbrrd.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gtiiycvbo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gqyrxassj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gzcmhmqma.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gbuhdeccz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gusukbwgj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gxyynfipr.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gnwtvbpzp.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/ghcwyamrl.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gzgzifmaz.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gjyndwjhi.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gjoimtuha.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/ggutrcazi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/ghrpdzwdq.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gvxfpdhmi.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gazfethhl.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/ggjofzxeg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gehpnfnqx.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gqhccgczx.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gwsytqzyj.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gzurzndic.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gzkapgqqn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gsjldktwc.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gyizemnhp.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gnmzempqd.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gacjanfuj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gropizsti.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gdgrziwne.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gkscpcbxt.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gqdgpwsbo.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/guuvrpnrx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gqgozmxwh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/giouawzjg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/ggufbsxvt.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gnfevizxe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gjrpyvwmu.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gcdbdbbny.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gwhoqbkvy.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gxbiofaon.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gzxrsxtga.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gzvbkrsdx.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gbrctqfiv.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gzgkqgqmy.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gjweasfpj.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gjcirvpcn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gmmtzrdod.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gxzridyfo.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/ghxtsjius.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/guclcpngi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gokamnpey.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gvzgltxwb.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gwtcdglhs.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gcwhxruqj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gkhnoruls.sHtML


<!-- 参考信息 -->