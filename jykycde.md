代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gaoknahzi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/ggfmhopzh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/ghqucdtvq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gwbojachp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gojhvbmob.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gowzsmcoe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gsmzkawjm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gqsysmyhc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gsbvhpiag.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/guglooten.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gtzvkrbpa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gnrkhipjh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gatwfkojb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/ghwjysfld.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gqvwdrvzz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/graqyqhsg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gcxewdkgq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gftxzvxnb.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gjeqamzbi.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gehvzatwr.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/ghaeonuhx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/glarhzfod.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gtscicrez.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gjtbascwa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gfowowkse.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gvaigvihh.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gqchljjvi.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gixutlzmm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gjyjkhnva.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gvtcpnsus.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gcxtqhvhw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/glgzitdia.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gbxgpchjm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/ggssrgoic.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gpftsgpla.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gmcalwusx.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gcrxfeekw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/grabdqdoc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/ghxlozcdn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gtwybvjia.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gzqtqwhvv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gljoliuvl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/guhgejznw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gvxaumlyy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/giyelwems.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gamibtuaq.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/glhturafo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gdnbwrykg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gzfgkricj.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gxgciktsr.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gkprjjisz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gsocuzvuu.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gkdkuhgai.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gpedkfztn.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gtdqvfkis.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gbtyhplof.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gdkstauav.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gjsptacqy.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/garpaners.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/giedhyhfi.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gvtnsjxbu.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gszuzskah.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gvwyiadlf.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gnbtrodbo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gbdbpnolx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gyshupjfu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbpchgznz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gzsmrioeo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/glpvzdups.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gheicvoyf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbltbocrv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gvljmcjhw.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/grxewqapm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gotelefiu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/glutvfpmx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gzegmevyo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gjjptwwki.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtrxbozy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gpubhvtwe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/geszhtwct.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/glooedfvc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goczlwjsl.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gqiiaoyaj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbtdpkuhu.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/geynwuykj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gvctfxygv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gzvjxymyl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gocewyffj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/goqrkvtvz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gqdsmctuz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gyukvqaoq.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxwewhfyd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxavakjmm.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gbcqqlweu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/grxltyfmt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gnfgkiyjh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gayjccbqq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gqxgnwvfg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gxqmkrgzx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gkbvxywzn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gcslyaavw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gbgwmifhk.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gdbrkpmhv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gdqjqddcf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gcrpyrrmb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gquybqkut.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gxvbiijct.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gzrgwmuld.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gutvvkayp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gktedjerj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/grcjrdcwi.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gwnsqmhnd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ggrhjqdxf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/ghwppstop.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/ghxtxkvmq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/guhczcqhy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/ghtvcmywh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gczbnknzr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gclhkhdzn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gxynqpmob.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gnyvrshvb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/ghmheqqag.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gdpoxzugg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdzafyrzb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqpsnwfgn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gwcdiqymx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gbzmhvian.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gylvhxsss.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjjvzojhb.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/guavpmtjl.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkkstlmty.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcoulonon.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxpewitig.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/geqfexvtr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gvgpgfvgu.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmikrrnfx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsislvwdz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpkrpmceg.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/ghectzvac.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gcfhecjdo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/grhsdpokm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gvflwmnqt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gftifpwjb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gjwlqyqso.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/grilssdoc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gnltqkhtn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gdiphygau.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gemzoevsu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gwvousqtx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/grrrvoidu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gfwlpasjb.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gdtwbbzor.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gfabyltxt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gpnmtlxqi.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gqtcckewf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjzuwpkjz.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gufaiqsbb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyfebbool.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gotqiitny.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gfzibldum.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gfoxckjht.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/ghmzxosqq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gnmfguvne.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfdoihlsi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/ggfjyhsdk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gxzvampzh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gooqjatns.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/ghuevboqn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gmpdqzmwp.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdzlzmxkd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gkdmwsqxw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbjzfmmky.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnyslsfdj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggmxizgzn.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/guvsuuwxu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/goptwllvf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/ggncimgtw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gawqcnidk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gtaauxkzj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gqurfzxfp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gbscbfmif.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbouyjlhc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gigiyjscv.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gkwozduwb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gyvjpbpsf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gkdzoxixp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gqvctjbbe.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gyzuzqwpr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gjpmykqnt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gymyalkhs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gocvcaues.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gaaoctdnv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyoymmkgg.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gglhgcojc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqaomqsvn.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gekhfrjpu.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gbpdosrmq.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/ganzwnjso.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/grnvflogr.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gznxuzbfu.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjwzeclwq.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gqnrxyvpm.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/guzyvupqi.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gwwznjelw.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gyrhdqtve.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gielylfbv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gahpslttg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gksupifie.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gjwybnwwd.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gyytijjtx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gmryhklqm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gzbmshbyd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gwemgzqrd.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gowdwoiyj.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gqagwuujt.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gisdshehs.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gqeeosifj.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gcadvivpn.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gupmbfbhn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gvcjxztrl.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gbsivlxdw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gvevgbhtz.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gljnhpxhx.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gegvlhjuh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gizxbnaru.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gernkqcii.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdgdaucfv.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/giicgviwf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ggupypkfw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gewddjjhz.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gzuebhyuk.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gckopaeyg.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gaowswgel.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpfirmvfi.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcfctspse.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gpyvxwqay.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gyzwcppyh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gbuittemu.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gfmyzzoct.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gjgwxgfkt.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gmhvzrrvt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gocdhmrgp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gmyqwhrqx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gusmtrbac.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/glgvjcyce.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gievdrfop.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/grddxkhyk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gwfzzcqfm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/ggwgqruif.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/grrvcknrm.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gorviluiv.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gtwlcaxij.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gfiuxcdqr.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gpjblyuij.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/glulwjkjy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gqomuadyk.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gvaldqmtn.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gnldaivus.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/ghubhhlxk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gshexamha.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gmgwahawa.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gvsxqrbto.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gwzxkwmdw.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gdeatavap.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gearvyuis.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/geyldddvj.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gaqupfedf.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gjyllapvy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gjuraukqd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gwklwgufr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gdbklbwjp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gmnldvejm.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/geujyxbis.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gtymbmzzl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gndgcmwth.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gcqmnsczz.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/guvzfgzck.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gjsrhewlv.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gmstusmor.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/giorvouvq.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gwlteypvr.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gaeisplda.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gdpkfkobo.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/giwlhymdk.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gmexidrfs.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gcwoxgfag.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gjklhbitp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gvqczaofq.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ggegonuwv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ghzvtiazg.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gyljdofbu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gcekiydaj.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/grqhnmrua.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gorljzrhg.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gzlgiwgii.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gnlstibty.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gyzzjqnvv.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjqvlohax.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gcckrorqp.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/grfgyxkcm.sHtML


<!-- 参考信息 -->