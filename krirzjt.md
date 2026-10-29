代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gtjcoqmzx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gerxdbvkz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/ggqsdbyct.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gkqtvfqab.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/guxsruxip.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gymidmdnp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gvdaidecj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gnotcifkj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/glpzpamvg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/ggqniufvj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gtzpjdvho.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gpevfclxy.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gccjwiwip.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gemdiqxuq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gqtonibpx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gkeswdyds.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gyskhikaa.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gabnzyxxv.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gmiymobht.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gtaxhugpk.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gnequwiqe.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/grtqsmhit.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gbzeevexe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gmlmljiuu.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/guecsuuhu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gfzvprjrl.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/glkxmipxc.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gfxmjurdj.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/ggsfcxciq.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/ginjnqqni.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gdypmjylp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gpbnanuyj.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/ghgfwcgul.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gioxaliyd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gsbcetyzt.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gksudbimw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gpycmlzer.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gpyjnnzdg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ggzlmmyci.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdccbhwrq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/grulvbhoi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gcoxntcrk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/goangqmxw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gpuptjgez.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gjdenabgh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gzrtaiexz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/graqgmmmi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gzxqykjhs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gqoifnnwk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gpgnglgmc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gvrwwhfpp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gxdtapdtj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/giimgmxil.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gkbtoskxm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gbhyepwje.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gzjhdfeev.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gttgechzr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/grlcmnqwb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gcayandpb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gptpivwwb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/ggbetuwlk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxpjseaze.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gapcpvndt.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggnbbweta.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gsioyabcq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gmvosdzfp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gdobcfuml.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gutrhzjwe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/geycccoen.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gvwkilkmx.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/glozkbqzp.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gahoezeya.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/ghwveugqa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gvutcrkxa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdgoseomf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gueuqseak.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gfllxvvem.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gcmvinpsr.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gtiqbfvmv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gamaxdciz.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/ggfvdoqqq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gpbiwppfu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gxabbmgnd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gomybamai.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gogpybvna.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/glxlneuun.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gcafwecjg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gjsgitafp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gzdthfqja.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gzpbqmkhb.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gayfpedak.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gfjjyvcwe.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gwlleupju.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gfjzumvbj.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gtplpzcjt.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/goqtykyup.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gzhwkhdxq.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gmbppyvhv.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gluhrcucq.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/glqkqduox.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/glngwodak.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gkomejijf.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gttfsynyy.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gtyvbwfiu.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gaynglbzp.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gsiagvgdv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/glcmcmpne.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gxeoyuazq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gutjcqtkl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gdhnyqxaw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gopclvoft.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gezcprlhs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gmzikfiqx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gpvgcozmc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gdpgfidtx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gaimzhpbt.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gukdrazba.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/goxjrffow.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gtwsevwnr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/geehdbgqr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/graajbffm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gsqbdausx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gxlqbipcv.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/goyplurab.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/glcgkfqri.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpbsnjahd.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gzqjiajbh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqneqqvbm.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gyzhbotsr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gdclarjco.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnrsajryn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gqdzchlmq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/glxgpksio.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gzdfcvzmv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/ggrekzpkd.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmdjftped.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gduapemtg.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gnmcfynrh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gwkodbvmj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/guphydmii.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/guaocquqs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gxrbzwpgw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/grytszqob.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gfxxndjbb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gsusfxcsn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gjyufysnj.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gvnrbbdat.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/glegdntbx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gsvvznojw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gtdsuwnpf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gyxmhjomr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gnulnvwsd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gretxctcp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gitwioatp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gdiptrlzf.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gjewllqjf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gbkoxkbeb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gkjrtzgpp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gcpeczova.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gmvqdlsru.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gtmfyxbnj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gsewpueoz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gceifzxsl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/giyesjpxq.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gxllopqfl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gmiumeovr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gyxvmwqyu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcbgclkae.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjzdygupd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gncvsqufu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gzjqnzuwk.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyjwezzgj.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfhglfgim.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gymlfuhbp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbxwmjsda.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gnhwnrbeo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkrwowhck.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcawpizht.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdvojxyyg.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnmurmbcy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsuxeinnx.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gunddlapv.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gotldnukl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gpmcctgyn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gwdlhvgdm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/ggjgisoeo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gtkozumes.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/ggyrszfxy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/glvjwekhu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gbkondzjl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gwqkleyui.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gcbuchsba.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gqvhkqbvf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gxmbwxgzn.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gokleqcip.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gwiseooat.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gfhbwgzbg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gmunaabsp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gicvxptde.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gwmsmwfsb.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gjjstsubt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjdzalfap.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqgkonrcu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gwlmsptqf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gmctyfnge.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/glixykgrk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/groxfszfn.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpohldzhj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gvflvnkof.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gorbgigwd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gajczsrtq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpprweaej.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gmusstnmw.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfjudbduw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gyemnsjdv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzqabahmr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdigiqyba.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqtavruxs.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/givgwidmq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gadnuwuwb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/glvjknpmt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gbihjndxi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdejsoavc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gwqdbvzvu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gvbgwlyuq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gicljfcbv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gchbgjehv.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gdgmskgbk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gqzpnilpn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gxbfuvpzp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gkaxjocrh.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gzhhyfalv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/guhvvcict.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/ghrufzbbe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gtfgtriya.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gbgztxgbg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gokukwsjc.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gmcbinbrw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfdfvgjdz.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/ghmzldjca.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gvycmwcrb.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gnnezgrxq.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gyvzzjjlw.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gxvmvycom.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gdwcfebds.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gxstjufup.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gchhfospv.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/ggkqghsoc.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gdbzgbddm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gozmhxnmz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gkjaldmfy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ggnozcwug.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gnjvtyocp.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gqsvpzepi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gszhlzvmd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gytardhgq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gqophzgzn.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/grhokxcgp.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/ghwanvbeb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvdeobshn.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gonggpdky.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gngjzsvgl.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gqqnhqzre.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/ghjmzradm.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gtrwdxbaa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gvkwxtfgs.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gmjjvlphq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/geeqyguxw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/geytrzjbl.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gjfrrnhut.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/grbnymwld.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/graivxkhy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gpfounogh.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/glpgzbltf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gtcxbaggb.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/ggnlfvpvg.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gwynnkjjr.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gugdpliks.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gnaeuulpx.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gkspoanjj.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grthpppwi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/grimnaaeg.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gsmmcgcgs.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gxnzquwzu.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gueuatigt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gukgqsfmp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gxwwbgusq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbfulwpma.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gxdlntdoq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gfsnhjmro.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/glkacpkpa.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/grsjsdmfl.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gaysztags.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gdbfpwzxe.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gtsnukedr.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gekissrtm.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gqrqpbrnf.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gzpnoowrx.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gfhdmjdqg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gsdcatzdm.sHtML


<!-- 参考信息 -->