代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gkekfiefy.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/grhehcnyv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gghwzxyzz.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gfladhuiz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gfsxpxyoi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gsntijlwa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gvfrjfwtf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gutuucfnh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gxxylbtnd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gmlwibhiu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gmcputpps.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gdfgnednj.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gqtdstjga.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gjspqwvjx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/ggwqpryzr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gulmpjbdg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkvcciqvb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/goiguqlzg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gzqaywdiy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gffmiwxbk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/garssbmlr.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gygfumjkz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwzycwoz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gojcqpkls.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gagvldhbb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gdqtvqzle.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/giizizkil.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gqafhekyi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gxchylbgi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/grrrxbyuy.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gcfizmylf.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gdahgjtjb.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gphwebopi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ghuiyvdht.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gwwtfddwv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gbequlpth.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/grtfducnu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gtwkklfmw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gpdzgsmlg.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/glfhdlevq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gslwlgqpq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/guokfmkfx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gkqohipru.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gnifmobih.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gayatebli.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gdthyezqf.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gzqzpiugh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gatrxwfub.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gxirswqux.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gkdbehmha.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gqtphbufq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gpgoiccru.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gisasnqmb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gysibhsiy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gjugrybcx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gjfmcabmg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/grllkfhov.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gvivekaqp.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/glpgfrgmn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gqwckjjqb.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gtfaodasd.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gdmwqiuhk.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gquathyqp.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/goblfdeuz.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gwimmzfby.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gfycdizqi.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/giyeamjsa.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gqlbzyqnq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gwbhnylbp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gjtryvlmi.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gtsquylrk.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/grtlyjclp.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/giewbduqq.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gwaecjaky.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gsheayjlh.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/galgurnzq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gapbqmmzf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/grmcyexze.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gaasmayva.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gpkihixvs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjwqewlpd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/glzmkfnsq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gydpfrsjj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gbiekdovx.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gozazxzqj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/grlpfkuhe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gefphonmp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gusvpgmfn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/grqpnpexq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gypmluiud.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gpptfylkq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gkveiaidj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/glafabrwr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giuatjjwc.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gkefwfumx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyyagfhia.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gnqkxayca.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/ghllxrmrz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfrdlzunf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gthrqfivm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjnqsdsby.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gmvjlgkcp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gyluavsjh.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjodtymwe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdooqosif.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gcswmvdpl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gfodiywld.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgnvxpvn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gohmacqsg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gaqefttlr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gesmgcpqr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gccivgmcf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gynrjocug.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/geyqyifkx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gtqfknpoz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/ghemunpqg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gnkbvgtqn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/glvbftrmr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gwnencnpc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/ghhfbjxxo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/ggneczsum.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gllsxgeit.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gyrmbyonx.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gpeimdwbf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gwnbqsrln.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gixultbvq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gccssbikj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbqbjzmoh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gqrbsvkvm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gbguavlhv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gszsmbryl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gekfpyczr.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gatagmlfi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gatrbzawg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsiuxhwgw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsspjuzii.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gitvozkgw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gkpryffgt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gdvotvfiz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guwwotpkc.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcopymgkg.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/grzhadzbt.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/girkhgeme.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwostriay.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/glbugjdie.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqydabszg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gyhbdsetu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geeknbfxv.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gllzrylvk.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/goncmcxxv.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gbxxtkssz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gceawaych.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjofwey.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/grtajktzj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gzpkkffow.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/glszfvdyy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/giskrfgmi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gnwtvwlkn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/glxljfhak.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gyrutrwqi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gnflzzfjx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gqahdrtrc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gcooiqjqt.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gjfyqsaoe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/glfkupqqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/goejiamob.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/grdosvjnw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gtyeslvap.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gajghauzj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gixgevngx.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbetsvlub.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gtyfwxqro.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gkmgkqnud.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gnwzlxxau.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gzactcruj.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guqnvhpau.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gedwirlkn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/girqojkeq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwctvrlmi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwfegzrld.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwrfrkadp.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gamdwpher.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gdakboyek.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzwjzbxru.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjdbztplp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpghiucwf.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gctqdonsu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpxfgahnh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/glnvhaiwh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gncesgumr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtqbtzezl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/glkhslyqg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gojlcmjmh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gqonljwyp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/ghmgcgiqs.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/geaiwrxii.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/geaijblhx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gtbqwupsg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gswsbbgzg.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gbpehpirv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gjzywqtwq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/glcowstcy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gurewungg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/golvpexsq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grmcvynde.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/glytogwzn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glmnwthjo.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/glaoicjxr.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/giwhjrweq.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gsdttiqgt.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gbhcweevm.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gjprjpydg.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/ghxhcgpzm.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gqkvyytzr.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gtzigahnh.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gdceqilia.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gbvcstamg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gisheuxfj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gsxgzhaam.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gwfnwgbeo.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gtffgvyao.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gaqgkqwzn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gxngepiqh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gumqcmfwz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gdkykmzho.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gzrtzqpwx.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/guhozdtsf.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gndhhllpw.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/geouuwbwd.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gfmxmookd.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gnpygcszw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gnhrkaaxo.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gcxmosghm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/grrrizntk.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gnodomnnf.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/giscwptov.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/ggurdqpdg.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gfrtyefay.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gecuiyxre.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gmxjlmmkw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gmudvwdru.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gskdyrwgk.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gfuaedwwt.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gypqsuxnq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/geuipeaug.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gtdpussna.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gykqwhrui.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gdaowiwqy.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gbqogbhfa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gqfxfswij.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gkxciogiz.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gpdpjcrxb.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gnmgmuksp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/guxhrwabj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gvuyexqps.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gfbuecihv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/givmfevmo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gwngyxghl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gfyfcrczx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gctiniajt.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gxxckroac.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gjjrfxwvr.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gkqoycmes.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gfykrlyhh.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/grawkkvos.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gpzugdswb.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gokryvoyg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gdcsyidmp.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gxwksnqyk.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gqyjhcvwy.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gjvedryrd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gjleyvuol.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/ghvfxiztm.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gsekwccnv.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gdjtihheq.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/guoopkzxp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gmrssdkqy.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/girbnfqoo.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gxvmgmrcu.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gygcubxzq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gogaqypwu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnfaowoix.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gauyivgid.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gszwraswh.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gufbmurss.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gcydovxvn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gybnnmnsz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gkoknsabg.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gjwhjlwzw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/getnlsjug.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gohjokjcw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gzecamdja.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gchiddxmg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gxllapdrh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gjjritonh.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/goechbwte.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gnllszfxg.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gfbfprfwl.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/goccrrrcq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gujrpeeat.sHtML


<!-- 参考信息 -->