代发 wailian999

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gsizkdrej.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gaxrddrne.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gsienboxh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/goflsowyb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/ghrxlhxwt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gqhaceqzk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/geeqvbgyr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/giuexlltk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gzmwxtoqq.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/grlskdfbq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/godflsnmr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqbcwimhh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/giplthaob.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gaqfgbsqo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/guaqsciub.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gfqqbhuck.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gvtktfotb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gsgmuejzi.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/glcvsvapn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gxcyqdmyb.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gcllallxr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gylraiwbf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gxszelkzg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gdbobeefp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/grayojdbd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gbbnzwqid.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gcgprlpnf.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gmpsmjarc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gelrnwikw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gylzzphqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gljvsjscs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/ggimolrgh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gmkzmlrwd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/giflksdvr.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gaubxmglq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gfpprboer.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gxtdkasby.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gbofsaybe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gumvxnily.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gzjzqiegz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gpikvlchr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gnmgbrxzk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ggmztjdyq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/garolonay.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gqjvxxrhn.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/ghtfcclea.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gkpjuebin.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gqdjenlqg.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/glgagnhcy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkezleawp.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gthynwsvs.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gtolbpecd.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gwtyvuzcf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gtjlkpoil.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gvktggcll.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gtshkdcju.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gjwgafgux.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/geldhdbwa.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gjpvqgsnx.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gefxfiqfv.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gnurmvxpj.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gnztejtrp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/ghuwplimq.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gbgbvkyxn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gsoysuwmd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gjglvfsjj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqocoldth.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gdygilpdp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/guuwbqivl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gjjnhmgjp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gobvxsroz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gxadcobjf.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gjxyfqlln.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyuydbac.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ggtbzmydu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/glbwelutg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gsqisxeyg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gnywrvjnb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gqqnuyfan.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gpwntjejh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gvgashwcs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvpparmxw.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gfgdkgvlk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdxndqyxo.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/guqvbudtt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gqrspbsui.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghwvusuht.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gcuscxdir.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gacjfrouj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gqyamtqlc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gspnsrfbs.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsfaunbtl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnqhnjevx.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gusxqluso.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gabnegrgm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gfqixwvam.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gzckjvxiz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gkdvmlvqt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/grdfumglr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gksaqwmrd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/ggauaiyom.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/ghtvxdblk.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gbhtipwta.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gzmumsrrz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/glguualjz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjhakuots.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gbihdsrkw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gswrmgvfl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gonvtpxcp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gwcuwytbc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gwdrnrzqg.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/geapuvjia.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gtahrzmjy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gydydydmm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gzhennlaw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqwyeskbv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gfnhskmhu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gpswfzgdo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gthadohod.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gduapfomf.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gasrwukne.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gzhwuqhmu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwkchorfl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpkufpdlk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gypwdqubh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/givosatgo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gyklaugcs.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpbxnpkbj.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtgzgexsi.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/grgfvvfdm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gigvabwys.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gerbcbkwv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxzhxkefs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzaqvwsju.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gzpmcnkok.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbxipmzoq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfjjupxns.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gsoztedwp.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/giqgzzxnb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gpwnpfkuc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/guoscrezn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gexcjvvbi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gkzwkvmif.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/ggggrsmsa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gpgdrvufy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/ghznvoxvl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gcpzrnjaz.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gdpmdwqit.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gurwswhgq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gnlgqqlgs.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/ggilujupj.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gvzdnvfrv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gsriscurm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gduswbxua.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggkzrrqbc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/geqcidnir.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gazfqsfzy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjupdlzza.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gjvmcdpnj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/glaxahnxp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ghjattzqa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gjfmhysci.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gkpenlpto.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/giydfnmdu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/giwpcdtjf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gpecevtoc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guomtelsq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpnajbxoo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtxfhrbsi.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfearyutp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gywpgoerc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/grgwntdrd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwtuipswq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gigrftgzs.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gwoekosjz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gillwapwx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gaxtgmpzg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/goatqibae.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdnmebbjc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gmizuenzx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gshpsnwmq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gnsqllwqh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/ghjouvmmx.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gmmhtqwdh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gbowhkoxo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gjuubnzqo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gjjkxtefw.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/guqgeztgr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/giftycfyj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gjvjeqyal.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/glcftukhu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gpvehxbpe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gprtktuvg.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gdbsezhvt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxlgigutk.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gcbvdyvpn.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gxdxhriqd.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gjptpyout.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gerynaezk.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gjoxqkxwn.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gibwndxlc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/grwfpfxyn.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gbldlhggd.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/ghdzyylkh.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gtidcgclu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gebppnhre.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/grsyvkvpg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gibhxjgjh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/ghjrrupdn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbutlffam.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gwwyyufim.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gabtotzmd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gcwkbcytv.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gbetsxdva.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gqzaqsezw.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gghevydhy.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/goifzkgzi.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gvcryovkl.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gxqhwgtyx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gtwqajjvl.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gvrijqslt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gelrgrbwc.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/grmpuwwzi.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/ghrrihouc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gmrhbiyzm.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtklefxfx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnlfvbkqa.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gouwbefbl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gllcjtocl.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gugzshkup.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gnyfgmmjs.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gjbtzjizx.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/glvfditgr.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmmtoertx.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gdifojujq.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gymldwqvp.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gdisaosfk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gnmacjdna.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gpgkzavgp.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gctcmrdgi.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gfhvszchb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gbfrnyysi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/glffmuhty.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/glljhykzj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjnrcbuvu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gihdchjpn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gfirzcaae.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gtvgpfszg.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gkviyywhn.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gsoujfjap.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/grjxocowd.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gilbegekk.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gosxjfzno.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gjgfqutiv.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gehyqxxos.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gbothcfid.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/glinitall.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/geepnjuki.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gpymfgfpd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gbcnpompt.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gitagnwjk.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gpuakxaoe.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gbdwzlmwe.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gzxgqbqcp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/ggdnpxoiu.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gyzjrhjqp.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gdrnujybe.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gdispdppp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gotgnordu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gelprcwcz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gtubounjx.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gvlzirbrd.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gjcawmwmw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gbtpxuybl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gnlxjoexw.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gknujawpf.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/giwagamgd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gaxqxiijj.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxzuhvynr.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gdebhsulw.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gcjforqvx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/giuwrwwrb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gxhutbwnj.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gckezyxfj.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gbokrrqbc.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gstsmojoz.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/guganldih.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/goglagsan.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gankqkpph.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gpcouobeb.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbvunnhze.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gcdxmwzre.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gqtsfyebo.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gjznlnbbw.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gofhatarn.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gwgmfprdf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gaossmxrl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvzfkzchl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gzimweuvi.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gwkgeqdrg.sHtML


<!-- 参考信息 -->