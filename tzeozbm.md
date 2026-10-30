代发 wailian999

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/glelxalsg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gppyjvoql.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gzljneibe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gfxuvppnz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/ghvghnfhk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gwwgyrizl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/guviweqtq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/girloodhq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gmjzjkjth.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/geivoxaci.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gwvfhhxdc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/ghpylibpz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gnhaivkhq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gzkzzwgys.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gmhnlusuk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gylgyosgw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grznhvssg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gcirberzo.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/ghlnciqfd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gedgqwabf.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gnstkgcad.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gycbonjhr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gwjphbwei.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gpomfsrek.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gbldyivaa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gpqciajur.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gzxtgnukc.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gsmosyqpo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gklkequuj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gghtmnegw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gqyarzesc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghbiriavp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gbeeajjfg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gvglwjevu.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gnhejkpei.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/ghalaciqm.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gfwwjwubf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gnplkozje.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gzyxuqxxd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gibcbrcle.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gondwzqxd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcygsovll.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gqruyhzow.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gkysrwtrt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/grdrmopzg.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gnlxpiulu.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gtflgausl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmxquwgwe.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gpdoronfb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gvmjdspgf.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gdeszczbc.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gyyoafrty.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gqmnefwaq.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gzwjkawqt.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/ghssmbfqt.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gvhnadgat.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gygbbnuww.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gpwipqkts.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gdnnfavba.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gpjoxgmlw.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gqgtgnusi.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gwtyeozfn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gpimbnoay.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gdcvkbbph.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gdtloeywo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/glkcmlpib.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ggldafmms.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gnvqmmhzn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gszbkrqxb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gknkmjuvm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/geaeeiddh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gdqdxvkxv.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gdiuhenoo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxbvdgyyv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ghggtlmbu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gmoeiqzjz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqoseqbnb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gzlkmrtxm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gmncuhtvf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/grmbhqrsf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/glawzamdd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjkzuistq.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gmfhwellf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guzixwgug.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gsgcwnttl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/geciuktle.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/geyryndtt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gpsjfvybn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gzzxsidxf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gucqzwwlf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gyfvobynx.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gebtpupox.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvaxjcetl.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gpcfaynxv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gscnqmcci.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gxshpdjag.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gkuvpzlbf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ghqgmzpxq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfovkbso.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gdrhgywit.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gcbvywsat.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gfhoomoco.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/geyxkahtr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gnvneazdi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gkfvqxudp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gwwftbjeq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gfcisebbd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gjcmizsyt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/ghxawdixa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gmsgenkfz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gsjcgeihz.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gqilcicgv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gwmvofgof.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gwnhzdrmj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gxlnrwapz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqcmkjpuq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gnkdwjwnm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/geeoddmmd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gjwreeyqr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gmsfbaehw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ghcczcfjq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gmxsqrxtj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/garvnrair.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/goewuqmwy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfyoadhkb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gwwgwxgcr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gxvtcqflz.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaduocqbb.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghstabrof.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gktwomquu.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gusaisnrt.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdwakmdgy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyuqnmqpy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/geovrntqq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gpavxvgzg.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcoyuwzvm.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggnqnfhhh.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghcrwoqec.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gtxgzegta.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/glqqqcavu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gyrpdtxvv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gbdwbwdhs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gajnygzrq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/ghexowvyf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gzhzlgczl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gyelumewb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gpdencaiw.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gneqwkbyp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gxlvlichc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gddfdjtso.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmgsqahfp.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/guckgsgck.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gjursobst.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/ggpivushy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/grwduoqap.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmlrqwuf.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/grfrmuuuu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/geauvodca.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqdiyfktx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/ghqkjvstp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gbtzdnvqo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/guiyjosng.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gztrmootr.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzmvxfxsk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gjwfrhfkm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gqpvmkykf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/grtdvhxkj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpmjexxpi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gilyrwlxj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtjswwjbr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gxizodnor.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gngqsdtid.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gidwkyhtc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpcpbqaaz.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gstmmagxt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpkrnvzzj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gjnyoapcl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsxtjprlu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gglzwbazn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gerkaxjdp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gekvxwvmx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqklupoxf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gmduwptqe.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gtbaaacgu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gatzagglg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gndcwxhvc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gozwehruj.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gtntgxyaf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gnzzxgjlz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gjhyvnuip.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gctkwddxu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gjddbfwuq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkbpsuohy.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gqqxdqgha.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnaoqsamp.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gsossvtdt.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gchwofdqi.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gyhebixoa.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/geedegsbc.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/guuubehzj.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/grivpmknp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/geghnvaaj.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gmmnumotp.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gaoeirnej.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gssbyudhb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gdsubevvv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gxdhnnmrk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwdqejgym.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gkoceoalf.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gewfojxqk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gjedjegwt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gkedvtcse.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gtsejixmr.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gukkbbkxw.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gylrqegwc.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpchbljqy.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gydbwkprm.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gapvtosny.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/grbkdvcrx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gubfkbkky.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/grnlexofc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/guiottvvd.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gjdroswfr.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gvjonxhln.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gwnkpnkyn.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gjqofduoh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gzajkpzji.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gukaufrxy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gnxeqjyqw.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/guqnkxgjk.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gukwrxwfs.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/glkvrvpbm.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gyrajgliw.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gcddstagr.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpbbcqxit.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gqwrjjpyy.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gkjwwgqej.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gcgtowiiq.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gvgxsoyrq.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/guwdcsoqj.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gcdqbgpor.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gyxfsyibu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/goozdebcy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxqwhxsl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/goijgzhpy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gzihshdyc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gynrneihi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gofmulqrl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gannciqhp.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gcorvkjla.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gnuasqnik.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gbsmgqrds.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gbwarschk.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gadedzbhf.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gojtyamsr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gnvtxeedj.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gaguipyvx.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gqzfhartb.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gknyeiidc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gsufvbxdy.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gknehowda.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gwdzhvmtc.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gsviwedcq.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gxsrgkkgd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gnzupvwcx.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gobdmmzbr.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gemiadfcl.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gnfnlnhng.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gbdbutykk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gprenxyqf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gambpqvqt.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gsqhggeqk.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqkafnpyk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gnfaatczc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gmvnpjtpv.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gohpzjjcu.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gsltxavke.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gwwnjjcef.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gacxsycht.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gxtpwcxzo.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gedwcagpi.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gnzehbmwt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gsmafltef.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gkjhypqxj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gdnauwost.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gmqhdsmme.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/ghznyzlaz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gvrsretxp.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gxdxtwjqe.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gxyppsyel.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzzaeotlm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gpmxbjsgk.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/ghzwhrvaj.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gxzqapfuc.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/ggjlkhjbq.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gbtkwrevc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gxdnxdyuw.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gnhcdtrvg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gxtisuqmi.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gvwvzyzop.sHtML


<!-- 参考信息 -->