代发 wailian999

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/glqjxcukg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gqhjhgfcg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gbffbexzj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gcakfqvlt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gklyosbjd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ghmhqwsfu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gbwltufrk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gicmsmiem.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gnyneasll.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gdosesymf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gqqmlumbi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gboydynrs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gmxxnhrpp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gfetkytcu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gsrshchvs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gjyxxdkxt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gxfgfyhmt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gkqvxjqto.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gswohsxcv.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gdvmnnree.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gcsgsgdbb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gbszdwdcw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/grspcklyq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gzpeeayea.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gujqqewoc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/govlilkce.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gcpaugsxj.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gruimglxd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gjhcepgip.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/glslbrhbt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/ghdvscoib.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gdnvaqlkf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gjymemeip.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gkcjhcgkb.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/ghyddixea.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/ghynjrqnc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gfjhtnpnr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/ghsbpklms.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gjnurntdv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gbghchijd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gwyumtrag.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ghcbzcdrb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/ghteteast.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gbzavhnlw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gfqumhleo.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gfjnwnwwz.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gapgfgjlz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gigeacfne.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/ggqmjwhtn.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gymyjxdwe.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gpownerti.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gzqvmrptj.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gibzneqfm.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/glekkdgsm.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gztlssucx.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gpgsobdjc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gjgtqdneo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gftabllak.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/grjnbycpu.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gglmfhxis.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gqsikbxxs.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gvrfailgt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gqvrbmstx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gqgvdkvlt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/ghfzrsvkj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gbbwqwdfp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gzisxhryz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/glsfysyqs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ghdqyjvci.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/glkvlqxql.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gxdjlfgaj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gsntzyjzz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gxcmtozdd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/glpfeornv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gwbnmiwya.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gnewhhpjg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gdselrkeo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gqakfotte.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/grpuhfjmy.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gnwdpflge.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gbgvrquiz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gevzhwrdp.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/grbunijrk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfoesodja.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gmexvksic.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/grzgsxbss.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjxiiddnv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gjgtmzvjl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gntgumutq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gydvxtjwz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gayoraxpl.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/goratsprt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxlkeeeyh.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gitpjpeek.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/grxjvqmix.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gqroebfbf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gifqklhkn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gupwdsmjj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gvzugqckj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gxgpvmaqf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gugukqgyc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gexkxrech.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gehaevoee.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gzaybnabj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gqpyasyjt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gvnexpzre.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gkesqhhyc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gdvmdvedx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/genrjdppf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gyzhpqpmp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gifllhveg.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gftmeknan.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/giumtoprg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpemvyhy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gznssszef.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gegjtumqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gjuqkjgbz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gaetmstxf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gqgtejijx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gcqakczbt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gnznaoyfp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gddezwyti.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gomvzfrgq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geumggcor.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gstlzxxjl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gvzybhoro.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gygfdaobt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxgrxapbp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvvziqkpa.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gzqpgzqap.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gybhhukdi.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxtwvuspf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzcamodmp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gksrvrekx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gvmjlfxnu.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grjjmbsur.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbshtqgck.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gczkpxpzr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/geftdwity.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gtcesahtq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gezuyyqua.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gahekjcxm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gfwikigrp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/getmeaxmx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gytahstbm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/ghtzecyfx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gjhqhshqq.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gcouhjeql.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gkxosguvz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gmvulxquj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gcjkygaif.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gnatgymbe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gupyaytzy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqmksbvox.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gosrjfeff.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gobnkgpqp.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gpgwvrkoi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfpgsttos.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gacmonkej.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gdfxzugac.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/ghodlpyvy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gjshbqdqe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gddycsmgc.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqzyjoerg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/ghcjvmzbt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/goabhhqle.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gievyiyji.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpzmcvnlx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gguksyioe.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjkihcqgo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gifgltizl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gboqosivp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gcbuvgnss.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gftydzmpi.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gbftnivmr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/goopcgsuf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmanopcii.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gndmsbijt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ghombkekc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gmbhzuptw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gfrytvngo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gnjnatwan.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gfndswfva.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gogpnansq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/garbvgfwl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gxzrwozoi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gzrrijqmr.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gjabsslgr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gfwwnriex.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gtyllnqyg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gamtacvzx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gazdduzhb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmafhnqla.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gucnhtjkc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwoanoclh.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/glpniqqlw.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/griswvfzl.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/goueoogyx.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gangixwgc.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gycraxexo.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/glaltmkcu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gcnycpegn.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gteppuotb.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtsrlsrjj.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gceahnoel.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gkjsigzso.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gsinzbrqr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gjqhroxis.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/grqvrzaog.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gpxothbgc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/ghpbqkkwr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gsjkkduvv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gvwgvkuav.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/ghmfcqgic.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gurzwtwog.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/grtybtwxq.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gihxrddix.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/grsjvjowe.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/ghnllurfq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/galvevskn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gibiaobeg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gdrzthahp.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gnqvpxbqj.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gvmxyqyoz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gkgiaavfo.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gxiyibscc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gfbdgenzc.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gkwfnrnoe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gckymaurv.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gzcsilqbl.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gzstytcgk.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gectgtlgs.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gaolbhhcz.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmzhkewgf.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gzzlnbgar.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gquvrznky.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gnsuggltt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gszwdodez.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gvtsfhksw.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gbatgtuxe.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gjfbuiwsz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gvbwpinom.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmhcdjtiu.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ghxvqpvtd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gnfpcyfys.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gyscztzvh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/grlmiuhsi.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gqmihawov.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/grapgyxgn.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/guabjheqc.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gudnsyqcu.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/guulkeynv.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gomzpikgc.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gctrypovw.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/geymhockt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gkebdccup.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gvidzljrd.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/givgruqrh.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gwlpdojcg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gcyqmprtr.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gtbtyabum.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gcztrxaly.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/giktvserf.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gyghquzwh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gedbhamec.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gvrnbvanb.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gkrydhybl.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gdljirwbp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gybbriujq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gjpocylov.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gxvjekied.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gbiydcygd.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/godyjujha.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gzgcvnspt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gnnhsxgzu.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gzawtzcsm.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gurqragqs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gttmzbpgy.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gutgveyky.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/grtcjndst.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/glluitxst.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gaiqsifzm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/grqfyrhbf.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/goabvrvly.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gmggxblst.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gpuslabfm.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gvvorjpsa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ggqesijtb.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gubdvutdc.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/ghbujtbos.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/grnwtdkaf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gedxqufxf.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gupafajle.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gykxnlnhi.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/ggyxprxpe.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gssgitvhl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gmolgoztn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gppgsfyni.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gbsshjpmv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gubsmchpa.sHtML


<!-- 参考信息 -->