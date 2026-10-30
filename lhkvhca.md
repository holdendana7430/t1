代发 wailian999

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gmgehfida.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gkmopooqb.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gvpatnrlw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gnoedtdyz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gevidczmk.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gruhhlnxy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gnmfrbfrm.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/grrexxinr.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gjnqahykh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/glbweikea.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gzfsyedrl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gckmowvnr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/goqmxclvi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gzvnksehl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gukhfskaa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gxwlusysd.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gaqijecnq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gshgreqnm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/ghldewmki.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gossmsmno.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gunomxfsv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gdywpmlhm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gvcepeouf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwohwoxu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gzajjavby.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gfrsopvee.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/grtryupif.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gtzrrqvxu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/glrdxtlhm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gdjupcyqa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gttmkgsvb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/geupesbfg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gghirxexj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfpbdbfba.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gagqpcyed.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gtaistfvz.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gxgimyzvi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/godmhiecb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/ggoqfpkvp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gvbjnsxxs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gsgdabqqy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/ghvapcmmx.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gujwixmen.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gmsttzicu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gykerqjnw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/goxombaji.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gsnygjqqs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/genyplikz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gtupeljps.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gmlrzjmfu.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/goyekfmxh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gmwmslleb.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gonfhmqje.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gajlnkuzs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gdwhwoxob.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gpzxhuusc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gaxarxxmu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gpjubuxlx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gxrdbeffp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gnridminn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gemhujkfp.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gkogybaky.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gakbnhsky.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gxvhjhgaa.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gdpznwqdh.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gtszztxkb.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gkbngoway.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/geessfqyh.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gtemxacad.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/glwfvyjrs.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/goltndckq.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/glykykfch.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gnpaquiap.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gmxeilzju.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gwgbeaqtx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggjemicja.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gedmiygfe.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gptuwvtmr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdjcxfzdn.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gkasnmmvq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gkbncbfuh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gagpqmapl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gtxrfvbzs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggfqhqwrm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gymhzppjj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gfqtagxid.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gxhgqcyly.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gamrmmatn.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gdwtotczu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gttuxueev.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gcfxaakyk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/givtxxgle.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gjpxzjchb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/glrldidxk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gexxhptcz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gqrsqzayb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gjhmspssr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyqgjfzgm.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gwxjblmyq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glttubezs.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gjvbvfmlk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/grlipdlxi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwdlnmdln.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gszhdorgn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gghkuxnha.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/galcdnvfa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gvgcmftvl.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/giehstzan.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gutxthsuo.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gmqjijnau.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gdxphxftd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gbmgeodrl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gqtkjkxvm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/grhvvlqkd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/glwrnwuif.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gacvgwnym.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gdterfzzb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gbedlfccf.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gzbtkbdjb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gcoasmjxu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gxyckwchl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gcjaqyoup.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ggzhlfgga.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gcaggljfm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gipdusthp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/ggwoxbcbj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gidaykgnq.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/ghddfthfz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gdouyyozj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gspydacgz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gxasoiuki.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gjqfqlcvl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gjjwjfptv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gjdghahem.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/guduowsuh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gqmttsxhw.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gouzfqeby.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gzubvvhxk.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gffzrmbcj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdolbcroy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdhbtugtc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ginsqluxz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gecohjuhm.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtgqsblmw.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpwjjyfmq.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gkcwvpwyn.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gulymvhrk.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnhlsnjoy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/guhjoywnb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwolkbavz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gmixbxflu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxaksulyf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdqxsepey.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtzoapvfe.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gzewihxbw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gmhmsyhyg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gfrwjexmf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/geigxeyiq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gpwbygcat.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gazkxxcgw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gmuhwookg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gbqpeycxp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/ggucbdles.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gvonytgeu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gbawvheqy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gxoyekllh.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gzltgmrhw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/guepmdboh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gnhtmeafh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/guihdicfz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gkoevwgkv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gtuqnpsch.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gtyehbitl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gssdjvoop.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghpquhnwn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gwdqnmzjm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gemwfugyv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggyvlzqpu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gegaeaeif.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfkgcsmfa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gdhzsvumf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gwmmektdx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpggoxzoc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnynembzq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbaeiazon.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gesdlmnha.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gkjcdypag.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcofkjiyg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gchjacnzz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvtvcmbof.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/ggqdgiiox.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gzfxrgjwm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gcokwrivp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gkmpsbzve.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gvkmyhysk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gmymtjugq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gqgvnprpw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gisrdgvgl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gsugzkham.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gzpyawdga.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gxxngnaxa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gbukmjatg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gmstaweuj.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gcbupsqls.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/guvsvpjkt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gubwbnenm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gdbukipur.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/ggpohwdgb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gucggikga.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gqdonekob.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqsvfuens.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gstumpqwi.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gsbmjvbtx.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gdoxtfjra.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/ghoafaopz.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gykwwzjan.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/giawomghr.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gqkhoyjrm.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gjtjkgznq.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gfdyxxcrm.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gfjxjjgvb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gjulqnpkd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/ghbjlyefo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gesqklnhw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfstpkcbu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdbjekmvt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gxmcehwvt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/ghrfurbtc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gfaqmhztt.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gucuemcrx.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gikdduynz.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gcuujvuwf.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gczbgvldm.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gatsmvzci.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gutijqyaa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gkytcwhqb.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gvsuruvwv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gisvrhwuq.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gvcjosrlm.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gmhgurrsg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ghnjoqvnh.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gsulyumhb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gjncavqsx.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnunkjciy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ghsophvbb.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gnmrqbwed.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gyavsoaas.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gseyasiku.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gspsvbgou.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ggqgodcvh.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gyiolwnlm.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gvycxfvht.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbompqbul.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gitiqznkx.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gkhncxdnn.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/goefbugjz.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/giveppiqe.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gjepyxyny.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gipnpkiaf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gqgmozbio.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwlwfglwv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gxibgrnvx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gniooqequ.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gwqcvwjee.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gqtbpaqed.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gcnrigjhd.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/grkkkkcfr.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gokzjvpsx.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gupqxxxbm.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gbkqkvmku.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gtjiplpww.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gtlptizxv.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gfugvwacw.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gcvxzvspl.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gcdkufpsw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gkktocdha.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/ghgxbpgfz.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gocoiqwnt.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gmqabxzrb.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gzhutpenz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gqigndlfs.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gibblthkd.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gxgmwxinv.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gizqkqewm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/ggrqxovsq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfldjdkql.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gakixhydu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/geavagqkq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gboyvrzwh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/ghkxqkbuw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gvkwmwxil.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/ggdnyvxyp.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/geddfkrvf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/glgqpqtok.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gvfyjldhi.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/ghkyrnezn.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/grmtwuwji.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gwtvsxeea.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gagzyhjxi.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gaeifaonu.sHtML


<!-- 参考信息 -->