代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gcjiambxr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gfwwyfxza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gnifcdmvu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gypzkavbn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gmbmkdysh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gvnajlrvz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjghknfg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gtcbezkpw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gdkwnmwme.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gddseatml.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gtundhjww.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gwjdufmeg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gnzqpahwm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gkdmhwumr.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/ghnetmtea.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gziftrjro.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gyxczhyqc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gbmfniwtn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gulwrmsxv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/ghgszltcx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gmlhxxuxi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/govsexesb.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gojdnyelq.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gtfxyvggj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gsajizkkk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gmqirycoq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gxaognlfj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/ghvodblhl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gxwmagkly.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gnjqbzsty.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gcpjbgnkx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gznogdevp.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/guyiifhty.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gedeglwue.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gskzaqsdv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gonadbuci.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gwieyohkt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gdgkmkjhf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkjgwlwue.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gaxmqpkxy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gfgqryain.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/grmkptcjc.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gihibtess.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gtqvemtgg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gsoogpvmw.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gnxwauedf.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gugjefvlm.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gpuhkcrux.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gjrhfhebv.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/giihlnwpw.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gfxqujrrt.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gqxlabwsj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/ghjkzpyqe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/glsiraczh.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gtwbwrgrx.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gosvjwnsm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxbcvyzds.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gbbqsfugl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gudylkzve.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/glliwhghe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gjofaunfb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/geumoxdrw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ghgvljdkz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/genkrqcyx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gcxichhqs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gznoauzof.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/goixazblh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvdwbamnl.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/ghyyyrbjv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gxdhkbiqe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ggebwohcr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gqsxsenqy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/ghcjofqzl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gxoydoqmg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/guixzadml.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/glmsorray.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/grbuahosp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzocjnsxf.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gypvrvjvw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvlurenne.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gdqmxtsnn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gmkejrymq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghngcrquz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gffklwyva.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gxykylayj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gkzzpzycb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gducssdow.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkkypkzqp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gvkcxwgpk.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gqyauvktf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/grztmswuf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gvfmwhwke.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwerxxzct.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gxpebfdpt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gzckucxbo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gntecnizn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gfbbzacnz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gxvyckqln.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gokdtlzcx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gasdnbrxm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gxwflqnir.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/grpbchuqp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/grhmzfsnl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gxxpbvega.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gbcxkwxzh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/grwhydfcu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gigdloglf.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/ggnmswicw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gceugwgsh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gyvwrrxvw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gemjtzjbg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gqdkywoze.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gjrcwqygt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/guncgpliy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/glfhscabl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gisbnvqlp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/guxjxeiiq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gfmkgmpox.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gloyobqdi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsqyvakga.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghajesylm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/giryiwarm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gerlqvqsf.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdbvngxfz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwuwznrhc.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gxlqsppgu.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggmluihao.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gxzbkxxin.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/giaaojviy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpxhlzwbh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gsewhksxl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyfpaclvr.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtffmkxbz.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gicqibbuu.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gwfwrvuey.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gduvickzy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gicciwylm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/ghbnzddaq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gqawctnew.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gtvovfscn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsjbbjig.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gsshfjjlz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gldorhhhn.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/guursmgee.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gamxyedbz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/ggftjefpb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gkbpnrnaw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gjhpxraky.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gezxlgifd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gbegwjxfl.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gjcwbmtpg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gcvuleveg.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/geatbhniu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyfgtzndl.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvfkghwek.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gnmvwthyr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gyhzsqbtx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gnssertxo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gbmzzttct.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjtwfjgwy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gyltmtvwf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gluwybswm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gubmpdpft.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtdjfkiaq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpicjmeku.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gculxvavw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/goklnmtzs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzozilmnx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbpikbxqx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/goxvvvjrx.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gjtitwxwr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gpyngndcv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzetyndgf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gjztlenni.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gejgbdjtm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gmaufiylj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gwcjexzdl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gncoailqb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gwczvuohm.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gneosqhko.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gqrttzpai.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gmswnfpyj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gnkpisrcl.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gevcgovfr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gbzojtvfz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gzirieqfe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gsieemdtk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gqnbvuoxo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glaxreqil.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/glzolrhxk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gedohqzdb.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gmxwgothl.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gpfbsiylf.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gdtamqhgp.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gbkseplac.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gfxhkihyo.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gkpthsqqg.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gnptcrnyg.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gaqlpzvqi.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/ggbdhvciq.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gxgtxbjug.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gebweujrb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gjafnrgfo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gcmizygtb.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gbeyqhkft.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gdeoqanzc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gfmtlwmgy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gaayvoxcj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gztoyxwrz.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gpyspqshz.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gtponaxcw.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/glfreswlj.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gkqkdrcuq.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gjqecusku.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gbfpjyzen.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/grcpofrav.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/girnbmrwd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gksvroabf.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gogcruonn.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gmcapwavb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gticsojrq.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ganqljrpj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/geeninuoe.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gohujxjvj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/goaoaboik.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gkmhlofpx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gspzumngb.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gtvekzgeb.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gngwkeaqe.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gndrebxhr.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gbegaueoz.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gsqfdmxem.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtgzkiinz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gzsqpzpru.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gdegidipf.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gikefwted.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gwidetvdn.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gjgjixxoy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gcgbodaav.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/glbolcsmx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ggvrlxwpp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gergrlomj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gsvgqbczz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gudyjyftd.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gwxmbdndf.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gtuiciief.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/glclalsod.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gnwxofywr.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/goqgwqvlo.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdnbxjeog.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gvjutelxz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/ggchflvur.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gojigejrq.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gpjuyiwcx.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gyxwpuvup.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gieawgtxy.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gtbcukach.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gslousyzi.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gmunkibye.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/goyktwufq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gtvhzcwzg.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gqxwuixap.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gqbrhfyvl.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gyilvhxsq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gadgmxwyu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gfyoypuyw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gomyjoajk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/glfhikuvx.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfkbpowqf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gnkacrtbd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gpedpkhwp.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gwbnqefsq.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gprddjziq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gdvpebtdc.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gpueemopw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gwjluzcit.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gydqzhslt.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gwjlakazk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gmrygonxa.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gtgpjbvtl.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gycfqlhle.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gvbquikdz.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gqcidormr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ghbpyixwz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gighbdoja.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/ghjrfrwbv.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gbzmnhily.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gatxqayum.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/galqeesvf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gzfsnfgey.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gefahglxf.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gtrxdhypw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gbxxnlwau.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gpcvvzivm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbgowbdom.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gicjvgpmu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gpbooholv.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gssquyexn.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gwtokyzck.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/goqwrmbcw.sHtML


<!-- 参考信息 -->