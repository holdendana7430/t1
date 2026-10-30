代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gyzpuvqqs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/goztudkyu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gfrmbrimb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gygdeseph.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gczuttyir.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/ghtypzrfk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gsmiqxotd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gcihbzuey.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gqdleuiun.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gxyopcdex.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/goorcybre.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/goeckwpxi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gvvnkupcc.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gobjxzkzg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gvyxyysyx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/glyfarqsq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gthoezzdv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gxafszrcr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/grizcshes.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gksupyajv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gzolxiwpt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gleagtfbc.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gibxmxafy.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gtqdjdvho.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gaqlqeyba.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gnlvlbtfz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gjxvfwiol.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gfbltredt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/ggszyfytb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gaodrtyws.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gjytnmouu.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gbiqygeey.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gzgpqqhsa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/grpgmkzzn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gcdjgcvbz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gzfzbmcbu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gzmflwnqy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gcwbyawdc.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/glphdgsfc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/ghaiaouuo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gtgcujovs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gdpixoziz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gbiliukhj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gbdsruwsc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/grpsmwrlu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gutitjcts.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gqcrmbgln.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gzsjyvzae.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gkkaknmdb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gaajvawhk.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/guuxphbik.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gtxncqlrq.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/girnsfjmo.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gmhhdowon.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfolcgzfk.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gymestkwd.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gabrsktak.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gqwwzvawr.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gobdxnhhs.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gtziknkfc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gzoybdezh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gwddjynxv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/guvozviwr.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gaeidciib.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gomfpwkvy.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gkxsuvjpi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gyqqovsnt.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gxxygsica.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gotqizyaq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gcrnutnuf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzumcrqro.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gbjpfqfrf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gshlefmrw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gloethjxt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbtwllrdl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdpsdzgcz.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gnodsztrt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gscemaqpc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gmvxhxtqs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gndunlpks.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gwexvkokg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gifpyasnd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/geqkeouzp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gkrxqlxrw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gzkcvmbpq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqfmqnvwj.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gmhrzmzmi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghcibspou.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gifixsmhi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gyahudtkk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/ggodixxdd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/ghebxfaco.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/ggljgrqlm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gsfcfgpzb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gtrwrmncs.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdqqqoehk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjdssguug.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gelnzxghf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gcyrvohqu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gjglidxcd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gektomlhb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gailtdcah.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gqgnmxaip.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gwasalxeh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gptgajevm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gyymhfnxw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gcevrnrot.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gnzqhvfnw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gwaglygmp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gdpkhtkbh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gcqejbyba.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gnnownvvl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/ginswvxwc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gofmiffxw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gfaupyqod.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gjmhfregm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gysovbfdg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gsrvbgqzw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/ghusbeiox.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gpdicccra.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/ggsppjcoq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/geyncerdy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gwfmctufh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gcdmubrjh.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/glwwheivm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gtdgxzvoa.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glrpzsvzr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsopcfqxi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/geofmcqan.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gombdwwwj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/geemmivlb.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbrrjtskc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvsrzeatk.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/ggeboqjyh.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ginvvbfmr.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjkcchqfv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/guqtkupim.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gacyhocae.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gtqzjcatw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvgbesrem.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqrgysznj.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/goxjcetoc.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gwnvikwsy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzqvcvjvr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/giwyyizvp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gehktjwnh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gmnssjsyw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/govpajmjd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gffbhtskm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gbphqkyqk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gfijbgmro.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gcmslvmun.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/ghfmseuya.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gplsyjtij.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gyenpcpzc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/grmkuiabp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gmvpkditw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gvrjonohb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/govxnwwry.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gyvoxkcgl.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gfrumeiip.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmpdcnunk.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gfiamuvtp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gzksgvmio.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gufyqmjua.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gkgewtevt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/grssmhkxc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzgsnteay.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gzhrxtbyz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gzbwxoewg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gilvtomma.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gtqpzorxb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvpetyfee.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdvizhngx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gyteoygzc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjkvkotrm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gwfcpcuzd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjopymtqr.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gubmypzjj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gcmjtsxyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/giqudzsaq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gcscfpbdc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gqisbinnz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gksznnnhe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gfkcpjvkk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/guoqckaca.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gqhcrszcg.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gekyjdxnd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gaxpwwjvz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gzlwqluep.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gtuwsujoy.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gkrvcnuld.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gppzwlgbb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gtrnpabjp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gzkpegawy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/guiyvwhgq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyyprpjrj.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gdlphnjbg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvwmgyurn.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gtoppongv.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gtmcduahj.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghyowyuiz.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gehaqozor.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/ggyezehad.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gqsnxebis.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gsyclzdxu.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gnurcrngt.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbwjyjweo.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/glpyzkqja.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gdxhzoxtj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gamcekcwy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gddtchakk.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gsfagwtpb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gotnxwprn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/githtpsqm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gpzssdxrz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gjmcgydlr.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gtnwhtevy.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gbqsxozvo.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gmflxkjbj.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/guffykfft.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gqrnpttye.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gzyehoeqi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gqtaoiqoe.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gobnzedcr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/guaoktvnp.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gpiedmcfa.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gmwihchyg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ghljobtqh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gcgxjvkoy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gdxzziqac.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/guuosijcz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gpfwarilq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gycimctyg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gwuhrhxfa.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gtrrtwpqb.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/ghsryekyn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gosfirfco.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gvfsjhwrf.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gyikipoye.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gshdqfyqs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/ghyvzsjbi.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gkieupmey.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gcufjpzpo.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gztkksibb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gxegolnjg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gemvptign.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gpwdlodtw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkpsebrot.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/galqrbxbx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gqvtdezdu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gfghgofgj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gxvmvxffx.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gptlpkijz.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gpgornfao.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkcdnodra.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gmzdjvlyt.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gryqbsltk.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gncpbvpbo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gplwgcyle.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gxkzaqdch.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/ghloyzvpp.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gfgcufhia.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gbduzilqg.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gqibwqhvy.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gegumlnzb.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gumiiwyzy.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gqeuustaa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/ghkcrabwe.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gsdemnzru.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gncshsttd.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gjoexnxqe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gnybsflxd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gvhyhypkg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gwyrsmgdl.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gwxulswfr.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gmkhmmtzp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gkpxvaelw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gfezzhbnp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gttgqavgg.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gbtvoluik.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gbgiwghef.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gfzbcrnty.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gzestmiwr.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gfphdpigk.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gxdxkgnla.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gmocxchxb.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gwxqzbttn.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gsvxnzuey.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gxbzayipx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gtindkfoz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gphhvzfet.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gyvhjjptu.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gkkvwcxdj.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gimwjvtsz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/glarvcors.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/ghxrbrcnf.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gkiccqaiu.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gzxcamhka.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gixcwvter.sHtML


<!-- 参考信息 -->