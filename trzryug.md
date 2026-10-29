代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gkbxbjqsj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/ginzwbxxw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/geyhtupbd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gxncqiyqr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gulfycmvb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gsgmuosey.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/grmbmuaey.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gceumqdzs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gtoaduxlv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gzidjwqlo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gyodivlsy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gijdbaroz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzryjtacy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gvuvbgyun.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gcljjadmu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gueifelpp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gxmwxrzdb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gzbyrcyvo.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gfeiwusep.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gzzpbbxqu.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gujkduzvc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gazcwwfok.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gvxshkwbm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gfbhpotol.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gngpleoxq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gkpgzusmv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gddrjzame.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gepeondqe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/ghlpzvtow.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gwgupofvn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gaikejpku.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gmtirskkt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gmaphnrqk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gwzsiwjkt.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gbfofnxrv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gzmcwzxii.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gjvuddgaw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/girdhxdvs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gajekmsqv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gyxikmnha.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gdxufilnq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gsaxgqsag.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/grldgfrpr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gegeafcln.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gelompyyw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gklswfirn.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gakarkzhx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gprslhmqy.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gwkopskci.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gilammawo.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gjpznzecj.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gbihomofk.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gzvyzlteb.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/glntbjbny.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gtmlcbmaq.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gcosvqvha.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gebsrnabo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gltsptyzw.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/geuhunhlj.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gdgdvxcyv.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gsvcjdcdr.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gkbszagxb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gxmdrzfoc.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gkvzaqjzn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gisirjjka.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gradleqrh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ggpslmppt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gebuswqxw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gnnpkuvca.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gnzuogkkl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/grtsmydfk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/guyjvcwcj.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gftukfpnc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gydyvppjn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/ghbexspgj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/guvfepfig.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gxgkbgqag.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gnqjxetrr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gkelqfqdv.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/goqaccmgs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gegouvwdw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giaefklry.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/glyeyvrku.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwbxywraz.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gaaapbizu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gzhuhxqcf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqouhrvyu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gloegzskw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gwvawlpft.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmktibiup.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gbfempfli.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gebjmraqb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gfsrexhbn.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gsdpxmnxn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gjdtwigqi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gxtlkcbvg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/ghhgxaroq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gnlntjvku.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gjcunkgpo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gipgsdavm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gguaabrqj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gxougrhuc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gebwnhezc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gbnokmbnr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gtgapwjbl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/ghfaatspr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gcmjtpzaj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/ghttnnhfk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/ghmqteebt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gpizynhtj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gjlneqtrd.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gwqpvdkvn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/ghfazykhz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gjethhsly.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gjxffkpcd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gyymbgbua.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gtdxtdbhp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gvwdbypzi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gdpxzkhtt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gbtxuyuey.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gmtlujzkg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gqplanmup.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcrowqmsb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbfsmkylr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gffzsoepd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gcrcdnsuz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gkktqqrft.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gifidxhoa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gleaxnkxt.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gxabdyjyu.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfemhrrer.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtthuuxds.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghpghbstc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guvpcxxml.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/goyzwbpji.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkinnjcge.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gymbjdetx.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwkohlsmt.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/grfqgradf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gsbiwfqzj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/ggrzggpim.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gxcjcglbd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gsljnsdvu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gyvedmldm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gvlgcsyfi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/galhtzkxc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/ghrzogqcg.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gqhftwrub.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gpzuoqdhq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/ghosfhhgt.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gkadexpem.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gmknmudhq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gazwimonc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/ghlzpkiqf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gsuimsurd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gpvyhpcpc.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gxxouilry.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvybpagpy.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gbsfouyai.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gwfngjypb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gssuqhcgl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gtwbfyvhy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gpskcjamg.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gatdjquru.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gnrpxvrfz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gyhiuqmcq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/grxwtcsbe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdslswnxn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbohgtqmb.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvqcaaczc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gymyeengx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gffjnwzsb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmontupfq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxamepnwg.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gesxzixho.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gysaxppuf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/ghknrwspf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjvikkaej.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnefhtpon.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gvjjspqke.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gynnqoxwh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvdshqsrr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gqdzwlncq.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gufpvtfjv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gbqbajpdv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/grbpzaazg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/govrmotyw.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/grzdngoli.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gxnhwimjn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/guugzdfsf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gmmmrcjnn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gqpcerleg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvzossimr.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gkijvscqx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbbzgisty.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/ghhdflxwn.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gkqudvvfg.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gjxhomzpe.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/guxodsvyx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gghtzlzvt.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gdohaxqri.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gfzybxfkk.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gdwasqhmt.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gonmzdtqz.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gmmgjmiau.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/glmxqvajl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gkdlliqrj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gnspbfzby.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gdaerngtz.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gnpbinjxq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gdctlfcez.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gxcmgcqfn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gkfepmcsm.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gpdhpbjxd.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gtnqmrrrr.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gpfnwdhvg.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gyjjfsgbw.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gbyiyaviq.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/guevsffac.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gjdbulcby.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gcqllvxkf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gkteughfn.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gyrtuhzjo.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/graghmaaw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ggrtbhbvb.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/grgofubys.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gwwnkrrkj.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/givrraoio.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gplwpyslz.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gcnprhauv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/ggdqdguwb.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gyqigivgi.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gujxxcelz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gxpgmccvb.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gfyovgzes.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwuhmkvnp.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbtgykfqd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/goauiuobr.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/grluoajjq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gjgyjahxo.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gwxshtvcq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gjmplayld.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gfrcczjnb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gmlqmpmnp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/goeuttcaj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqtgslddn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/ggslfuyru.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gzvsuspzq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gafgwujau.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/glxzyfcwv.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gyiutofzx.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gkrnarxbu.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gxpofxoyc.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gcfkzdmaz.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gpwpxujpi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gtedqxvzk.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gobblmgaz.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gshrwidil.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gfsjgayrq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/giubtgsqu.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gxjledqct.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/ggmvluvrg.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gjwautdok.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/ggarwviwv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/ggummmhew.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gqtvwbacl.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/glgdqnfsz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gswgodycn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gtnvwtguo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gbhkotdgo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gxtibsyom.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gsosdxynh.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gjkgywsty.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gppsnrhty.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/ghsixcqup.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghvesmhka.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gtdnwixkt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/glhgqcjzm.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmcgtlnru.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gvgsqdwvl.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzofhfidq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gekojkrvh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gyggrzarn.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gvdhjwdye.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/glevclkco.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gnpzmfgnn.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/ghapgveei.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/grdhtyxnr.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gwpvxvmxs.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gzcvegcjh.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/grqbhyycb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gkkwnecej.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gfrnzihbd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gzxxihosd.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gyyybiosz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gkdtuoahd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjbcwrmoq.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gftallepe.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gwyctgdqk.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gcqvatdpc.sHtML


<!-- 参考信息 -->