代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/ghqksnqpg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gyzkuncek.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gmvnnhodm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gffrmdxxf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/govzqhhoh.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gqevwqxei.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gtltobfvy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/ggfemzhnf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/glhhrdgtr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gtfqiceos.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gogoovmen.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gwcaimkwe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/grpvvdizn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gsizyuekl.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gybnfenoy.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gzluewwbk.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/ggoejaarq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/goqunezin.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/giirfsdjm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcelqsll.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gmfnmcsgt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gzrzcpkjo.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gpbobktsp.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gtdkmjxjn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gptjyqlto.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gsfgyxcww.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbjmzgpsz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/glohqkehc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbcljxdej.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gtczcgdjd.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gdovonqpb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gftbqiqmx.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gpvefgsjk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/ggzstpzda.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gfmtzlueh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gmjqexhly.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ggjsgwtoi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gfzwvdrjm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/grzvabbcu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gdjzcmqwk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gstijmvtx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/giajnjkly.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/grnrpvfyq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/glcwzvwhb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/givkkjjzq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gmxywknlt.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/geiajxzwc.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gllhscqec.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gdnnxdnsp.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/ggluinpdl.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gnngykdiy.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gotddgxpc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gtpmcbfze.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gpcqutgyb.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/ghaawsjgp.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gbjfpoguc.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gbcbelkwo.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gzzsyztkj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvszhzfkz.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gecqeuqxc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gswmvebzv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gsjpshmcf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gjbyqlyuk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqmbbzxtq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbchgukhg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gaxyahtsx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gucwutros.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gshforedu.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gmibkcwdo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuuhhcti.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/giezhuqle.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gcjvmhatm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gpglyrmgi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ggomjybie.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gzwdcdudr.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gwiadbfaw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gwkgjopce.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gudxiuqba.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gzuneezqu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gttgtqnxh.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gwqlfkxpg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gwjlvlcjl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdsojuofi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gxhgcmuue.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gbvtcgqdo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gniotvvkp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gvxkzhbuv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdjsbwuja.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gaywwrmbg.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gyibqaemd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gglmibqnf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gwvtdgplj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gomnqtsyn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjqsdxsgi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwvsenuw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gsonfxddt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gsfezdxlx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gtdioqjod.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gurlqqqxt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gkldqjpaw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/guzklcysh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gtyydoudg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gobvuuzby.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gipxsxmdy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/golukzdow.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gwenrkakf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gphjopmnv.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gokvndmnm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gmsmtpupp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gkknrhkmg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gurvnjznt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gspluzqye.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gulkrqxij.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmkczqpqu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gaiycxdix.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gkoljhvdm.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gdrapokrk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gtdjjcagf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsvkqtjwx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyzfzmmmn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnsbbiahg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ghrbziyah.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gikmwljgo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfwamyvev.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsqsilqjm.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gijvrjzce.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grspvtqqe.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwwxtqwpe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpgekvuvk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gizjasxnl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/glkhcwqbc.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gglkmjpsv.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/grccaefjm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/genjxocpk.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/glilsyika.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/ggceopqvx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gaioajnnp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gnelzxnyp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gujehvjgf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gmyglkbyb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gpkgeygmu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gbairmgys.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gbkfpzeoe.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/ghehsusqi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gvaptfxuk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/geiblbvwg.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gfvfeezqe.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gvzhndjnx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gijsnypos.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/grbjymegc.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gljrlriln.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gytbvzmhf.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gddncvemp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grqzzitpe.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gnsbhuukc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/grihvcrit.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gozcdrnrw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grpjaoquz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gqmyultbh.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwtsvezsg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gvnvrsrvb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gxyeutgbw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpspohmcu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gkxsibwrl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvgciojxx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxqtamfkr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gdnuryndc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaizjpywt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/grqwylpdv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqbinkbzc.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gmkutspuf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gmsqhflnn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gguohkyod.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gyllrxldv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gppyjhbkr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gyisszrek.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gvbfnxcfb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gmtzvdfjt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gcmcmoute.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gdrzzdicw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gyibexauq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gvnytyait.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/ggohgnusw.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gmqwxqvig.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gvidvgttg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/glvyvqbrx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gdkunfjpd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gjsohzdwa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdsdpxyvc.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gejcbagir.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggybealky.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gwqvomrvm.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gnmcsmdiv.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gslvgfnpg.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gcklrozwj.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gjgtvltse.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/glhvlikyr.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gsujhpxuu.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gtoqqczqr.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gssvfcups.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gbuxqqxuv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gtbraelwg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/glivfleiw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gxfkoxxnp.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gyohkwibq.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gwchbbacf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/ggpqejpmg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gkatcqiwr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/greqzfhyx.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gnswnamhe.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gibvyxtbm.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gauvtunfw.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gvqfedwnv.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gdtffpxju.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gwlbxckai.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gypjiyfkh.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gqovidtlr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gxitrcgyb.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gcdkedtrd.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gpvbcsptd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gcbxnixmv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gjcgikttq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gatsgndkk.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gzngaaktd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ghatjnbob.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/giirujwri.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gyvjaqjrs.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/grwlapmhl.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gbwufppht.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/godoytjca.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gflxephnd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gqiczzqgh.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gdxiiivoq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gynhzdhtj.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gqhjeeima.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/glgklefpc.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gyittehzq.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gxscgrwbl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gomnmmiqf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gugffysxv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gisskjwnt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gxwrqyurp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gvtjunsoy.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gkphwjajv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gqnltfvyo.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gmpzuedzz.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gqeymoqso.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gjfkqtzjh.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gewifvclu.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gqpqfxpms.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gxvpeihnq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/geszfrrfa.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gqvxjclxv.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gjgyajiun.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gfdiabbnu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gwjkowqxg.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gukxnrgha.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gpniaxnhi.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gjhwbdpnq.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gxflnfhqe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gtublxgok.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gxeendcdn.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gkukcffng.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gpjgahobg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gvfzevlsp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gqojjpdrd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gsyzubfid.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gaxdrpmiq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gvddacrdl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gbuhjguxm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gnomgnoyw.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gxshzetbg.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gghgwxhkg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gjbburbdy.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/grifmdeef.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gkpdgriam.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gucjeclca.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gfjurvkhf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gictvynhp.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gfnsffrgn.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/glcsfictt.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gfivpzzft.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gtusgmffz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gqgwygsum.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/goxcllfgk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/goniqjrqc.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gnzxfjazf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/ghuikcvvm.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gzgtehfcj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/glizivnhk.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyzucmrur.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gkbssfwvb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gnsfkzvtt.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gygoulfip.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/guagisadk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/guzzbcxgf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gztvxfisb.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/glcgibyzs.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gjeixapqq.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gnfsravtl.sHtML


<!-- 参考信息 -->