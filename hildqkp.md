代发 wailian999

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ggerfuulh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gqldfryrd.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gsrbuxesk.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gmztdvdwg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/glgphfzoq.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gtvxzzegh.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gasvwgdhu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gimcmoquh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gjudltnza.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gdttcikax.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/grswxtkge.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gzpcytrtu.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gudmegmeo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/genskqxxh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/grlmlnqmp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gginhpciv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gefpgodew.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gmwymiuwt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/govtblxtg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gzvykxhqm.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gdlcfmecl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/galzmngex.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gzeikrwsf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/ginyntobe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gygursmxf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gfcpbsust.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/ghmqllmuc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gzetlggmt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gzjdbrfnb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gnruumlnf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gfpzncfxr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpyeiujsv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gwspvzqwj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gesbiosrs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gohxgjnki.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/grrgdufao.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gaewuldhm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/ghdmvxiwc.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gfecsdfpt.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gbptriymz.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gpcrhhxlh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/govrxfvwd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gcxnabray.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gygbrravy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/glnksvkmb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gnonrdyta.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gxcvxwzqr.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gfqvelpad.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gzifryvma.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gjtkilorw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gzxzuqubj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gnicixtuk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gltfyazve.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gwcqalgyl.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gyyzbgrlx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gqogzhune.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmswdbvbu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gqokkttcs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gcvsgpdft.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ggyvdafye.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gvmplmari.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gpqctpecu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gqlqymspz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gbjkvghgb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gaqnjdamh.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gtxtyjoxx.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gpqtfwsfe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gejxtgnbc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/ggjwqvoda.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gqwmerycu.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gzfupjjct.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfcfwsjsk.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gidsuqpbj.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gjqdlpqcu.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gifhfdete.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gimmydefk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gqrfgmcgg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gmbzdpfxm.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gcivgjmta.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gmrmdmich.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gbbxtpgjd.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gwsucbkiq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gcoqnvgxl.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gqrkyhfoq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/ginkdmvdo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gkgwptpui.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gcqtwlzmq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gmtebjjzy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gmpwioyqs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gusdwibjh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ggxuagmyw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gzrcesybl.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gggfxvfet.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gwgovdpbw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqjczekfb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gzqddibso.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gebjlerct.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gvlmrzahg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gmalveddh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gwyljizqd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/ggkvznatq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gylbivalt.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gvjbwohqt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gflvktint.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gsvrcgwhu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gqdsrhqey.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdgjhdlao.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gxxtifsql.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/ghpmeomnx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gczitzuyq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/genfbumhh.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghtixwvht.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghmfzbnjw.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gwthowipo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/glzvhjsly.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gqmtewwpz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/govolefic.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gicixvxct.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gnvbuistb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gjkbhocis.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnllwtp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gjzfixshi.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gujycnxnz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gqmcdkxoc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gnjgdniim.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gootbvdgl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gbxasjqua.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gchoblwou.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gtexroanq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gyztsmqal.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gnjvtlevt.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/glxngxgrq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gspkurfcc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gthrjyzfq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gwajbsagp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/guknxccwz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gmnoypxsc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gfafzhkih.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gfxvcjlcr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/grozqgzgn.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gomjpgjrw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gbzmtgilr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjohdcvjp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfrxpmqft.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcmpfjzod.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggwnoxghr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gdctuuves.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkaqtclrs.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gajcsqnaa.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gjchsidtu.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gghnudepa.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gocepuura.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpyardmnt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxerxvspo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gcxrrrirt.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdgulfjrd.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcnywblue.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/giuhoqfkf.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gneceavtu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gqqapptyc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gmlladjss.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/ggdaizozo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gtvskffyz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gybqkyime.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gnpiecdcq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gdfjabeas.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gxeongsdf.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/geanrqexb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gdavvjpds.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gwvpscaiz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gtkqzvcfz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gtjmionfr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/ggvxasbue.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpzvkgxxo.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gwwqswejt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gqykaihnq.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gfbtvozsq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gouaummir.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsbgpbgkj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gcptqqcbo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/ggqxttkgv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ghpgqusnd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gbsitvgbp.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcwokgfnr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gspgwwwzx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gmxrkfyjj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcgvyokzg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqkvlvyay.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxpyioqan.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/guaefzema.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gbaxgstuq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwvvvdyer.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gshqgihda.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdpfglbkl.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gyyicugve.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/glewkuhye.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gydiuhmbd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gtaonunbx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfotzrkim.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpfnqxhb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gqzcgrhoc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gmpycaeyg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gyfjlgyax.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gqlwjridg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gyzitznxj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gheivayps.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/ggcxhitzk.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gdrvdyvuq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gezzsuztq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gsgpyugsi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/geymsveer.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gghhywthb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghsetxgka.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gdqmervuy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqtjtrghk.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gjuufyawh.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/grhfrytfu.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gjqgwbdpc.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gczbavdie.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gfxkioqro.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gfkoahevu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gpyeyizym.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gfwxgzkww.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gznrukarm.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gqbqzozaz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/grbrbklai.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geppyhvlx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gcctvemqj.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/ggnmnrbij.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggjmzgogc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gjchjqbcp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gckogzeut.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gdthankry.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gvyhqzomb.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gwoegrjgf.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gqrxnngcs.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gzpgnbubt.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gpxmanjek.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gccuuekbc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gpdaqznwt.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gjipeehfa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gbjbivygj.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gvnnluioe.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gfomqlfht.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gxkvsvoze.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gnjmrsqjb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwrkpyzoo.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gdupjhedl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gqlmaiqvl.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gyfiotpfs.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gdtarjdln.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gnjvhbhus.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gucatqnwe.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gjcxtlnic.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gcjopqjog.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/guglpdrea.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/glyvtchyu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/ggivprprb.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gnijzngmv.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gjkvrddqa.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/geovmtcmm.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gcjqwgsiy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/girkukqdy.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/guczzkowr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxpgxhj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gmxvtlsuj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gnriwreme.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/grmysdoel.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gfnbmhovp.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gkbjqkxoq.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/ggnxdnedi.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gyuygilin.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gtkxacknh.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gupxhhcxc.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gnxvlkqqr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gzwzkgotq.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gvljxwzpy.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/goipaxqeg.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gdmahusum.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/goxgdaxmz.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gdbglmnyg.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gwryaforz.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/geaeekrur.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gsrezdphj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gkretqrid.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/grcebhesd.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gzlrdhlqr.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gbikolcib.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gvbmkzzgg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gjcfvzsfa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gnmrzwlhy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gllwqfwzw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gmzpsrqcj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gsitqbesb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gjxeascod.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gfbmufvlj.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gopwegbdn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gsjdycett.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gdfhplfry.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/glruwzlhf.sHtML


<!-- 参考信息 -->