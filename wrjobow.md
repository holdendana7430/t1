代发 wailian999

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gmfogicks.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gtiqbyczl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gjiylwhmu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gzgdwpiep.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gncyarwmq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gomipxuwm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gtyayqoty.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gttnvdulf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gpjjwzawb.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gsldnpgpf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gshulntbb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/ggtbvnawk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gattkwqfq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gsudlbupg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gelsttkzi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gcbfdeeny.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/ghpkwebtl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gkfdskcmq.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/ggpxrixzs.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gpwybtjma.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gqehkhdys.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gwrkeziix.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ghmkpmwkd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ghwqlhfws.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gnzvepxuf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gvgyvdueo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gsvmezvyw.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gmosjatav.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gmzfdbvil.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/grzgeabon.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gpdmwzvti.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/geaolzwgw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/ggttaeaum.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/ggznpfmfh.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/geiptsdlx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/giumqfwpo.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gmscuoifa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gqmfdkmco.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gpsusqfbr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gwkffccvq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gahysjize.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gezsthrhk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gjouqnvxq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gxsxgovpk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfhaamkiz.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gineezxmz.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gttwukcpl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ginqnqmyx.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gblmeiwpk.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gcfradsqj.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gvrxdwwdf.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gdpkevimz.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gyviyjpvl.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gixlofvji.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/givikdzkh.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/glvxrqnsc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gpdcjjrad.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gjscolbdy.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gtsoxrqfg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gtwoxlbvl.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gtzskqlhy.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gepkdxcvg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gfcnudzjj.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/giipmhdvs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gmotmkrot.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gdgmzqkmr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gackrqyer.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gimmhqulb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gnejxokvc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gtzkivjut.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gmzcqvyvw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gdvqtazhl.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gpzgiplxk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/ggwynnbsu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ghhntwotk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gjevgvpwy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gpgcjmynx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gumunobsa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gudvtftee.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gmucdwjox.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/ggjvubxez.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvmopkbjh.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/ghllebvep.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqlanpfaz.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gmmqzflzv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gifcmgwlz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/goorwqgle.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/goivizdiu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/geezqbgeb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdknwbvnh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gerdympvh.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghqbnsdzt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghkzfbjle.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gwbqfzsaz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gfrtkurrb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gigknejvt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gluvbwxia.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/goziaoldx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/genkzxjum.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/geztbrqrw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gqzfgdebg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/goczvjuce.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gupdehoow.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gjvqggrpv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gkjuxpszv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gseuuspel.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gizietjna.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gdzzylgfq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gbxudzflo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gyxlqogaq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/geuowyfvu.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gxvhsxmwy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/ggtdjwjvv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gwdgzcezm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gbkmddxbl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gnjjdyqjy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gwbxviygl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gspukkbtb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/grnkkhcqg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gkmbebhja.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/geslrvcpq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gnoacyruc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnbxrhhug.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gehmqjeso.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghyywlvuz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gzopukosl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gtturacxt.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnqfebtgq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqkvyvdmg.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gvbrevjaj.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gozpvqfnp.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gyctzctuh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsegvscnl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjttlxaav.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/guggkvyox.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcvnshzqh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtcobferg.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbvhcospy.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gcaelxxmd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gxgeiddks.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gwdmsbjje.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/grkivouii.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gehvzqexj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gdvghgdii.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/ggsjbhmxk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/ggapjqigo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gtsfkzylk.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gprudgzby.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gqthhxjmw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gfqdweigr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwsvhver.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gkvnhsivq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gunznnalg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gdqtjaogi.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gzoenqwwf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/grtbojjcs.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/guczkdgti.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gasyvtumx.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/guzqvrhme.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gmytzhxkc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gwxynwpbq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gnabwdzxr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/grkekvewq.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdrrtjxwu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gfwoklxne.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gujrwminw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghdvkmadj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsacnoerj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gttiutdbq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gptzgagth.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/ghdutprga.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gdthwbswp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbddysnvd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/goyvqnnmr.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gysyqjbox.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ghjjwbgdh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghmwwoqdp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gccbquybx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gclvnljom.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/giuagrvhv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/ggthkwrsp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ghboxdpaz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/glhiijhwy.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gzygwjigc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gflsarvvy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/goohxcfcw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/goednjilg.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gsuzrlbkq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gfjdaitcs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gfmyymrtj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gjqxyrsrw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gjfrhfvpe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkdcgoalg.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/garbvoqrn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghdmprxsw.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gruujvexr.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gdhnjzamz.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkuowkkcq.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/grcedqhne.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gurledqmn.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gyloduyve.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/giwqlcdby.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gkbubapuv.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gqeacpcma.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gfvywnwje.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gnfbcfrxp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gvfpulfmn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/ghvqbhwhz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gosruezwc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gjppfiqaz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/glmsvabnd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/ghahvbixr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gfkejolxn.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/ghhjiqbog.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gfcimgpzr.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gnhebvzor.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gadrxmrga.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/ggbowwerf.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/giiqwvvrq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/ghxkpjftj.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gxnmhfrdh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmdrsmwlo.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gygkxlluh.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/glenydwsw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gvkzcxera.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gdjnxvxrr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdlsxppst.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gskzlahem.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gicvpzeia.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gjeeddfqe.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/giltlttuv.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gjmtqpnxl.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gukkekwlu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gggwjndtm.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/grzzzhilm.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvwibirhh.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gtwvmhegg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gdxeqovpe.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gzjojmoug.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gbmnamiki.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gkjuupxdt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gbtkyrrcm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gihvwedvm.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gopuyjfma.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gdloewpbq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gsyncprtt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gykbgpvdf.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gndhspbmp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gheerzgfx.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/goxjdwwar.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gwibvhdcm.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gaxfobhxg.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gpiljyiyh.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/grpmvlfil.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gwjgwyear.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gqewhckoz.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gimacewkw.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gyktavibz.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gkovjuqib.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gnsyqajpm.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gzjkwurrr.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gzjoeydaz.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gcrgngilv.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gjinbikws.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gxlrgdoyr.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gqsoklzqc.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gxtfwsoxa.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/guvykopuk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gnvoqalcy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gchhjboma.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/glddifusz.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gxvgcdsrs.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gusemgnpl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gihlqlxwc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gbijwlcgg.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gabkkgwze.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gugfiruxr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gmakvgrxa.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gkkigjlvw.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gadgnlqbg.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gvplddnnm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gzylwzaoy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gmherwgii.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghnmmivkm.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gmpbcqnai.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gggiepzso.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gckistocn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gfuqardgn.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkaiplngw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gbuqjegeu.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gciigalrj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsacdpjn.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gmuluskre.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gisttttwo.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gkmavywqu.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gnbbeybsm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtdlnptci.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpvemyplp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggqtznflm.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/ggtvhzxhr.sHtML


<!-- 参考信息 -->