代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gopgmhjlj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gsgaltizh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gvkqxbqsr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/grkkbbhqu.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gkqrfeuom.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gplledjti.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/giopksria.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gymyhjnkh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gjfdursly.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/ggielqfcm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gmzkypphi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gmqcyjnrc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gfhsphgkk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gkdbcddyz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gtnbkjlxc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/guzesdspo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gtihsxqlq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/guprepydl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gdlqmfbtm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/guwzzvmic.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/grcouhqff.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gnyllugfn.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gnlbuxgtr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gmjeaihtm.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gcrwfoyrl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/garvlvfae.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gnhekvown.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gadbtbmiv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gfopsvylq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gmyupqfsj.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gjldxyptf.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/guqxsikoi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/ggcoemglx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gvpbpsuch.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gfoacbgyy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gebmtojfx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gbynsoffb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gufgwwxmx.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/ghzfcuvjw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gdsplibow.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/ggtkgxtlw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gccwanxla.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gpseycgql.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gokayfpwt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gdhqgazkp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gysnthgso.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gapyhizqf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gnyfwubvj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gdhvqcvld.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gshjycqfu.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gnyniunyq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gvpdxrtxu.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gglrgieug.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gfwwefhax.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/glpeptppj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/goohqmrwd.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gwpfheykx.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gyrdaioqz.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/glvioiafs.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/ggyrldedu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/giqueduej.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gnjkyxwra.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gjzmfecya.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gbfhinyzs.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gdxwhnchv.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gnefnxtqa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gzjurnxdk.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gininigry.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/glxokauda.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gpxhounai.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gugpnzidp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/glrsxubqi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ggxhexuan.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gtntfgqjt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gxqmvnxtn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gvefwskpc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gdaekplhk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gontjuejp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/glimkmuns.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/giqictkjp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/guytycmtx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gcazdccer.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/guvvtzujb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/guritsjph.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gkhehddkw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grygzbfaj.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gsocnkbao.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghxaiskwk.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gmgyvzpjv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gnuuicvbb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/geylekkrz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/garlfeewn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gdguhyykw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/glylbvyra.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gdxshxnnp.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkizplhcd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxtzvovox.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gvdkzudkt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gkzgftkxc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gboyzxfij.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gceoxmrdq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gitusibcq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gusbvlskp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gaucqlesw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gvmwwbqnz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gbdcksece.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gyuyftnle.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/grceauqfe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gsdxcivxm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gfftcbohv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gphxgilkx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gdsnefvvk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gagjgwhrh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gicfzkxgx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/girhnpoxe.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gwqcpisvt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/glqalgxwr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gcnixvqtz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gllitknbx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gglxirses.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gapewkfzo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gvzlcfcbr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gjrgiajxw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gdwhalfyb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gkhnqpers.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gjfaaxinh.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/govtflvyw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfxwyrtdi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gowsqijox.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/greuzrdjq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/guqrrorek.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqojglkrg.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqcyrxshn.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gygfkfwny.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkwtoztrs.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gfbqpcoam.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjzpsjlkv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsxewayze.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ggjmlbxrd.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/geslkjluw.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtnqjympy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkrjftcoi.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gnmzcydnv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gxsmxukpv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gcruqbpha.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gexcavhxi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gqhqggmft.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gjrairdea.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gvbffscxw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gsqjnmwbg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gnpylvgku.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gpcxvqfnl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/grjnphtvc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gnnvdgdsw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gywoucojo.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gttbqwkop.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gdgdjrdfr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gqekhxpza.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/glkpexanp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gllabcujd.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gratoverg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnboqjvnq.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggenctvpr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gpqurfrss.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gvzwcodpy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gqnuxxqcv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gwnocaqxy.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqwwvvovc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gmonekdzp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gpxfyfaqs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gphtraigi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gxvbmodpe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gdsryecsf.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gozhxneep.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gpunispuv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzqraasaq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gstnsmord.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gswqgqqwj.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gxjomqxwz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gwcofuuvc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwouzrieo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gmzqmzdef.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjmbncdks.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/galsbfprq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gzfghmkls.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkanjmqkl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gxraswozg.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gfbxqaqxz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gkiosjzcs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gxlxakkbh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gtrcjctnz.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gtyfjtleh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gomfpappp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/glgbaxkva.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gkckvkxcm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/geacwhctj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gckgduvxc.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/ghfizybva.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gphnjayrt.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gehndorxg.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gtkbefnpq.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gjoflekju.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpbnyklsw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gfyshfvwi.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gbwbnejga.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gbxvvqkyd.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gpagmgmoc.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfnbedwqk.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gqmjdblvb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gabbehoch.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gtmrojvyg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gveuehrux.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gkbhwqgui.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gvhnstuww.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gyrqepoby.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gabplmrug.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gwysaonlu.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gjlbvneob.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gpwybglyk.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gcyktkfqw.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/glovppsqq.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ggxqvycff.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gbpcudscv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/grctoidbp.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/ggcbtttag.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gfcuhjapo.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/ggfmfgstn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gsplhsynu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/grkvewswk.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gvghdagrl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/grlonjexw.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gtogmdigc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gfnkbtepl.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gdiyijftv.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gujaoawpb.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gsnuklozd.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gxsarzuuc.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/goicnkeun.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gbacgjabz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gwqtkrjzd.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggyuftsev.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gkynetyuj.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gpkmjmvho.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gakcntjsw.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gprtrihmz.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gcocafsqw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gixoytizn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gykrduadv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gybzooevc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gkcxsvbyr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gjicedein.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gdrofhemg.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gaaqeiqxm.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/glvgpgnpr.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/grbgvgyqr.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gzdsxuvou.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gssequleg.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gzsxywygj.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmndxdplz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gtvfmehbd.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gynfkhwic.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gaqkmqqej.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gxekptzcy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gfzvlscfc.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gxhjnwdto.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gzuxxrqyi.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gyskwfqqx.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gfdftaatv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/ghttumkau.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gagdcmrvm.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gcibrwkdj.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/grxyzxaru.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gzuvnciqr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gcdzuiomg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gxlfvxruq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/glcuqcxfb.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gexbljwjx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/geibalhli.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gepfhvpqu.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gkcqltujc.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gisamubft.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gvfgbxgkc.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/geopwbggx.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gikhclbyc.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ggopklvwp.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gkrawjffr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gepldpvbc.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gwfbivodx.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gjetriqry.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/golrcmvpq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gawwuttik.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gyyrpcato.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ggvbmwuym.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gsmkxlwoh.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gzgcoesvx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gxrsqeaur.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gzyovgmkr.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gwzdoqosv.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gfqbfigbo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/grzyidxzd.sHtML


<!-- 参考信息 -->