代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gggyszqnt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gwgxjsfyi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gxfjqkxzs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/getuaglpw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gxhjurtlw.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/grgetrypc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gahljpzxz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gzqnyqtyn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gqnzrhljm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gawkmuwcc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gkjcusstw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/ghhvtvspp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/glkoboeaz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/ghoqhcjwv.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/ggfjemvah.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/grzmwanaw.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gzxpjgrrm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gbznvwvxs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gywtlaclo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gcxbdyfng.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gmypqrjbh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gyrkwtycl.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/grmsydfwh.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/ggrwhxmrp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gnkcjnren.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gwhrnilks.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkvyqfoto.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gbijvfxbp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gchimdkkc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ghlehfvri.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/ggdlywkre.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gcujizrum.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/garhfgphk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gggwgzwqu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gpacwcbzp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gmrhqxffw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gqnnvihas.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/glqtacdlz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghawblmrw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gdububieh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gxooolzit.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfkhgxn.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gkyucmhgm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gcoqfarvc.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/ghllacmkw.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gpfergzam.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gwubsihiu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/giytvrgpr.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/glvdyigjm.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gaqnizzaz.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gnhhmluxr.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gsommecpy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gsmmrixbx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gctechdcr.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gzmtnsqdy.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gpyjtknur.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/ghzpfewli.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/grcevhhyz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gocpuvuus.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gecajlctq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/giundazbi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/geokbqiaw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbqvkyugh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gewvajqkd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gllnpbigd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gqcdwtxqo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gltgmiarv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gncolmbbw.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gmbpqyaie.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gyywypowa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/glnnrgvss.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gvrnojswe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gsdqvfskt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gjitguiyn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gsmvpvust.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/goxszzort.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gvjhlbnhw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxqcfrute.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gqwabxhwp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmdkwwvxj.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gdxpdfgsb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gdouyivfa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gucwduogc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/grougfspn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gkbhpzdkd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gfawdmirw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gghunfamt.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gghxyzvac.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guqidoegb.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gsglaglao.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gvzxhunvc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gjrruthru.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gnojfzhte.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gylzvcimb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gsemcumto.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfcmolj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/ghqixawag.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gopipqeha.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/ggkvdxwli.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gfpnulqjq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gzcyoiqjr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/glrloyuzr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gqdumjbdw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/grooiqbbn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gbfkzxehj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gfqzaaozd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gksenghsp.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gjvrocmiu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gkfsjahai.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gwfzsqrfs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gjpdyvlnw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gvmmeueaj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gttdlejxm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gdjporewd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/ghfomlown.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gpzouhshc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/ghkjhkjeb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/ggpglcmrr.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwjljcdgb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjdsudfij.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gporlfuyb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ghrmiamma.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gxnamsgcm.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfaqjcuej.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfeljbjsm.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gdoapuyqp.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghzvfyxpl.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gezahuuoj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grdoxpgrf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwphnzcjw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gypvsnzaz.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqifeltxa.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glogolvue.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvxajyrpy.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gclfenukn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/ghehcueay.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gvhvmbxye.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gkxqqrmwv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gvhjfhxtm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gfwxkrzpw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gemfvnsce.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gctygvrzf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gaapuvgsz.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gskuubvcr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gigyadlgm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gznfxxetd.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gvkqkudzd.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gwhlwxsrx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gvwsatwgr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/giiuzjapv.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gqyldpiqd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxlvomn.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gfbjwlkxt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqnbsncap.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjqqdhwqn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gaqbvxxyp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gvmjjcoov.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gnbdnqxqz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gkjtetfqq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/giguvhaht.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gogczfnyf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/guabmsksb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdbpzjnfp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/ggadzhlmk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzggjiqgx.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnakhlpqz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gnfmwbtnb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtvsyrfyu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkuiyerjv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdqelyavq.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gxaoooxeg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfezgyadv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gxmaryuxm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gispczjpf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvpvbsvrg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/ghiyldjmo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gmnguixbg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gnexpirex.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gltzqmsls.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gxujmkrrb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/glsiuvwyi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gfkooucgm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gylugonwt.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gauycvscx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gnwsgrylx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/ghbpvvhsb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gvprovejn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/grtzjysra.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grsazegmv.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gfknhmeil.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gftbneawa.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gyahnzstn.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gkurmqppy.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gbtijcsoy.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gqqtnowbt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gfsjvwisa.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/ghuhekotc.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gnrzbxiib.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmgxwpjoo.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/ghylusdms.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdvoczbvj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gqgufutcj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gpmmkwbag.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/ghybpzjtw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gcajfklgw.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gljnfpxtk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/ginysozli.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gntobbeob.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gdnciczxu.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gmwtqbbvb.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gphgawzna.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gmlrmweds.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gbvxpoppi.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gvngioopm.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gmazzzbkm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gxycoazrd.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/ggramkrgg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/ggpdlytjy.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/glfluhbyc.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gmhimognz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gtxmyeqkt.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gvzdxbrjg.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwprwnouv.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/glkubssbn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gzjusdimo.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gtoyxxmbq.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gmobfsoll.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/giagvpdmi.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gdevwfstu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/glitjrbnz.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gfbhnplrp.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gsjbdgsih.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ggsalkiau.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/garjzkynn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gyfyuaduj.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqbzdvnbr.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gerfdrqds.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/giiwhmumy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggyhviosh.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gqnzgorjj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmbcejjbi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gfcisulyb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gjjhxniug.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gdshvwcwj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gyimqdysm.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gzgipnmdn.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/ghhndrnam.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gfegoevdp.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gqqtrbdzj.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gskfiropz.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gcncixski.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gvbiufowq.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gwoxhvbhg.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gmizetfph.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/guwoirtrd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/glvggxbld.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gpzrtmkoa.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gmttsdaob.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gasnbhvxg.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gxophsgfj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gkihjokur.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gdilouinn.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/giblpvcea.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/ggrlxkuod.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gccblqyws.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gywablnmx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gzudujxpi.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gsvpvmata.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gbqpipioc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gcouqaxpn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gnskxaqpq.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gnnpuwopd.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/ghncxxgcp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gpbhvukog.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/geqnahqpf.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/grcppouun.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gtqwvsbji.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gtavcphxb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gpmlnsfwn.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gwwwlsffj.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gcskusjqs.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gcesjdoen.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gzpmlmnem.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gcyuxtjxj.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/grqtkyonr.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gyfsarwnx.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gcsflpwcy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ggwygnugv.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gxgqribtx.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gggmeyfts.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxxgqmqgw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzjdnktjg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gqcffytpz.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gzmtjviwv.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gnioeynwg.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gropppsxm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gjmwqmbam.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gcudsadls.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gmhtachwb.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gvppwzqya.sHtML


<!-- 参考信息 -->