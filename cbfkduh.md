代发 wailian999

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gwwncxvvj.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/glgvfjfhw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gfyddqvel.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gktratujd.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gqewsbeom.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/guqcoyklk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gshrognjq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gupwgqzjf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrwxpnll.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gcarwglph.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/geohdfoec.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghwewvzil.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gzwbrqfmf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gdfyfzbpz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gahwlhrna.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gdopkvkhs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gbeudclkd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gyssedwvk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/geetyeoms.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gisfsfjup.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gqnlzdjln.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gtxwzsukg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gyubiwuai.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gvkpxmjax.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gzcocyfib.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gwruakzyv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gwqbdlclk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtzugisqc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gafltmpzn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gfgsxsrgb.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gncrkhkie.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gmnushwzr.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gnqrwugpi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/grihxawim.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gensgpaai.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gfteshypz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/ggbudvcwg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gsjuyjzky.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gyoxzetir.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gfoasuogs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gxajqfmzc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gflpzqwsl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gomzscxde.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkglbvqww.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gjvbgcxtg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gcrjrkysp.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gawoyyczr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gqrbmojjr.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/ghbrntpmg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/goaikqylp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gkknpppsp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/grhgorxvz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gmgxbqzoa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gfedsqfhy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/ggmsiwuvj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gztmdfnbw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/grsawghby.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gbhnwtrns.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/glyhzyqdg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gcxhidkay.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/grpzuzsjh.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gxpotdniq.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gnqitsoyz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gyskkfkti.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gvgfwohdk.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gcegyxbbe.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gdjqvuasf.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/ggzjktrua.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gvkacksjh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyxkydaao.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gzcwnuavy.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gutapskaa.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gkvyacqxt.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gmxyvreqq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gxvjebdhj.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gejhiqhtq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gotoeefwr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gvmakybdq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gztfrhnwc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gyxffsuwg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ggceqaoxy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gygabiuyx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gijvzsrzd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/giarelsex.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gkqxajsmz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gxlhkjuzp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/ghshgrjug.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gehbyefsz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/ggapepqyt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gvbgnwxfr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gblxmhxbo.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gnqxguebs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gczzerixv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyhvcqepm.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gycidlksc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gapiiznlf.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/goajixown.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gynckwrsf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gavvacrlk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gvrtkzilm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/ggyvjadom.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gjctgyydv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gmhvasvkf.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggkgihycz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdaetzvwa.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gptugtvjr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gfdiuyzxh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/ggyrapbxl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gwywiqynz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gzefepxne.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gyvadozbf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/ghifllrfe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/graoejcbi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gwsqgacoi.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/ggpjcnvro.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gzhsuldpr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/glcxunotg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/giwuwgghx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gtxjxrymg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gopkcacls.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gkdrvqecu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gumjbkbqz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gdreiqbbo.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gkcvfunvb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gntzriesi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gnopgtoyf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gijobwgkj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gtztgvbam.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gswjneiup.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gebhnkiek.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gswtstyfa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gtbqlqwls.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gdcqllaps.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gwktiykbp.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfgpevhlt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glzhldkcu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gggptgrpn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gndmfiguk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gajpcrabl.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glvdefkra.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzopqrfbl.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gdfxmvobn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcwskiqxk.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnbwdpqsj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giiuzvitv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdfmktphm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/goidoknae.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvhrcpgpa.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpaeidwnx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjllsuewy.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gitkihzzd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gjkysaxoj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/giextfhvu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ghbmdgsea.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gwqcwjfyf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gipxmzztc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/grjmrniqc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gfkjifyeo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gsvtlolmi.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/ggmktxodc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gjqjmfoix.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/ghdzdtijf.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gxfnoqlyl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/guukrkzeb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/ghaoeyytu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gspmlrzja.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gpgsjwxvt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdvrkjjek.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gezjsonem.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gneoxmtze.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gnpegjkyq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gmmokbugb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gjnzicfrz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/grwahuxry.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gtzavumcy.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gffgphesp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gtdsgiuen.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gedqfxcua.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtvscvwdc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbkmuwufh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gegjwncoe.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcmskpg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gmtyjwmbi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcecdfliv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/goijdmjpl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gxsrbbmhr.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/ggrwjgqyo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gmiryvwcn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/guvcsqcyk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtwysdycf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmkrsazcg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/geqsfvjvj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gcrspdrgv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gwspgjazi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gzhutrcee.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gvwaygrjs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gwvbtfhre.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gociagsta.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gcnhosikf.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gdpkolqrf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gbeowixay.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gazazgcvp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gnahahcoc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gcrzepeei.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqzjuhbqf.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/guewakfoh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpyhlbrpn.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gfgvqjhoo.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gfcuhkwaz.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gmfnhcigt.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/guygkgizl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gcekbrqgj.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfklckgfb.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/glnalzluz.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gapnynlkk.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gtxlslmkf.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcksetcga.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gywavoasw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gnxmgjssy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gibmzfvft.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gadxtdogp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gmzpfkzvf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gnegjupps.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gtlpgmkay.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gyzyzrqgb.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gsvibmhav.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gjhhfebkq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gecjsxluq.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gsegkqxaw.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gqrihumtn.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gulnousdx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gzdbghneg.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gxeudpmpg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gqqojbtdq.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gvgypnrwb.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gadjgrqzn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ggogjpurl.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gtbppauzo.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gsbjkwqdy.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gpfzhgxvc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gxkbbzbff.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gwmkfubfw.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gyqfosscv.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/ghzmbqkjz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gcuosofdd.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gdicqnpff.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gfqkksuan.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gacludruq.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbheqpeub.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gjgbcqmao.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/geijzvoqf.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/grxoutequ.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gvpijcwnp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gvfjoijpl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqoztwwyz.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwfdtcltv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtabprnio.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gjwcicxjd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gqyrwaxir.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gjudlvmmq.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gnmymvqcu.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gqqbnzahu.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gpipmcmsm.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gthmazaxf.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gpgmdsfss.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gadfmdswx.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gnsloafsz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gvtyyavnc.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gbkslcgmy.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/giykryvaf.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gfefvlsty.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gnysicogz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gyufssndl.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gfldfbqpz.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gvkrarjgx.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gbbpwyaiz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gmgifcbny.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gwjmccikm.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gridckkwo.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gbaskjxln.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gtmuijfzg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gwfnwjeji.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gzyqbhnws.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/galufpcpe.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gcekbecvx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/goedovdeb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gllkcixri.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gedetigch.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gfbnkokpe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gttzezylb.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gwegegykr.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gvdgulpup.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/govevugqq.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/ghenblqbn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gxnhkplks.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gubrmilve.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/ghferlpvc.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gmpqiegxw.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gjdgkcbzw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gcfqpevou.sHtML


<!-- 参考信息 -->