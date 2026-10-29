代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gzevtwofm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gmohspzcs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gtwpwtysn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gdtogpjlv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gutdiigqi.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gmxijuztm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/guwbcvdvd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjbvnanhz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gpujghoxh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gkmmxnjgu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gekhcijgk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gkvdrmdmb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gmmzjwvdu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gwyinmdeu.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gzdzhoemh.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/ggjgvnlyu.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gatizwgbb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gtlpztlmw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gxysgdygq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gjxjtqyym.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gtcjoollo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gmvsjrviz.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gbuxueatq.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gpqawdenu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gikflgzab.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gerzrwiej.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gaueoqgbu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gnlpuainn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gepqmbjqn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gffssnoel.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gffihefqx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gfvfzjofb.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gvhxlwfry.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gmkrdrelr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gudsdklib.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gnrmbjzzh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gtuupxadk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/giozsmenw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gvxrmxehv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gbhizwywu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/glotqnokz.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/giabfmkcz.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gwffomzov.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gnkrymuso.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gttqxatop.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdrqwcnt.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gznbmasqt.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/govnciqcd.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gkuuajxll.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gmxijygor.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gpxcdrkgt.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gidymrrdb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gurhxecjh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gefbpoyfm.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gfuqxzmll.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/ggiptpnsn.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gtzxvjxrj.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gbhxotizr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnaoiuefh.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gdbrfteuk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gigukuyxp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gcdlqizlm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gnqqjvmav.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gbspshuww.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gknbisvza.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gbrvoiyca.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsqaxxjta.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gngvbnvps.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/glerjcjjh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/ghfrylfmp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gvudszndp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gahuuqzty.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/grmudatah.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gfhveudjz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/grgfmujyc.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/guxmlstbt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gpwuispaf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guvcezwcy.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/genggdeze.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkfnwqlls.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/ghgrnewmt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gnmktqiav.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwtpukegw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gieaxrenj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gedqbqyjs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gljyaqjub.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gyrcjmffz.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gymrkqgpg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkhhiamzz.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gqpdvjgbg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gkokusvxr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gldjzeazg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzirobwaj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gojpmhfru.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/ginrvilzp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gzlyapino.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gugkptzxm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvpofjzs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gdzoltjvt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/grjeqywsw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gaigqqlgt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gfkzhfqzj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gwrivnhxs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gocctxnkx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gelmmgqyq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gscnoimhs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gwregobxt.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gtimzlokk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpmrwcmsh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/guhivtdfr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmdjzhkwt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gvnuxifeu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/grhgykqmd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gjqbegwcv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gnvmekloj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gdduytyqb.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gdtuhhacp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gbuqxebmv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxkrvmico.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdxgxoirc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/giqwcgokf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gissnebbj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/grzkznffb.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/geidfqzge.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gudsvamxy.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gslpwyuxg.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyuhlwlnl.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gudknkwmm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmhujdzqp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzqjzlfjv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gquwyanxy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbfysrcsi.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghrvxhyqk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjapffdho.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gbwntohqu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gpxmomiek.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/grbqokcca.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gbrftuxlt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gcgiiiznf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gqgduypkn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gfogtxnar.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gphsfyryy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gcuxqjrrk.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/ggnrbtxbv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gtraodkba.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gwhuevnli.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gnhsmtpij.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gqnjxxzuv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gnbznemdg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gisolnbnm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyyxdhqk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gknnuhizs.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gxnglxfma.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjhmlqqlz.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqmsjnaeb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/goxthyxsp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gdhlxzcie.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gsgbvwqaz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gymnstinf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfnuriqie.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gsjfcncmh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gmddscqtx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gunimavou.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbnxhcmrl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gprilmjkw.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqzophpgf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gjmgtagwy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gsyaoktch.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gamlxrzzr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gliuilruw.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gaxllidjy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gvmxnjcou.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gftsgmder.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzrvryaef.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuhtvolb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gqtczlxmb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/geugayiik.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/grvagnynf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gzzxgkdvq.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gzzadcosn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gnafnmcki.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/ghbkgliqk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gxyidhnxg.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gybnqnafy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/ghrpwyixx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gfamzzrha.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gnprmdypy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gtvurdfcy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grhhpghre.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gqtoxwvsw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggjmwicgl.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/getposmrp.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gayhszmoq.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gdblytkyh.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gbgjvitlp.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gcemvpygb.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gttkysuly.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gbdrwylcl.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/grnawokgx.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gcxnbujfz.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gkkdsokme.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/grnecxcsy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gljjvdywq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gbxdykidl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gvamabvds.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gwoqxsdjq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gaavntoam.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/galikiebm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/guchlzdll.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/grmksttpv.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gkhlgoleq.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gaimwnhzm.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gyyvqnmlb.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gwqlyvggt.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/grmalquxw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gbaghanhc.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gpvgibphy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/guxxrioxh.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gilyjebbb.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/glikcmzum.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gakhbknai.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gczwhbxgw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvozfyuzw.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyciqakss.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gbogweaoq.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gsqailkln.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gsxnojjog.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/ggdizjtaq.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gdiuledmo.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyatoykpr.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gzofadbuh.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gsqoyyfoj.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gzepirkgv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gppgunyub.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gzehoedeb.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gqttuofto.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gymwupicq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gxrkqjfkx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gqqygwdbi.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gjdlemosr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gixtzepro.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/goomeumno.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gaaeywstd.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gtmzhxaug.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gqfwcmueg.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/grgkccswk.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcuksiy.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gdkjbadmp.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/geumdsqaa.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/grlhmptnb.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gflsopijl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gogokrvfx.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gykhipisz.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gegzocsfd.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gcmafevxz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gfeqhwnsa.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gfejgharl.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gfrycqfwj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gobybtjiq.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/ggppsfnzl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gbzlfnbbw.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gxdtltcxl.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gphjgslqg.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gaxtyqpnc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gwagiozix.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gcxnrmszb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gbdowaumr.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gmhczypmi.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gpgqoypzt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gndrjpedj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gvchutpfw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gihcfeepa.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gbjwpiypr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gydbkxtqj.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gtcsyfmmm.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gmgchnayh.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gtwliwdkq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/guoqnzdng.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gxohkxtth.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ghymoaeod.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gdizzugay.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gjjixavua.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gbfjfdpaj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gnpvndflk.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjklxdajf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gigsbbwgt.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkwtypmda.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvtckhvh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gjuqvmmtz.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/guqgzpelq.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/guvoefvvs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/grajcdisr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtlovdgev.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnfssjplg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ghgrektlb.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghqwujytr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gvjvcwwyt.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gswmcyueh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/giffzajfw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggdwemxsf.sHtML


<!-- 参考信息 -->