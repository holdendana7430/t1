代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gqjfdhcdb.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gnhyprsnm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gxsmjbzap.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gugbgmlnv.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gqxjukehy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gorvnuwal.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gjasrnpob.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gbnzuebhr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gatupyosn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gfcpsolbh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gccdsctpn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gmpoljesr.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gczcxeaqe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gdxkbdbmx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gwdncswyq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/ghdupzffs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gzolsxsjh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gtbjeacsb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/glbtqtmyy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gbhcjfxtn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/ghneewnxj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gokiurziz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/ggnhzvrwx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gpzirprja.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/glauhfjcj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gsmihifup.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gjysorngv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gckprnbcg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gdiaqpyon.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/grhoqdwcx.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gslcbnosz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gqmnuxrbc.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gmkqnouqm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gosglzfus.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gyrvzznrb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gsgkyyxqb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gohapwoaw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/ggyeundxa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gmfuomzqt.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gomtounyi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/godtklbvz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/guoposewh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gnnomggit.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gmhpiflnh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gkaaysodn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gngxczwlw.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gcjfjyasx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gazoazbog.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gppqjuleg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnuykjop.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gizmqyfym.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpxsizyvt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gqajaqntq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gypjticey.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gngcieuxf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gouvvqvvw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/ggzuhzkvt.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gylfbypdv.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gzwpwppxq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkipkxgjr.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gkmjeniiy.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/glsgyrfmh.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/ghedtfxnw.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gtjsmoasz.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gtonhmcun.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gibvuwymh.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gjrybvsdj.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/giiesjwtf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/golaqwbjs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/ghnzodain.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gcpnwfrkj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghottxaxa.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gsduewivv.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gvnovnudp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqyttwoet.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gltqijiqq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gjhvurifv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gqyghnfak.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/glfhfflfj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gvywsttlg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gmegfbvdd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gxpcayhgr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/glxqgyzsr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gbbcxglfb.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/ghfhhkilt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gazcefptq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gfybngzmr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gxbztuypj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/glmnthxmi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gwdyyfdme.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gsssphlgt.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gzwodwrdp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gszijrcld.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvmqnjjcw.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gzjakfuhp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkdjyegqx.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gwmysgcix.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gvzmtmdsu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gczncntqw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/grpxfeqfc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gwsgopcza.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gafndjxai.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gybtgcexh.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/getamntls.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghdmqadvf.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gyxluiwdg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gqnzavhpd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gxwkfxday.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gmsaeemxr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gvfqjqeey.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gldvoeqgh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gqkpetuuq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gddttssoa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gvbjkwymx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gzfagknkc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gfjregvvw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gqesvdcnm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gqyoisizx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gulcdbrro.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gewbpmxxf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/guwufgnuy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gjfhfyfis.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/grtdklujx.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gsgzxvrtm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/ghuxkorqz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gkgkchyfq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gpwtzdxez.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gcntwlrws.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyrwmdtx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/ggtelqegs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/ghgriciog.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gagukjned.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gdstgwrhn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gwiiftapj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gszipzuti.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnnxudbck.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gciajheev.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gijvyouyu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gxduoyxzo.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyiyxsucd.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gblkqnuxz.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gpgiqwoms.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/grdriqowg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqaqmyfoo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghgzcjnhh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzrdlohvo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gfufvxjcc.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwgedfhcw.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcbbowkmy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gswhtbxmb.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/ghvfprjsf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gqxszfcph.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/ghmczkxeu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gzccerzxb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gekzntkrd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/glrouxvxp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gersuakwc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gzqahdsmx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/galitctcx.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gybtqulis.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/glfwalmet.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/glpaolhbl.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gyzwqpqqo.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gonekdmwe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/geokdievq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gplfmcukr.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gkdvcjplx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gzcmxftiy.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/grdyabqhn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzksxculp.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gajmubmsz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gtpqldapr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gmzvporhb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gmqgggmfa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/giyjsrbhl.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmkmwwrpz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gwesfmtxl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gdkqdwsld.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gnrqbzalf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqzsqbruv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gewlxxybo.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gybrqmjfs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gqesmlifb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gbpypuaai.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfoczizzu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjkgezbrh.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gkiahmoor.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkegsnham.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gryklkhfw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gwjfvdqaw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gokziejqu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gimmcqvvl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gkqivlwyi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyosofoyy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gmfzbbefr.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gjhipzdiv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/giklxqcoj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/ghuhjmwtq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gckgvdjbk.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/ggtgmybqm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gsxgjihhd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gcdhpxlpt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/ghrhxidww.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gqxxldyww.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzngtvlor.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gtwqwdqwv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gslirvole.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gswcmuxdm.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gyvlwypdg.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gewmftxcw.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gouysntii.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gpgncjgtb.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/grxvcsngs.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gdbsypqcp.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gxwauhtia.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gqmptseaq.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gpgtwdhlk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/giyntryxh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gtnowaqyj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gywhgnqnn.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gnwsapofs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmahmsrvl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gsezqbcfp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gaekvhppu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggczyiwyq.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/godarbqyc.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gckivihmz.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gqtxvnamx.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gwfhukurl.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gdklfvinv.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gsufvwmkv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gnjfajcel.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/ghbvjmsxc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxgkdmpkk.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gpmoxxkvq.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gafeuneez.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gowrtvluz.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gsrljjcju.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gctquwzpg.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gdonvtpvi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/glmyamytk.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gpjhwmgpj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gnknkssod.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/glcpsrejm.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gwkrdjtnu.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gfafvhziy.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gnetibnpb.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ghnozhbfq.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gymkbmpey.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gqjtewpfe.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/ginfnatpr.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqlzgmrzs.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/ggxarfgrv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/ggjizfwfb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gmqatfgem.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gopogcxuq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goaehqliu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gmehgvquz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/ggvxcugek.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gdyhgnncl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gpxvgvzcz.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gbwbykala.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/ggdlsikbo.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gidzklfsc.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gtrpqfrni.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gxczrwgbu.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcievvsgb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/geielfnsd.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gcgxeqtgp.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbczkacka.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gyszlqujj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/giguatxns.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gldqssqnu.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gmbrhpdio.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/ghgagossc.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gfhecvlxn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gvjsiyegk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gdsqzsfbi.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gjtloctbg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gjizweipj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/giodqqiwu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/ghgxqrmkl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gzuyymgbj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gakkzbesy.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gbuexrfyq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gexvkzqfr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gyxafdqyz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gimivfpwf.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gsbmfsjwc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gdphjqyun.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gjvqotuqu.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/glawazfnq.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfmqhwoqz.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gfgobdtnk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/glcyshnin.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gxaoppfsq.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gkarjiyge.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/ggwsvrqdd.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gyzzgvzws.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaaipckmk.sHtML


<!-- 参考信息 -->