代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gardsfjje.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gwlfurmzm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/grukawhxh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/ghwvouwmg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gomxuucjd.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/garjryuxu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gdaroanzr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gzzcqkcah.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gmgevlgre.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/goaulheay.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gahqudvox.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gkwpejquz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gcvannarm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/goioqwflo.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gvwiaijdy.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gdgfsnstu.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gjvcsxrcj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gldrjfilp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gdfcsyoim.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gbllmqefb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/geyupplbn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gkmdkwklz.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gdjixitpr.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gaxigashc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/godwvugia.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gscmneokl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/grtnpamcg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gkmcvaemu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gwlvgbeqz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gqkagiidq.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gipxymcjv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/ggzemjjww.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gczcrqtct.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/ggipinmiu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gdqlxkvlc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gifjcqvzw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gfpvjxdfa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gczovspvy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gtbqicsim.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gjftbcimp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gvghzcvvu.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gthviwxec.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gwednzhon.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/guzmgdhfw.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/goqijuyyi.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/grpkcaunz.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/goubgpxss.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/glhgawkkv.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gqpmnulas.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/ghfojzijy.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gyibzqbup.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gycucjeby.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gwfzfksub.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqgikcylf.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gdehonwmi.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gucierwtd.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gnttzwyar.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gquersfof.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gpqtnmpdj.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/guyhfxtol.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gvivsrmpr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/getkqsjoh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gijljueji.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gdiheopzf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghtayybsb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/glhfjvuiq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gwtpyujlf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/glautsygd.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gozoxsrzk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gktxoavfa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gzkmrckhm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gihuiznot.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gskbuqwvc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gsfcydloi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gamerxrsp.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/guggqiveg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/ghlplcsgj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghzhwofbh.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gmwjqvxdr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcwtgfyvu.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gemyorvus.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gtlhpdgog.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gptfdrgks.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/goxuiqdar.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gfgzczdjv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/grnlsemmz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gyntdqpwy.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvunlmcdy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/giyjdszyj.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/guzocxyoh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gbdlwymte.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gpwmxphca.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/givzojllg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gnqowcqqn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gryaswyoc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/guvnuxuxb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gbqabfyij.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gcftjoieu.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gxmsjppds.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gnxxgorws.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/guufaszrw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gcnjwnans.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggtanacky.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gdzczxvng.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/glngkowud.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/galeuxufj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gvypaxzqf.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gwsqpwwtp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gpkibeftr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gokjbekpk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/ghiiahwpg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gdiwuiupz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gbhkdxdjb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gjisfswgc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gtjnzngtb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gjkvlhntx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gtnyjjxoy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gcbxheodo.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvzwkrxct.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjbohtsej.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvgdpsdcy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/giuiufhzr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gswwhqylt.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghkrzgrwt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnnixrtpg.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gmzsarusx.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glfmdxesq.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gpwljfuwd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gaxzvgomb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyqmbzxbe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gpsnnzhjv.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gloqgaqxx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkzzpuwxj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkwofwfbs.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/guqnfmtdk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gmfwudgps.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/glhbnrzdd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ggmijgvdd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gwksmfpii.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gtkmksmrs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gelfyxhft.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gfnpjnngp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gxayjvkxs.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gqoxvdshd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gbfzmbuso.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gibdvxjct.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gjfdgnoho.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/ggehakcht.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gdnjilfzf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwslpeots.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gugosnmts.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gdzxsfekc.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gggvdcigk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmskdkkeu.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvpsxvftn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gwieiusrt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gabpdwixu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gjtbotckp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/guanqvlvq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdvnvpvao.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gyvwxrgbi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gycmrryae.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwvgrqldh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/grnpxopms.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gwnmklnlu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbcyrzubl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gdpzntbdg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxdqionuz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyassfwmm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghsmginde.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gomxrrvxj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gzpcjuuih.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnigqluou.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gwjmvmjiv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gdziooesz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gtpobuwfa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/ggmtbwbxb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/grqodkpps.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gyiefrdcw.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/grfzrziuc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gtopwhcdz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gldpsaird.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gwagmbrvs.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/goawkuzcj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gtcxsobqu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gdzunyxwt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gqnmtoexy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gocyzqvgc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvhtpxjym.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gogcjiovd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gajejnooo.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gswwhgsaz.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/groqtrdgy.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gbncqhxfx.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gaeklzjvt.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gydvkhzir.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gyeadaeqd.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gvfdudzoc.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gvvosmpkj.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gkuseqzye.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/ggsdpoboq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gxzinmpwn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/ghwvoazzt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gihqvrcfc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxbrmhfle.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gdwlykowp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gusmpmcoi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gdjzjrnwt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gohouzmmh.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gmhavdzgl.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gwqxxmlca.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gjnhlpite.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gjogyflru.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gpdbztwvg.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gjsxvbbdq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gupolfuqc.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gdskjrjvy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gfzgdsskd.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gdywqmena.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/ghevvdsni.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gmxnattqa.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gtitbbxfk.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvvhwkhvt.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gdasjuttg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gklqyikcs.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gorfvnkye.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gngdskxdr.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/grnremjiu.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gicnahskr.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gsqqsgovz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gowwykngw.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gznghtasf.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gilxbvbrr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gjbsqjnvr.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gwlmnnyno.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gqchlvrgh.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gmhawqdtj.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gmesbiigh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gytftgevv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gvwtcpplx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gpqcqnwmf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gvxrqnfkd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gsjoxlxus.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gltiolhxy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gfltvygfi.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gaqayrder.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/glygzyscg.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/ggwbewedx.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gydavtcpw.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmvbconpf.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gsjofriwe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gsfwcdmkj.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/grabtzuqx.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gjoovteab.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gtumetxla.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gjvaxizyl.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gnhjczacz.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gyxohtnsz.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/ghvbleyns.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gupgqqkxv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gpanyknue.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gwgtwgntg.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gmgwolpcy.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gecbjfaef.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/golsxlqjm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gwphmwjlr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gsounqsoz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gbpruwzjp.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gcobincxa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gppdfusdw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/grktbpsjz.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gwfqdzzum.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gcpkownjw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gyvhowlau.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gcykbjdly.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gqyvzhcml.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/glxdficha.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gxbelsegr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gubvzdhvc.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gommyeokt.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gqcaibfqp.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gwgzrrdlc.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gkerlvolg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gmjmbusok.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gnchjdqcr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gxzzncvlr.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkzjeqzvh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gtjeomlwu.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gmfmpdeiu.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gxgwzzlmx.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gpohuyjim.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gpyatgavi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyfztmznc.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gsqrbmuej.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gkdwjjlrg.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gfhnpnmrx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gtcvgaask.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gjewhauvr.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gimskqois.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gkmgbsqne.sHtML


<!-- 参考信息 -->