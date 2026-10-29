代发 wailian999

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gewvpdxvg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gideepgcx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gdhfwohsw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gemdvgyqv.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gpndvwwqa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/ggwigzqab.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gkryqixzc.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gmtvjkmes.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/geelsqras.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/givnwpvku.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gqdtlchuo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gyiyknaov.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gjgsarfey.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/grmedfmxe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gqdpykqfo.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gsvezdggw.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gnbruwjsq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gojajkjde.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gaarapbao.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gycgplwha.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gorrcfimb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gzpbbdafc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gmhntdksl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gqxdnmwin.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gpuevgbsv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gleznnjwt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmfqmaxia.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gpgdxvmed.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/guqgqaooq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gycbxqfwo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gvbkwqdzd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gihcaybzk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gnzizmhtf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gczzvdgan.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhddiivb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gqxipymmv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gopepsyml.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gqwgckgdu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gdcfbfwew.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gmtfsoprq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gwtihtrex.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/giytioflk.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gxsnhewyr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gifxygmth.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/giljooyxo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/ghmhemalb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ggqircxww.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gpkxydfvb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gnrbmwyah.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/geiqkjdef.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/grtcaftdo.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gvpjshazo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gknwnfesh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gghdxompb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gislufsiw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gevthofum.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gvfckzyms.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/ghlkbmcqg.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/giadkvnaa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gjuiygxax.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gtmhitecc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gfmnwazol.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gfpmgbgnp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gfssbtakb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gdinzdmlk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gpujlogbg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/glhegwtdd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gdtzwcbev.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gnqrxevov.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gwyghokdr.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gzjcgmuht.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gebopuzus.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvshinxw.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gfjemxzpq.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/glpqqvcoa.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gsiexmesu.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/garkjlkmy.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gjetssqiu.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gapodmzej.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gvhkqeqvi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gvmcxnowk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gonqumuvt.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/guhiqczvr.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gabalkxty.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gwvnwnwac.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gndqylohc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gwzifcilg.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gqxllbwkj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gzmexpxey.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gpchiuswi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gtjnxluom.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gtydvyiwa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gjwwnzazi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/giqtfzyhw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gehtjiisb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gjmukeyfz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gicygozhi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gjklhstvt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gakzimflz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gxpmwdbzu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/ghkrhergc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gjcrnyuxi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gvnvrtnwu.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/grrmmoewi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gaqwrgvjg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ganvmnslu.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gbywacjad.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbpkezhtw.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/goexzkbkc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gjtmnxguy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gydhabekk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gqtfhayux.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjhdpmake.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gxkzkwfij.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gdfsjuutn.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gschovjfo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqbexmzac.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gdxjhyzwc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gkylbvrtl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gcbcqacgp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwmnrdkmq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gwpfeiqdf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gsafkichv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gnuierhog.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/girkpilox.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gyhswrgcx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/goomtpknf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gubbcsyvm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gofjmdqxy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gpprcesds.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gxjdyhogj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gjepsuxpf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gtnaxdtlb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gkyforuua.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gidfbdlqu.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gkskdhiyd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gpdbzqipx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/ghbhoiqyk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gnoobokuq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gylitynhf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gnsvxibdv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gzdkkqfqw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gvuymzzpt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/geatcgmnm.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gnaivspwh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gaxyqqdkb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnmhnjazv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grsaagkcf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdrsoxkku.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvzquldkt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gompvvfhz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtwvuendi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gklqqhmbu.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gnecnjjuk.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glvinwjnc.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghjgiyljq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghldmdtej.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxrvkbzli.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gsikjemof.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfkzborfl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnswpsmts.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gdkxxdbqk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gphtcvimx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gmsutnunb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gdwodedpl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gwybjjbeu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gtmydtduj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/ggalxughh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gpkqpyfpe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvaegek.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gzuuhugqo.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gfrevkvkd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gqngdkoby.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gqbqtnuhf.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gcviozrjn.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gindlchbr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/ghsgiooff.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gsfwkoexy.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmdnuduhx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ghgatoefc.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/grcxkjisr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guzbazxnr.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfvydtjrz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/goduqydsr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gcveohyqc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gtfamokgu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gtawizouk.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gptefpcqx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gltxnmqvi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gjzotntlc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzhgeaboi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfhcpnqps.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdmgszwxe.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxzaaryxh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gpsbysgyt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gudgqpokj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grcnspehh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfdrsgmug.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gbifvmbfu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkvbflhaq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gnunlldhn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gmwxfqjzv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gjeesxfow.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gyklsberr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/glelbmeyl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gvafjjdlg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gyftfegnd.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gqmjqmrof.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gdeizsxuw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gmoganbqj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gbxjuizpd.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gljpazhkt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gpxbiyupz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gmsfzribb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gmykcduyq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/grtgyxvjy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghnuedwqi.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/ggllvynna.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqzirrnsd.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gbllonlnc.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gsjsanbzx.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gakdxepvd.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gkyvcetug.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/ghvocbcdi.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/grrbiazjw.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gukucqgnw.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gekviepya.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/ggojostdy.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gnskmstbx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gtiwltmvz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gruymdifo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/ghpwhvyye.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/glxccqpjc.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gupamuiok.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gxlfpdirq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gwsikduuz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggmpaclce.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/glxhnukob.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gdsmffiqq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gazzfmlda.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/godlecgdp.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/goktnqmkd.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gatewldqm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gykumnars.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gpffsfyvg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gwllogola.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gbstaonwp.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gamydgbpu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gwdzklojk.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkxrzlvrj.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvvbifocy.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gdhxcvard.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gytqqvuig.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gxcvzbalv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/ggzjmmgjn.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gkcmdrjsi.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gcsjljhle.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gnmhuumlq.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzwvelfnz.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gpntguofx.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/golpqctzz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gkydtpoqn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gjdeutlsf.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/glryxewkj.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gyrhvkqau.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/glcwhmkpm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gdtsjnqnm.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gvbsezbhk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gtwczkgge.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/giyzkjibf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gcjodlhqa.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gkofvwxss.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gcjsgncdj.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gixbdbucj.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gzuxqtcdc.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gbeblpqld.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gdeurpiik.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwtfwyauw.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/ghcvkdrio.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gootawyep.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gdadivjgw.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gvdejynjy.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gzamxwewy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gxctisksp.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gkahubxhx.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gunjcttin.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gdzepuydp.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gwklwqqck.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gyfyjxadt.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gnaiwaleq.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gyqmzgoks.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gsrjgosmj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/ghcvuxkdj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/ggvxkjewh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gpytligxz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gtkazfeyk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gngrzeuqk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gpxmkyzib.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/glfxspaox.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gwfnuubxk.sHtML


<!-- 参考信息 -->