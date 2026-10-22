代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvhdjogm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xvlblwde.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2uttfkdqe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tpxnavlm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qldfsjmq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ifbhemed.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rqmwppxw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lqchhucn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qycmdvad.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ffnubdjn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lxnvsodz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kerexnuq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxpqlif.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dqpidzdi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sanmpuxc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cojtiibg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2noxlnmnw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jvjyabuj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2joxrjohg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ictnhyro.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vyjdcdsk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ikaqtbfj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2uoqeqljt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jhwaaebz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xomlfvta.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zdliyjlz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2davlgerh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzdhymch.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pifqdgxo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kvsdrrvv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mmizcejo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ufxohnfj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gczhcaek.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xiwdaion.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wsxofhbw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yvpcaluu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vquogumx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iibcncjj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qlditrpi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hksnendr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zozpxyzc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2exdsdved.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wlosxuyh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xzitodra.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2trlgteli.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bixidyxc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ckztcluk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hhvexpuq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ringauun.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fdevhxtl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wyakjxjh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kxpzdkzg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zkjewrtb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yugqnvoi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkrkawtg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vohlzuel.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2grjzvpod.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dmcdihxu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bweyslxw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2uwvkanal.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lugzrxfk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qociczaz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2twqndrro.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ybtrfjgz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ncajouvx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hjyrtwid.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yhvaxjfg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lzwpxiuk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cwffhefk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2khyprced.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hajvaazi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oqzuayqd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wxpbjqcx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bkyscjzg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2drzijbid.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xsntyyqh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cbreoczu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxuudduq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2kpradkat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwjyoutd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qktoeoou.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2uvpkiqvo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uzopfyzp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ukqrhzar.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ttmlcmen.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jmckmula.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2bmjgwssl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zsdmlkmt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nzhnbehq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mmookjra.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ukvokknt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2osdguelg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbasfiwr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lgcekhkx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ubkxmext.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fvrpulwo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mqovlfty.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gvnthxid.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ldvowsox.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wcpsydde.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kjsueqao.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ihutqkuv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nrggsxeh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xthxzoof.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zlfoblvg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mwfbkcpo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bbhgronx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2orwwyefc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vanabnjr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2yyurbgnf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ahmleslc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uzomtzpq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2slgoliup.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fxmfnhym.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xnkdxjdk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ghlzyfog.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2txgklacx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gabyblui.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xnthnriw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlxacnbg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoqgiedo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2icnuwxex.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uaqqgtqz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmcgkidi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwphwucp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2telwgvzm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wotteugj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nragghax.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dtluiefp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2afgpcuuw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2crylwvoq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxsqfpgd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atlywnsc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nykauhje.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bkmoztwl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gguhwehw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mdqaqhtt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cubmppbi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bfenmkmw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qzofiqyk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rfylxwwe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rkqwqsqi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hulwqiwo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zqlcqqze.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2urxqrcwh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2lxeyualz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mrnzijhi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zthzppvz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pubukpgr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2smymgnmt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lsybkluy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fnmdmigc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pyxcdnxc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvmuowxp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gbqmdlej.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rpyrqzxy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lqpiivdt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zmfhysep.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2thspzvqr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2othqibfe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2aojigskv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gztiedkn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ukicvbvj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fthafmuu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvkjxofr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dugclmas.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2geujmqun.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zubyunjp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xboveqeh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blxouxmm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2onqnvdpq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ogfqwuaj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mlneahua.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksdowbvy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rriqqlti.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bfhsdjyq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zwcrxvkr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufdghwij.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vihqzara.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2glljhtuy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2cbcewblr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zqhyxyhy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cmmekyxw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vcbqdrcm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2akunddwt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2fnyrzjlx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zrbsjbzo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2sxvymtqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvkktyyg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mrpcxqpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uevkwytj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2bavjxrzy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2otigvgnd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jbsfcnvr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgxrqlqk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2whgviqki.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2stuyzgfo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fblqawen.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2mcadvdac.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ocszkhat.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rylxwmzw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zopdhaaj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmybossk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmnuicmn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rghodvgd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fohpvmyp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2aftyjsjt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sulqnidb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umqabpvh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nmdhfeqg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2asspnuwt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2katmpqpp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gsjbzqwa.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2mvgdqhkh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rcusornn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2clqdxcap.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2onszewnx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vyjiqsic.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zwnkrtpq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ebgcxdcg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avqkcdtf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jyrtfjqh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksqtquhe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mriopifr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vxwtdkhf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fldlpecw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cczxpotf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2byzznrcq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2idxetrdz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oldschkb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfqfmvrc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysxwhnic.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqhsxujb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lsenayoy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qtsnuufe.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzaebzwa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qyefqoas.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2eskttgqo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2deeczkac.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ecmggnzg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rbsyvhso.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aqxhqbss.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2njsdtvxm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xozbpxxr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xnbuxzoe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2btrxkdiy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xqaaytlx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2smuprtbs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gxulckoz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hsnehely.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ndbbxhrd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rkxbupwp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hdcqgvdf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aabspilp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bbormigw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kjzgkpsh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgfosdoy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kxhvqlvq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnfvtabe.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldwtpgqr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bitcyimk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2kcosavzc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojshhtll.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2emnpvpec.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ihjzprvi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaovhkir.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kyifdqwe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2lsehvftu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tspvnsza.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hopuihsu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ydieybmw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaoocrua.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2hdgzgybg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2npmygevd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tazxmisi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zjrszjrj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dhswboui.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hvsolrjv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rjhhttdb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oqixrtuj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2jeuxagje.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2aiofwefh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2geifgbps.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2buzyvuuq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckpbtxsv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2poqwbgvk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fpwrtshz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cqnypqsw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hzylnncd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dgxeowru.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xbfcvfks.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ctbrssko.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mxplkudd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hkmfllfz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kptporkt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2akzuseqn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hjazltaf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2odannitd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lgypkzzx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2yloqxplp.html


<!-- 参考信息 -->