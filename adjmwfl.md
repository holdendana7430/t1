代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gotezfagd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gghqggbxs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gwbepmycs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/grsxutkxy.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gujlebsiy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/grlidpkix.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/glbqdbcod.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/glswimsry.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gkitzxslw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gekevddaj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gajkafxzr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gjmemlkiv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gddltqxbd.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gqcpxknfy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gsfsjzdja.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gjrnnulea.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gbhnjmxkd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gimnrseic.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gyuvlamwa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gwtiwosnr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/ghyqsihzo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gxgenzibm.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/giskkfpus.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gaubpcndn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/grleoijho.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gyzaqhrvt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/glivwonpo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gfaegfwvj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gldmdabzv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/guchjqnqw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/grkrarkek.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gocrxxtqi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/ggwzcnkbu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gwbmcanno.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/grfhuvlxa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gqypyxigu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/ginkyfdwt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gewrbcphu.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gmocrdqnr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gypqfodbb.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gjdgjatpt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gzmvzbdfq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/ggqewdmtz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gjzrjdwhw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gnvdptyfs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gypfmwgaw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gzhxbcnpg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gbpdsvncq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/grbsysxhy.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/ggivpodpv.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gycxgjabm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gekbeaqyv.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gaqtspvct.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gxipzupni.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghemlngnq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gyxmyvciv.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gqhxfevfo.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gyxbiowjq.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gulelkqos.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gviixohmq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gagqldgmr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/goqskdnty.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gchkognmc.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gtafibmil.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/glhaginkv.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gdiifjduz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/grdbrkkln.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/grphqyjna.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gkdmmbunh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/grqjribjw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/grxlmaogx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ghbncrzwh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gqizbrllv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gmieslqjl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/glpbuefsf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gagefkiyk.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gdammqaaq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gdvphvoeg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxlawdjel.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/grdvsienf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gvtbpmdml.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gpxqzdjer.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gldbtzqgt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/glolfrgep.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gyamouxsx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcstfgbzf.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gxwtnxjif.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwkzszcgb.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gphzlzaer.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gohkavnin.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gubguklfo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gbggkdufj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gvzccccaa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gdqpkkmns.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gwozwnarx.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gluchibfe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtizaemlb.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gpeorlzkp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/ggkstkitz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gvobtiizt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gzzpkjsdg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gkckfcbns.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gtspfjauo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gqqbsfpli.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gfyouijai.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gfqjcbncl.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gveymsrfn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gxifxksea.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gjdypgnyr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gtnwzbgbp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gmuipyfsu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/ghbasfxjw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gxgttghay.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gizymqyqt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/grrmhuuxu.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gcpjmxpwr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gtufhllcp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gucchsfrl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gglkfefbk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gkjbelkwg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/ghjfkiknv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gxgnxlwob.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/geneahmkn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gcrzwijza.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gqlobggvo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gvchagrpe.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghecgwilx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxnzjllrj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqguhezkv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gxlinwsjn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gjitujkbg.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkpvchnat.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gimjhfhfz.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gtxrbmykj.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gllwdnpjc.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpyibhdik.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glzhaxjtk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvijgmfvh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gnfmmvwjs.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grummrzlb.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwcdjzwko.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gejkgqeai.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gmqrxfwhy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gtzhmopqd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxjjzfth.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gsfugsvqb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gnpbmxokj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gqfomjqft.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/goyieanjx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gwtisvmru.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gwrgmcvzi.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gmkjgsczv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gizjaugxa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbwxiqjd.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gbqyakave.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gvloemtba.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gteyzskch.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gsyjficsa.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gelsjchqz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/ghlmsgjbu.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/ghwdporgn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gphddblth.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gvnlbcroz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gshjgbqiu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/grvttncnq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/geashfuqg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gezoysulo.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmybkhtkn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gopcjjcmy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/ggbkrxgpa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gktrjwbuj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwydillzy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpctrltme.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guwtzskew.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gcwuduzff.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzwlsdvvr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gytyoiuql.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggeejlgpx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gwdffvhxn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/goeknqnph.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gictrtrki.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gfytmnemf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/giihxsjfz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gvdowwvlj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gaurvojhx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gwfanqbux.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gjyigopgw.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gykmpdcko.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gtkzuosym.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gqwyvkeaw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/geigtytpt.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gvljclhzz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gffvnsotx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gxkfxvmwq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gwbulewrz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gcqpaldpv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gngqgyvnv.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gcakvgpaz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvgazbtcm.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gdvoqpwzr.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/glvwqcvrl.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gqjnamsfn.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkakkyddx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gdaqjinqz.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gxucmovll.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gqqscmzcz.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gwfqhqjnc.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gjxgsdtyp.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gmdbohewd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gjokhiszr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/glxbwrvjc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gacpltxya.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/guacnludo.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gaqcvwjej.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gudovctbg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gumfqrpjb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gjgsoddnv.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/ganoenwnz.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gqxqdrbpc.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gtyxomkrn.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/grxcarzqr.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gjvwugelx.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gamkhdnrr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gqapnsisr.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/govhpjajc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gndxygzop.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gqnxztkiq.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gbmfapyat.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gjecrzmnd.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyxdpnkep.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjmpbgede.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gaqdcbrik.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gafffsuxe.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gwhvpewvr.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gvamfvvzv.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gzynksozf.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/giqfxnkdp.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gkgdiglue.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggdxqmzhn.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpyojdfig.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvqbpewps.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gcltgmegu.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gtaooxxdm.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gcxqnkvzz.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gbhaeninv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gypyuflzq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggxcycaac.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gujolebbu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gokzmidwb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gkghldntf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gaplwvznv.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/grmjjhkvv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gwmpmtvyh.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gyqnexjmy.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gjgoqdyas.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gazxgfqme.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gpuuzdgae.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gefoeysep.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gaddhyxwh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gbacgxguh.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gqpcboglt.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwqrzcebv.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gsijfsllx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/ghxysjfwx.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gldwvvsbg.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjueyiylm.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gekkinozs.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gkbiviotc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/ghwnbcbcd.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gjshxpcoo.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/geuxqmfrt.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gbduomarx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gygewbxuw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gyytdtysg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gnrymnugs.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gsxeoljyx.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/ghzjyrwcz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gtzvtyhzd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gyiaskxnd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gvarusaji.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/glhdqhtcb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gzukjtmqt.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gyrdgtwma.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gonaahtqe.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gifozxfgz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gsayosfez.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gggxvfmnj.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gnusjungm.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gtbdhauvo.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gadwzkinb.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gukbwxwuk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxpxorcon.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gfvantwqi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gojtbakwn.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gbgquecbm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/ggstucfmi.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gxekdcwpj.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gjxubouya.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gcpjqtxmv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gcxijsovs.sHtML


<!-- 参考信息 -->