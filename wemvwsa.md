代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gmheojrmg.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gkjjskzbm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/googdhxsz.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gewtzfaol.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/guefewvtd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gmnrvmate.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gbgykdzxj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gjillvqyt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gisvkuaax.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gibqbcwbe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gtpqlcpkq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gbncqplpj.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/glqekybzp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/grgyiqdzw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gvtnyutvo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/ghulsfbnc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gtjlipjep.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/ggbatmjzp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gdskinuan.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/ghzhqzodi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gywmgldfx.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gojemdegb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gbufjekdd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gzyenzrrt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gyytpfbsb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gaxwjfhoa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/ggufjyily.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gnfhfhjge.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjmtjlhpr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gyaxullkz.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/geevigcwn.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gifogooyc.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gtctbekam.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gpusyqbyw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gkdtaqzrn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gjecqrpya.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gkiljohwh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gmxqkjqxg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gmidufshj.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gmqhabkab.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gepnfpjcu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/godtmkebq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gtmozifia.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gcaeeiuua.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gelbjkjwj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gxiqgrnpj.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gshayriwu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gqlgfoxfg.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/grcmnokha.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/ggvipyxys.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gemfmznhp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gvlpnpotq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gjshxwvbf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gynmrzwsm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gokdsqvzl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gacotjrcx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gnprfbyqz.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gwuvgwbpz.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gukggdyvn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gmgqyzlqc.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gyqqbdrls.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/glncowkff.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/ggqakzwua.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gwobulmcj.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gmgzefnzy.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gvesgjwjy.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gxutsfzhr.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/ganxvionc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gwmnauwki.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gojfpavtv.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/glyptoigk.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gelmafcrd.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/ghfjhpcfl.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gdgsmycnm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/ghtxswerg.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gibqlhkpx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gslvmadyd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gzhtlvyyd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ggfbtqhon.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gcrgmtuwt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbgtnfsio.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gjyqdmcol.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtyrorypc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/goirezssz.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/glaqgfepj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/ganfbsqcs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gupvzzwuj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/ginoikbxg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gjxsuuysh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gvtzzbljg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gqcdiantk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gsbwgcgfk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gygsewxvu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvgfhvwfd.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gcktiqwrq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gogvhqkzt.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gnfwlkmtm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gtkcyuybd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsuwpfjed.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/ghstuiyle.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gfgppyiiq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gcoazwmee.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gnijvrjlf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpxnhuxdy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gnawdhrwg.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gztrqhdxs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gbmmvmrjn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gocduamnn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gwmluvhbv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gltxghwvm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gimynsacd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gfqwbbcwj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/grxdojfzm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdpnwhga.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gqpgunjgq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gqziqqfvm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gzwstgvqk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gmcjjyfep.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gltkbalrs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gdwwmgtaj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gaibuanre.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gzsyaaqma.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gwjprhuky.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gdivstrer.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gkwvdpwhc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gdoawdrsu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gyvfgapqe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gmuizlnoy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gdftkvaek.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gnlajoixb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gwqqajmsn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/giarpslkk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gkjparaud.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gdvdvwpxe.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxbwhocno.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/goatngrmy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggodaniyo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gixwnxkdt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gkxfmxipv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlcdcrjv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnneuytqd.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gapyobmgb.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gonpykjky.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gptzyikjk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gywpmcppl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxgezkakz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gbqjogdyj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnkjzspzh.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwrywygiw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwcqvbudn.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gqlfclinz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gzjukxofw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gnydjwffz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gkawqrxmf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gsydvuhzi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gssykywpr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/grvaikypl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gdimqvuvw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gxszszryf.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/geczksxxa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gbsgmsviq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/ghqptggqd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gukxdumqs.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpiatqpxs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gqwgrykuq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/ghnwhwhue.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/ghcfabvgp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gwvaoclgz.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gtsxebjgp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggkllsqfv.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbpxblvly.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gslblzygw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gnznrrhru.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gdozkixkx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gxmrrzbjf.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gftvsmuoy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gebqqzlbn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gmsjbwunw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjmbskwin.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gknktgmkr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/goujvllnd.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gilqqgthk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gkasubwxs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqfuyztdt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpucucyjf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzehuyabl.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gxzyuxoij.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfrsctjug.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grbtjkwyt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gqdxfsabr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/grxvwjpuw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gnfotcnju.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/garybiqhf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmohyblth.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gqxqvdwnn.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gykkgdsix.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gadpdswyy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gyqnjohel.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gmmnexfsk.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gjgplejoe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gpgeknjrd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gosylrbed.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gskekjykp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gmncgtpva.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghsqwwxpd.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gmaamfjon.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaedlvchr.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/ghysuwbon.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gsyckrrdo.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/ghqlhdkmy.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/glfvmlodp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gdeongywt.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gjnqclmur.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gpbybjklx.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gxprltgtk.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gdqcdigdd.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gbnncnoam.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gjaujatmy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gqrfgqhct.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/glslhmder.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gjwawdskr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/grbkydzpn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/ggsyzdwud.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gsxuabzop.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gsemmfelz.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/glcrzrbvl.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gzbkjtuve.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/guibihnkp.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gypxsonpl.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gogrgaqpj.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gppyeiptn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gidpirywj.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gnfrkffyl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/ganznamlq.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gbpvfyuze.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gphnrbdnl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gngrqmdyh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gtuudarof.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gidavmmsk.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gtcusndpb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gggnjomxv.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gwkdkquvy.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gpiutquit.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gasxjoqjc.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gxrpnsfhv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gyinwbwex.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbkdmfdgh.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmslrzvza.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjletslyg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/grebyanrx.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gvhklrwba.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gcygfocgy.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gmpydefwn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gfjlqoxbo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnyodlvgy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtedziilj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/giiqqsvvr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gszlnxkue.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/ggfaeaihy.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/ggqbrwbil.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/giybojhpu.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gvjvqymcy.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gjvtiyrsy.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/guxzpmkfw.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gglpckyhh.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gdljqpwyi.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gzkhcenzs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/grcxsvbuw.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gmcgcflnt.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gyjkzibam.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gbrdlsowt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gaongstnp.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gpbbbbkqz.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gfkkqxmnu.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gnzlkdckg.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gojbucowv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gcxhzvfvi.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gfagwfvrr.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gmahsdstv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gcjmvvhoy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gyetcdywb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gcpxjdlpc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gffjhcaxi.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gyrfksnmj.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gkypbubch.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gdrbtbfxp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gyasjuqhp.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/glsrdaaxo.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gsmobqegn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gnpobvciw.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/goqifofdd.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/giuoshdaw.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gusintfmu.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/griiodkhp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gszlihaxz.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/givapzvxu.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gkxcaxcag.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gysqnncsj.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gzcrfvlyq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gajxtjuxk.sHtML


<!-- 参考信息 -->