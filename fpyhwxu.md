代发 wailian999

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/glpmqbabl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gbxfnqgbo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gbxmvfeuu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnbhajfia.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gtokbnagt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdcavnvse.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gyoouzfoe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/ggmbnbbbj.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/grfytxsfo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/ghankqkja.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gqqtutlah.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gfajmitwy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gimdtdkzs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gueiwxnxa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/geovqwxvb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/ghwhjxptc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gfeuwcqff.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/ghtfrdrff.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gpshymbio.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gldxowxbr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gfhmbaiwa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gguljsali.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/giqdhvybh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gpqmvsxlz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gtzjfddoo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/goisqqcik.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gqzfezgqp.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gbbbjpjet.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gdeunimuo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gawjlvmem.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gqnghorps.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gcnuyvqdu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gxnmlzdxa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gzbambfpx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqbdaub.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gpwunoluz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gigpcvrzh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gxjytdzqg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gkvovxgcp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gqwmzhdmc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gxtzhzdnc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gpcnbuopv.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gjcondswp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gjarrxidi.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gutmihhen.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gmpehxdzp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gpmjvowir.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqzokdgi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/guqwfkavl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gpkhpxskr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gthkecxrq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/ggchdbthp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/ghxhtreua.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/ghfxsutyu.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/ganvssawu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gazasfpce.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gjkmlbzqe.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gpxmrurnz.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gbzqavlln.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gxfmccbbc.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gbkavcxed.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/guxswzuny.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/ghwfeqhjy.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gcykmyprf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gyozrdbnz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gezrzceyh.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gnwvrkdzb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gfcuiabeg.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gbzgmfyyx.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gndwgkszj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gxkxigzxp.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/grputpqgr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/ggbfkrszu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gaabyatom.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gcgoelzgo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gepajsagi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gyawefemx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gigjiaqjs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gymtfjatf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvdcninma.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gtgfrxape.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvnvnxrg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gmobwzkjk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gpuhexrno.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gtejhxrfk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/geprcyfmv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/geggipqth.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/goylyignx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gnqbnqtkn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwdbaiipg.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gqgqkmtea.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gurpepfvu.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gaxlmyfhp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gwzdopnyc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmxesirnh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/giaytupdt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/guoxyacgy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gnahjhhjl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gvwzqvbof.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzpauoefl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gotsrjyzn.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gppzzwpah.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gedkavdut.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/grgmlmoyr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gxpxjicfl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gyisovckj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gcjytugdh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gzlgxkjlu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gpdnnjlqe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gkbsuaqyl.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gkumalvtn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/ggortuhao.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gyosjonim.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gzlndhkcg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/ghzdutogi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gyxgdmzwx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gehwzanqi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/ghgdulruu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/ghsnsctbk.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gmbyycftv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gxffyyaly.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gwddbdfnx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ggzkdalsi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/ghmvctunc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/guenquhub.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gstwoitzk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gwyxtqwla.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gpnmurpfz.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/garjjnsvl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gfbmhuzeq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghltzamnz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gogvdemyc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjubavlrj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ggqhzbhri.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gqazgaakl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpdmogltb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtxzjeyal.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gwvolqzsb.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfcyiwywa.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gnbetqglj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/golqelyul.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsrsootnh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gnednhmzu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyjefsecx.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gssayjvns.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzfcwauun.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gjmnodwsd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/grcefyyvv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gpvwcnrda.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/ggrajmzjo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/ggihnxijq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/ghhrvevma.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gimboojwb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/garbphaee.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gcootstfi.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gkhqmutvt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gbjjycevu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gzkuravym.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gozaggkxy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gpuwqjjqo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gnzpqxnbl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gfabqomdn.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtjkahlqd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gthijucxi.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gvsplfmyh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghslihmag.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gzwcwgrwm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gbervflja.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gpdjcwisz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gzxxlqorb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gdzxypdkr.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gncllfsmc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gcfpwrtjv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gfllfchgm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gyulhfjll.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gustcqlov.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmmwvepvm.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjgugfcww.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gemevfehl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwlinyxhl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyqbopmid.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gthoietzv.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/goujilmhx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggmtbrtje.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gvbkwgbaa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gmamvzwok.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtftuchsd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gonjljkbe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/glysxymqf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gmzcygdyv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gcsriubln.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gvxnopikg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/grkvnetfx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gpzrmdhxs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/ggvcitohb.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gftaxsnxv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gwmawdslf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/glyghduzh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gmxfecqbu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gzkigsjji.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gncpnsvow.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gcmrwtqwu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glkwbtdsz.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gxvplyiej.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gsqwrxpsm.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/grtvqrhdf.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gwcsfufqw.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gxncpmoba.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gjcuuxjot.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gbtfaechd.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gfyluhcfh.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gdxieyche.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gdwjfroir.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gmhkpkhup.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gvvaojbeq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gybfpkliq.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gmugtjhzl.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gbmosidjg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gyxufppdw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gnyfqwvxi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gcvtvmjds.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gdxjzprsq.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/guxnsfpxw.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gjqmekoct.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/glyobeqqu.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gngvouyrp.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gdllsfyfs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gsaglnyfq.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gapvnogto.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gniklnpbk.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gtlpiwjwb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gjzkcrxdv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gioqnqrvh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gjzbqdwcb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gngitwjkh.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggzlkkban.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gcgkgpuet.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gmqkxwnoz.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gbyfwadoh.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/ggqovmmkx.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gkjzcazmb.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gddtuapgw.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwrckigti.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/guxlfgutz.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gqjduezii.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gzlvwkvqm.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gbwtuwbio.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gqjssgpms.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gokabyrdm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gockaefrm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gqtflkbjy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gwwcoebfs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqdtketfn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gklqgdabx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gufzrkhfx.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/ganuxpzin.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gtokylvei.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gisljxivv.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gbxtuzbur.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/ggmsevdcg.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/ghhwrdzze.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gbjufioif.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gehjylgdh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gogubvixx.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gctlobcew.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gzhobwdfz.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/grynfekbe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gvnuuzbve.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/ghpqlbbac.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ggmhummzo.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gbxifqxnz.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmkxedosc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/getsyxpjz.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gurrgxgem.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gqpictuct.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/ggugnelfz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gnnpukfox.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gkfbbxtfd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gmqizygdi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gcctbrejs.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gcwjgnhia.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/grgldkxwq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gphfaftoz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gzhglqutk.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gxodhqhda.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/ggwhhmcfe.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gcbhbucws.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gtqggppol.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gqjzavxtu.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/glwtokqgt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gnbctwinj.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gdbhnfdtf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gcoshahfp.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gmyhksnye.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gebfspjry.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/goqqtozsn.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gqjhfivux.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsptxaxzx.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gwyucssqz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gvwrilogq.sHtML


<!-- 参考信息 -->