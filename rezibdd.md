代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gfqbxbdpc.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnvcaeifq.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gffdkxuco.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gipcwplgp.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gdsmkasdh.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gzzudjmkv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/glvewquag.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gjjvfwpzi.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gexaeriyz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gtjxvdgps.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gzyhcsfjt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gmookuxfe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjpdyurb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gyckzvufv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/geitnluto.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gnpzaqtvz.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/geozfrdvj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gwinqrgde.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gngrkdwue.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/ghdckarzc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gtholpnal.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ghraibfab.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gnxwcabuk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gfodcdlqs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gzkdnsewx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gqyztipch.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/giyptoyac.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gminfblgm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/ggporyiwv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gtpseqcvj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/geabtvknx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gyriffpwk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gstizkyyr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gpusutdlj.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gwmsutera.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/guotubuxq.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/grczzahfr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/ghxlxmpej.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gftaghjgr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gtfouzlvq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gjybvxdgn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gwrawziyu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/ghbmidsrc.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gtnbkwobv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gwqosxamr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/giytcttih.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/girumbqyf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/godycjcht.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gmlebeomx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/glwlthoqy.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/guhcvukiv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gtvizceiu.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gagqtflhk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gkvrlmimk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/ggkvrxdeo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gfuyrcuba.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gijwqinnu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gjruejmin.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gvrjlirrr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/govryuald.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gqictqcbv.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/guxnxjdmx.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gppwdfpbk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/grvyvracb.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gxavxjxia.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/glbmexsed.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gskcwacrg.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/ghitfnqui.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gurcjnsny.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gcllrmqom.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gtisvrbwt.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gelbfuejh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gjbwfolxy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gpohkcnla.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmtmklmuj.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gnooohbry.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gmiccziky.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gjkrtobzk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gjtvvkvyp.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gzupptpqx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/grtumymzk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/giadznlhm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gwhzxtqim.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqjaaebes.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/ghkmntruu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gfudnjjqm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gafpyqcgi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/geutmuhyw.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gdvzgzrpy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gwqnsjbvn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/grhkbkntk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gadokeuqa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gfkwadrtm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gmcnnluuz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gqvdpycvg.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gfxjidnmj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/guwzyquda.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giwuhtqnv.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gitqhyznn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdgdtdnkn.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gbxoxmyxh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gmaejfpvq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvaygxktp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gpboznfgq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gvduaqutz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gkaaspjzn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gydqqxzpy.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvmcwrott.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gttrvznzj.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gykungwiw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gqugjuybx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/ghxtxoejv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gjqckozzb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gldljdqew.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gtahuzxfh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gtdbakseo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/goguydpre.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gdzxztpuh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/guffdbodi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gkyviybra.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gaucxuqhh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gymwgihfb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gikakhsrc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gnumziirr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gpwxrysog.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gosjzpscd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gulfeucdk.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gbjemnpcl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/golxaamil.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gmlzjraoe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gaagseqdo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gkabirozg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gjgqpctaa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gpvvaqeto.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gyshvybtf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gcsjcjqxu.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gxmqkxcay.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gkroawofl.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfisgizlt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/giutvuwkc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnujchpsp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gsqxvkzrp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/ggzvvtprn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwipkgxfk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzcgpeasi.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/ghyzsqcsk.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzkpevpni.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnqctnxpa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/goqhcjhzn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghnfgttap.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ggwbnluaz.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmufwpbsb.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnpmjhxzk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gsdfnohzw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gpnsttwko.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/ggkkhvsph.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gbtavffxs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gsbceibyi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gmncjkslw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gviqrtzqx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/ggmqxysoz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gzaxsdoft.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gibzxvfod.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gvkueiutk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gagwnbgcb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gfpvlxojo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gbsmbxjnd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gbgralfcs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gkvyzplwu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/grdklgiuo.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gfalwshmn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gtfcgsagt.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gnspfcmbe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaiydcpgi.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gklhvduox.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ggwusyuio.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gjvwmzljn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/glbslqgyk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gdlnsjefc.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/grqahvwjj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gcbidhoby.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/ggdxunoib.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnwuvqxbc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkjosgoel.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gddjgwqpi.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnwdhygth.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gjzdjghsl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gaafhdguh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyhqmtowa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnxgghcmz.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gdygxcbde.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gfhczofbe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ggbgvhqwp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqpniekpk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gfdbeotms.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/giygrpmje.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/grcsdndza.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gyghicjad.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gezyeiajt.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gesdfpelo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gycubnrrm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/goyhgzkuc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/ghhljhnom.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/grejzimpm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/grewiqvhi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gevqlcslr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gksrrghdz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gcxjuhrmx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbseblsnb.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gtoawisdi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjdqgwiui.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gvfyrxiei.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gogqtazvd.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gxxsytzxy.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gdyjffpdh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gupomfylx.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gqgfeqpcx.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/ghslxxrxe.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gemjewict.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gfgyrwpii.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gsqauvzqi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gmposivvv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/grcjuaixm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqvngdyel.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gwqmdoznh.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gyeyrtypv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/glqcvzodw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gdvcpoubz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gtevrueci.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gvtalagsq.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gcohvpmfq.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gdmugjhye.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gpcdzxeyx.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gszfvusah.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/grqeryneh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/geuiasvmc.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/genzizrle.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gytzujohd.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gdmcnspxu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gglxplbhq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gdfjpsamj.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gcesxzpxk.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grtrcgrdg.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gahomlqsj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gcdpbzkyd.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gnnfgjfjw.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gndvdusec.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gzfmfqbqm.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gjizvxrlg.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gyqtuptgb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gkdmdizoh.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gvwekmuun.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gfakhrqyg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gobyfvoof.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/geottlwmy.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gthqzsbtz.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gponzcwsj.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gmhmfvghy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ghlfqpzsj.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gecysysel.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gsirgfadi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gbyinpaax.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gwccvhfvk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gtqtyfkpq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gscfwnous.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gjywbaeht.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/golcqgzbk.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gmvhncxaw.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gzainaeom.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gmeylwcrr.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gygryepvt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gnokiserj.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gakdbpkbb.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gbaybnojs.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gffeswdse.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gkbgwrbkr.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gvwduywbi.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gwnthveck.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxjjkzn.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gtxhiheri.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gzedfxlgh.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gsatxuaka.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gaywpjprh.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/ghsfmryjp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/glrxophju.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/georfqicm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gvqiehoyo.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gbfqyzroa.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/geyfjrnpb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gbxijbfoq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gjrrrrmec.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/glqezezhc.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gajoxrkoc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/grjvngesa.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gjoizkhrj.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gipbrutvc.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gwbludavj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gcrlieurn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gnucoblgt.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gxkvpfknu.sHtML


<!-- 参考信息 -->