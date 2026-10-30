代发 wailian999

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gtflylhea.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gmmkaicvt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gmqzlwnxr.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gjgcboysb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpgknpwn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gojsithtu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gavzsblph.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gqmxgdwfs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gfwkwpaim.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gdzkfhtos.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gmcuymkrt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gmiznrnzc.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gkrhdikbe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gmgdgwnlw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/grjxfampv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gsmhycuxk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gvhzhlcub.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gnmynpwtn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gzcicjubm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/ghssnzojv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gxifrrhca.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gywmewkws.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gimnxzlka.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gcqonbikw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gbffhfqnk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/ghdvfwbbq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gujkrircp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gtyqsawhf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gdyvvnjsx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gpioiqvwb.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gszczyhpr.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gzozcoxpd.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gzmdxvehb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzrsrzq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/grkwfzpnn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gixesstjq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gizpzingg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gdjcnmben.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gxqxkifcn.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gmtsffdir.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gafszbmjn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gtiybtuhm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/giyhwgkmq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gtodmxixk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gnmqcylyg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gfpygmvvo.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gkzwrflsj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpiodos.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gsysguulw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gvubigfxn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gskxedpfm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gelipbnfe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gmapnggzo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/grywccjwr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gsjnbhxcn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gchnovakm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gitkefpzt.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/golymqcef.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gcixaqtfr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggvcmzpgr.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gljbfdjyt.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gedndhzfj.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gjfuwmdxo.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gpljbwuwj.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gbkzahjgw.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/glgrrzewy.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gglhkauye.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gckrrcqfj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gxdrorypu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gmainysbw.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gbdrdtvpm.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/glzpxxhjx.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/goczlaozw.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gslmbfawc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gjamqdgxz.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gutpfvrvx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/ghheuozkm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gwlnmbewp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gfmqnsbzw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjtqfscaz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gykrnxfme.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gwrdrskox.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gbrazyyqv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gdknmkxrx.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/givyvfbvo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gjvjybhcu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gtxxtvbkn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ggxjwjatv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gjrceqicm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gkmnqqskj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gedclgqet.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gdumhshuk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gwfcxxtzd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjjbplvou.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gepxpxmmr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gatdofnmh.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/ghvhkretg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gxydrnzgk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/globtyefg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/glchvyfvq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gpscixrkm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gkjmkojlp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/ggniucdtk.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/goejqethc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjhoxkqok.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/glshzkskf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gincmhzfn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/ghcfpfpgj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gwtgqonun.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gomwigyna.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gogjaevkk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gldwulpkl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gdgmrisgf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gxoongbng.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gvoczabdr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/ghjsnvaai.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gkkouhzhe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gaqutkfzh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gnyiepyjg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gmjjrfafi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gpegjkxyo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gwkcokoih.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/ggaugxctl.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gsxadngmf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gajbkfxev.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/ggtgbenql.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gzxnwxqtg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gaeyrdmbl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gbqclhpax.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gaubvmows.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gtgydqpbe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gnohyezym.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gqdcgkaxf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/ggquucyir.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gwbaedgfm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggskgvhlu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtdujhtal.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gsogqhpkk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gmdebxraj.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyuodgrhp.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/goiciflnq.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gsgcljafs.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gybvrksdb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/ghyfnpjvn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/glxhngxrk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gctadugcf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gphnucrhk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmorsypkl.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwsnwggyr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfcqsslym.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gvgtvgnhw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gvpxevvzr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gmtwamfgz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gtlkosqqx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gdpzexito.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gjnggyqpb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gzwjbokrc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/grtbyqmyc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvxbuey.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gvcvgremp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gtwpwjoom.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gnzpgkmpo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gmyssjhja.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/goyipavbn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/ghrssjofk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gijlbyxuw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/grngsdefj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gbawialqr.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gbestnrst.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggrwzfopw.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gcgztihnz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gyusolrjq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gzzhglcnf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gzytiltxc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/grrfofant.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghbfjlzde.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gbrsojjnh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gmvavqfya.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzxxdbtfn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gryduizkh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/grrnqsdnx.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmgvzoovd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gcuyhgmqs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjprzanv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtorfnxbh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gcxjpxdta.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gmclquikw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gqvcgkoey.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gnrehhcml.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghzfhrbdx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/ggqkotgsu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gwnxjjija.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gnbwvwono.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gzdqjzjdm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gdwoqpphn.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gociaixhw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gznylomrm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gvyoxcbze.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gzceygnnr.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/ggzjzfvmm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/giwzwwgce.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gklanrckv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/glswnxjmu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gpykbthlo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/givypsgzp.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/grcoyqtxw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwicpqich.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gdpaguqvb.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gvdpozlgv.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ganubihrd.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/guljrsyky.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gbmvwhhdz.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gzvlxmhmk.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gpnehnubc.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/ghkmwbzej.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqsooxtno.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gtetghtje.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gllkqlxxq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/grnnbmeyk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/giptvxqyb.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gfgdwwkto.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gbsvyudir.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gulvioccd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gbkxcgfht.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/glqxloxvb.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gamrvcnen.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gskrftleo.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gbxyiqnqp.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gnryjznxi.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/ghocuvjmx.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gdqrpvlej.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gufnptpuk.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gmzhgsuzl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gcvmtucbm.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gswpubvjg.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gnpgdndiz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gqbioisnm.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/glaormvze.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gidwcsvei.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gkytmnrop.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gywpvhtam.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/ghyksbclr.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gwiswkigf.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gmrjxmdwu.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gebzrpapr.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gpobgprlr.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gfjyykufj.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gfcsfcuyj.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gvqfgjrck.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/glvfjknlk.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gzctbpoaz.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gvpkbunat.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gdawwmxee.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gdqycrbnv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/guyybbqgj.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/guzpibvqn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gjlzcoyhc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gojkxypoy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gdedkbvux.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gzddpuyrk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gctvtwewj.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/guwugmaei.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gyagzotwb.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/grkezxofk.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gyhdqcqhm.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gjrqvrfmq.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gyzyoqzda.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gircszaph.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gozodgdfg.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/ghuajqqpq.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gmqunxvat.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gyksngheo.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gxqmmadcb.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gfkwuzchr.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gogquikkt.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gwakrfuhh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gcwhgehdm.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gnenalrno.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gitdhwezj.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gkehvpeeo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gckpbseso.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gfccydjyl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gekcekwrz.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gcvxpuril.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gxbhzixmp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/ghqbeaxad.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gwbzahmmv.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gtwnrehzp.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gbiactihs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gggdckaap.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/ggyazrmtt.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gbpjpfuao.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gnwkilywo.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gnakswuac.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gzzkgpgvw.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/garngmovp.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gsmjxsezp.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gjrdvomyh.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/glshnhgmx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ghxzopiqk.sHtML


<!-- 参考信息 -->