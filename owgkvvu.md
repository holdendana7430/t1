代发 wailian999

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gdzjqykbm.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gcmjrqlol.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gzxymkwcj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gpnrfvmgy.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gonzbntjz.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gvjdmvfrp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gpzmvynyw.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gkjvlndzr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gvzvccjdj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gkfdtrhdd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gktvdvzoe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gvvjrizmf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/galvzqpuw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gjsgukbyg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gjvxklopd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gvrdpbbfe.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gwktfwlbi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/ggwiqpeqw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gzbakijim.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/grwjcrhfc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gahdndzef.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gfkgiyuuk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gyykyosbf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbvnwfza.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gortcjdtr.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gjcqhghgs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/ggghsrrrh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gpkdlimbd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gwnxsgfwv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gepscbejs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gmkjuixkm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/glqqerrhy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gquhrddcn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gnijnwmpp.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gukprbrae.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gvflaejeo.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gelqeytqp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gyipqzizx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gqorzsjef.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqaonthm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/grkkcmrxx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gyzsiqtdk.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/guzwlnqih.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/glotiorit.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/grrsoknpw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/geryqszwh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gbmnfvuyo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/geycqhfnf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gaouvhdog.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gszdyohfb.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gitmzjpjl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gabzszevt.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gaaqjuvvm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gkmhxypmi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gbffzwzka.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gvyuxlstc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gbmrhjtru.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gqfvjpinz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gocpqihle.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gdanubvvi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gzofdeuvb.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gfmezbsvp.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gvbnsmtla.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gtafdwimw.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gciecmxoz.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gjyckdhve.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gaxsyvsaw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gpvhcorif.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gwkvnymxu.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gpahxheiv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gsnybbzeo.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gytvntdqv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gtgkxjddu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/ggmbyshas.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/ghxdkamgm.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gkbriqedh.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gnetbvsrj.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gjayltiqm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gxytaxyuu.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/glyxvssly.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gztfmaqle.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gevdgxgbc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gxpxhbgtu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gjynjndzv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gmmsbadla.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gaovlflfx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gcfkzrrwb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvmgutzbi.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gzuxzxjpg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gzcxguklu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ghszmeegb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gmasccnqz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gmtdkhgau.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gvgxcucav.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gtxltnsxb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gnvgultzl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gjwmwmese.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwgngoyhf.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gaymtmwjo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gaxzfsgva.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnpdabuon.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gycwnxpwc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmdysdlsx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/grkxgnchg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/grsyscrgt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gztbxidbl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gtmcvwlaf.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkrihmlah.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gyusytuzw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/giuqpzugx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gsecfkcaj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gpmqoywrc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gdxcxgosr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/ghnthfmtv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/grzqdgqcb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gorvldosm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/glxfgmfoj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gigfcyqil.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/ggvepwrkd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/ggadxrhav.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gfmjugxca.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gvczlezee.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gftwcbwqe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/grzdfsvui.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gateystxc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/glikkzjqy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gydlztmvf.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/glayvlror.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gdfgnxbpd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gyqynjbkv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gbgwbdvkf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ggasxrumq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gzrnujojp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gqizehbww.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gdzsplova.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gwiypktmn.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/ghmlkenmb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/ggjdmwaco.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfohgnlek.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glssivwuw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggslgmsnf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gegltgvcp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gpeftxemt.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvswhllav.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkzhcctyg.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gqrcgjjbz.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyrlubgtm.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/galeqbmyo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvgiwksaq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtoegzfva.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gpxjcyrbn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkjichzdi.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkbztrnds.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzwinfiku.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gaxhbixgh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gogzsysby.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gfuogsyii.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gzzxaxcyy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gomjbxnrc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwvcfnhrl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gjyajgvaj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gzdiaojkn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gerjyfsbh.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gylkhijhs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gdnatkiyi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gxmsumwwu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gfyqzhmhz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/glovgerah.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gndzwkycs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gxxyyicoj.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gikcktimr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gypdjzkuf.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gzzpmfocb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnlhkylwz.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvlwpgsqy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gnnlazqlo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gjkclryxh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gweaxusku.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gzmxqqvlq.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gabdjasrq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gcjmlazgl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gkkhnhnyp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpvttzmhr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzbonqkwk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggxulldch.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gscmxpenl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gojirnwld.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ginycsjgd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvmkzmeeq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjqerjmmi.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gdqmtwzur.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gialsdgux.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtdstxkwp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjufqcpgi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gkdickhrz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/giasvzpxi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/grvoxwsor.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ganculjdf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gcnsvorbb.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gnlqstcmi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gmjdpyowo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gkxaxnans.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gqeexpdjs.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gqholtsvu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gteoknhyv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gfdlaiwtm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gtrnkahcm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gufdvylqw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvxbgjpdf.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gzixiwgkh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpomgkmku.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gmcuozrac.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gmhpjfkld.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gxtznvnch.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gzjvpmfio.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gxluegvmr.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwwazlztq.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gzqccjxbe.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gwixxrojv.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gqqgialae.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gdiscskku.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gtclxgksy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gjatlzhos.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwqwmqjvs.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gjypwjveg.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gzfmjnels.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/ggcvfseoy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzcdubani.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/ggfmunbeo.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gcswcvtal.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gfmtwtwyl.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gxgrfnfkj.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gmhctygky.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvbpytexa.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gsfcnhhue.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gosmtjyye.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gdbcmajwo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ghmgvwgvl.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gfrpdagzz.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gakigujea.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gzalmpgeb.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gmghudfbe.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ghluyfjei.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gkktcusum.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gqjabguld.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gooqiebxs.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gflhpsxoq.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/ggwamohke.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gyzgwzgiz.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gprakkphf.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ghyehmyki.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grqlvolob.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gkudhvphb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/glruqsqlb.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/glfjovsgt.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gaazigndo.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gudpxwstp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gfpwrkgfv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/grghffxdf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/govybtawz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gqkkynzfw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gsvkjcdxj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gwioaokao.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/ggbdxydhh.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gdmbtllya.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gwfevwgyc.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gystdzxat.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gujvkbsjc.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gaeuvxdkr.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gaaupxbih.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/ggyjadwhe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/ghqsltorw.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gngkohznl.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gksgahehk.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gbrjbalst.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gxtnowbux.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gkygezgub.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gpbbdcdfe.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gdesaomvx.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gbxsanxrz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gzmjefxuu.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gdsqndalo.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gkognabrf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gufmwrzjh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gifrllwri.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/ggbnraxhp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gphtmivzt.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gvopzlqww.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gjwrnqajo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/ggtoklayk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/ghmxkjmqj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gontcqvvf.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/grzksnngy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gwvfydvmc.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gzetjvixf.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gtfjyizjb.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gyjhsmtav.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gezirlscb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gbidtjsby.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghaeagscb.sHtML


<!-- 参考信息 -->