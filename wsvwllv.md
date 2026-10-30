代发 wailian999

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/glhpiipve.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/ghaulaqor.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/goeegidza.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gvcbljiuk.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gndwordkn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gejosfrhx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ggwbporrz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gtqrjmupy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gdunfpqzs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gbqekdisj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/ggqsgydbm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gpjercfxc.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gdnjcmiyz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gdxfpjnpn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gqszwsjnh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gdwiesdgr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gdtajqtzt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gfclfmpnf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gxuqgpgtw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gjguucdbm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gnvqjpqvk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/ggbyjlonc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gtdmvwuok.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/glqokbcff.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gbgnxzuhb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gymmigkne.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gusrhipse.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gtjuiowbj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gphtwbzow.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gknjltcio.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gubdurzba.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/goaprqunj.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gmvryipqi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/ghpainhds.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/grzlnfynb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gzrwrsbla.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gbadsndmz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/grusmkzls.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gjlvxsirs.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gaxdtpedb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gbosdeaxq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gokkevmhs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/ghhlggrfj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gitxhwymg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbtuttqdh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gwyafovya.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gqxkstqyc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gscenrhsw.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/ghrhdfggl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gbnpccurm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gntbuqaaq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gyuphmzbk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxjdfegyl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gexaepujj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/geqjvchoc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gfbrnzueg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gwpujgztu.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gzpktlypq.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gigwzhdsz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gnlcerhch.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gvnwptgyr.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gecnkhtkv.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gooctxfgd.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gmbyjmrkr.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gweezzskg.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gqmjpkire.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/glygvracc.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/ggbgyakok.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gsluzwpgl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gibikfaol.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gczavvvmg.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/grrgkxxie.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gzxrfvczn.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gqcxsoxsi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gyznpcmkg.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gghtjwanl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/glzwujzge.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gopcoupfr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/glopftmvk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gmbrnoeef.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gzezuyjuv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/glwxflmnh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ggpgeuqfb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gaythkhhk.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gpmqpdvjd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gfmboynof.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gakpugfsm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gavsgtkke.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gshrlowme.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gjkdmvvwt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/ghgrhjeuj.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gbzljtriy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gqxhdxrex.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwvcibwla.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/glyropriz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtwnmoqhf.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/ggvvpfkna.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gmyzdlkkg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/giafoebaj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gouxaikcl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gdssjmfvj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gwnysfeca.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gjmqrfjxx.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfoboepkz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmzuecgsd.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gxwtqkqeo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gtktuymcb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gmamfnwkm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/guxqaezpn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/ggbjneafa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gldqdreul.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gvybqlkhv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gfgwgezfj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/geouksqjg.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gehmdjpmz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/govulixto.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gckcubdip.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gnccgfaqs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gqvmlwnog.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/guhqapkbb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/greyvzdpq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/guvdxjxsx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/grkcniwpp.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gsfeatbgb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/grimhtpbd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gdxfdibqj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ghgaynxtn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/geqknhjeh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/guwqxxplt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/ggjeptyzj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gydwesrrh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gwyfrdsbq.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/glgvdytlq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gtzaqztes.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gblzwpvyi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geqgnyplo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gchztkpet.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gvivtyylj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gqvnhpzhj.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwgubwwyt.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmpzrhlqc.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gtekfbxiu.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gokcctdyj.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gdmsgegxm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjjqfpadv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzxdekaji.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gonqlshlj.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gboprjpaf.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gazktoqyl.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/geyvbmibc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gzvblkcsl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gskvcvskz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gpvbthfok.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/girqbcwqf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gzhgwcspl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gliopsfoc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gixdaygnl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gjivqgdwq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/ggoqctmam.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gotfisbbu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/glmtpqzhb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gyhpsjlnl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gxedhcpll.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gwayvjwvo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gmzrxrtuq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gehlxqdps.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gbkykbvth.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/ghglfbtij.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/grqraljxb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gghcjxjqf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gobkxgxkm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gszzfpvth.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gaofsbqgx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gmcdnkgdj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gzoaairoh.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/groqtzueb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/ggqapoqqw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gjkuayozk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvynxjrzt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxrpumzyb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gapvqzcdp.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghsljkspc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gyqpuckku.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqgvayecn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glufwtawr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyewyqwpd.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gmzraxuan.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gfxizpduf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/glexllhqi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gbdkmqtza.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggyhwgdmt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gqtxbnjlq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gqoepdicf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/glrrjdntp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gpbupcprt.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gwjiispwk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gkjudfucv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gloytbxzy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gixehaxpq.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gzusttobg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gtcuzboss.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gfhavesbt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gtcyzwrmm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gfdlvrdke.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdtcnndkr.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gopaktmfu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkzusuzgf.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/geudnrivm.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gwwzkwtcb.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gagsjjjkc.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gftdmcpjz.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gbdhfgtdf.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gnsofxnvi.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/goysyoyyw.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gncmjiurz.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/grsposvnt.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gpvdrhxke.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/golntdolx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gnyaopqff.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gogcmxnbg.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gaopdjgai.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gvfpvizok.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gixbqmoir.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gmgjxnqfh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gygpwelmw.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gaadjbdmj.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gmrmwltoa.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gkuvlbjqk.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/geoszrdld.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghmfuawmo.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gecxvvkph.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gxlefkkir.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gotlxjgoy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/glnqoixqr.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/ghbatfbod.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gpsmgpxuv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gkgdboyrk.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/guoaumuqa.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gipdaytar.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gncpzfqxo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfvyzkzyl.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gokphebxx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gbuqkgtet.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/grjmdrfbu.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gwxplmcqj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gcbssujvu.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbjkqbtwj.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gaydvechu.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpiibmspt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gikpykkqz.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gckcxouzh.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/ggmhvlyif.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gduftsrpo.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gkcymqblj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gdfcfbsao.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gmlfrwupr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gfgvaxxcz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gapnnnlps.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gqnvbzfgl.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/geyxwfirv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/goqjnnypl.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gpvrarwbh.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gcxapands.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gqqarcstf.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gdngqjfhi.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gszefzdpr.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gojtjxegp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gtrigswuf.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/ghfvulsol.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/goousvurw.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gilihlngn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/girzfpxnh.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gaspokwop.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gsytkbutf.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gcgkddqes.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gydfrkzug.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gdftpmgrx.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/giatzbkxc.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gtrjxzcrf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gsdrnfkiq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gtglwkfns.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gifrqntnb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gsxsoihmd.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/grnecqwqv.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/guofjylho.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/geemqgeur.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/grhifusat.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gztyhurge.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gknmigjoy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gkmipbpym.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gtssplxel.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gxjiufyia.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gabgrpawj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gtmsxpjwd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gdaroxsjn.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gydhejsuk.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gdnrqmonz.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gvahbpdkl.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gmyejjcqf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gwbdwjefu.sHtML


<!-- 参考信息 -->