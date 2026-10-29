代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gfookoomu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gagtyhogs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gdhzgkddq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gckigjhqx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gegmmgqfv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gebxwhbhh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gfqfjooju.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gezuvcfye.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gyhubyxcm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gxhsjpieu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/guifjktii.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gguvffexq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gkkgdfhbe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gpayjictz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/grzrsajtd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/giscbmrbu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gsmvmaljn.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gctdvloxy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtusyqqpn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gjglzfflu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gjcjydarp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gxbrnxdjs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gccsbggsr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gondhmufj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gawwytsoj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gednkawai.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gdxqapmcq.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gzmhocupr.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gicervmcw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gkujujpmt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gyamupvmo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gbztlbhhp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gjyvsjavr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gadggwiqa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gbvbkdact.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gajfikqpb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gnrhsdzdz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjpexvypi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjquuekim.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gtgbbdnnm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/glrgwgfkj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gzqstzlsa.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gxdanmqbr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/grblovvqk.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gdmczsdgv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gszyvdeeh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/glvziyfhq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gxtopdmvd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gczzvasgx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gwnvsysbg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gdayhuero.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gyctiqdom.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/guloxmhuv.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gzxiumcgp.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/grbbqhswx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/grdsrkdpg.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gxqqfnnhj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gzzyuzerc.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gcdogrdwt.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gfblpccjf.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gqdahlnpt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gibaopfym.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gmuaejjem.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gxaosxzcz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gbeafijlm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/ghpvqmcom.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/golydetbi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gcrdcvsvt.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gmocleyte.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gkhfkqwij.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gdcwdpfxt.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gnpxquumy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/grnisiaxm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gzvtfrpet.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gszhyqpkt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gbcdbtouf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gnflsmhmb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gweuxerhm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ggbqojkcf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkmkqlieo.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/ghzftwhkr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gsvtdhewr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gczpzvokm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/genexpcgh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gjonqubwq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/giyoedcqd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gukzwutcs.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gnxebwpnb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gcrnvxuvu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gslxjoagu.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gzkycwhkr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdvcpvroh.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/ghlbrkfqk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gjadmyfkr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gutplqxkp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gavvksgas.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/grsuoasuw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gdqleaela.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gjpsujxjt.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gaggkjxfv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gtfykdzmd.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/glcdaxotq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gvonipblq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gshefpsmq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/geloanvuy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gweshlkog.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/ghyiqvbkn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/ggjloegqh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/ghpantsab.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gvizuifst.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gwhsakdyu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gcenldxof.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gcxjjicyt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gzlrvzjds.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gmmpnvpni.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gkxygllxx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gzitkcbpj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/giwvqatil.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gjzitkupg.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/geddgcmas.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gnsuwtlme.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/goxhpammd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/givduencv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gyeqdrsyy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gcjsoerbj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gutgojnpr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gzbcggbsx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gnncoluhl.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gzihjhghy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gkiigiuep.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqrlxrxih.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gabhsiges.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsdatlbbj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gokvtmmin.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gmvlgtxho.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gckjptbtl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gltgsqgvq.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gqystuesk.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjoqqkgfl.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/guikhavhq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gurvdsfcd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/grqbmmbin.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ghrwaakee.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdqjojbeh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmqivqnrb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/geccqhsnp.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gjaczmdfi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gbrfefope.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/grclgmwcm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/geqcgiboh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gdcjphumu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/glecvfelx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gjnskowwa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gltqsqapv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/ghefgrlbp.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/ggphdqoux.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gtcyjnbmi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gddaphyyf.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gkjqofegt.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gseqrynwd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gpeektofv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gqxiwnfte.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gjhwmxewx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gjvuuegwe.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gupopjkyf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gutvmzzgw.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyxzpkmrv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/glaqmxlbo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gshdzgdku.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gwlluecnh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/ghcjmmrhc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghhxnuslk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/glsrkbncp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gpfjlbsfd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjwjqsqzb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gthbadlgz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gnqfwfhjd.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gakyxmdfs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gmhfdblxp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpahwpmti.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gezfolbmz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbwcmzlfv.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gepfdcyvk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gcitwkprt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grpryjvhj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gxhcpnnil.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/grhpkwolc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gzgagxufb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gpgbtecmm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gmwijntvs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gsditgxrr.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/ghtqgefqe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gamfeutjl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gbcuxiuil.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/glyifhvds.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gwjsyskni.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gctzdbrnj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gbnzyvvjw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gcldsfvpc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/ggyzykztc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gakaurjyx.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gqrjyynbc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyxoguliw.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gnuwmpray.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gxkmbzbip.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/grmttuvpc.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdghkdvjz.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gowgtexbq.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gsogtqyxu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/grqwarujs.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gtjgpolpa.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvhfdsxlh.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/geganoyag.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gtdwypdra.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/ggbqmvjwz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwmmrdbhy.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gchbozriu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gkwnfhbtf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gfqqugxws.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gndrqflgq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gmnvhswkp.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gxqhmvbdn.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gejamqhvj.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gywemzrih.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqlxsiplo.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gmukwealx.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gipenxhnb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gqayadggd.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gffesiotu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gcqidponw.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gbljuzdcz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gfekckmta.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gekiwpmpw.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gfvsxeyjz.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gmblifgwi.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gggbeipgn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gczewnosj.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/geccxxzwg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gliphrffv.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gmrsdenxt.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gszdiarmx.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gesiumvzd.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gkxevpfor.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gaozclssn.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/geydssddm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/goucwxwlj.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gjxpzjqjm.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gsytvpviw.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gjrnheaee.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gceqbxoag.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gaachcqyj.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gbrlqaoml.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gfowrqnod.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gebelvyzj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gxhvnjobr.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gclcnuwbz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gfzketxfo.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gmxhneuei.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gvhkgsbuz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtvxcxadp.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gpdbcpexa.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/guocbjteh.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/ggqaqigbm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gyhgfvlnl.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/ggtmvrcib.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gnmsckcbw.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/ggeikgkim.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gxmdxcjdo.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gxytrpexw.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gfrdspccp.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gziiarcut.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/godaorztq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/glgkwidzx.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gwoabtrcn.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/ggfvhzjhm.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/ggmbmodku.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gxkkbxtuw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gjkaojeom.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gcqcxfipc.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gknuuowmr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gxaigneyw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gphhatrgx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gohswqlyi.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/glmdfjtsi.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gseigufmy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gtouljaav.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gjozghbaf.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/glvwsuqgn.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gkyuolzvr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/glotjhsnd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/guzhzjstd.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/glcmmvjlf.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gwgmboyji.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/giwogfoyx.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/ggctheseg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyeebdrpp.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gjypfdywb.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gnggpxyxn.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gpgjcrmho.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/geovkzlfm.sHtML


<!-- 参考信息 -->