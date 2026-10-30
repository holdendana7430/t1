代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gsarpvlqu.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gewokihqr.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/ggishjrzm.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/guukmlvgv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gnofuykvq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/goknmzbtn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gxlijbggx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/ghthtjilu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gobgczebd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gnhkxedfk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gavdhgstn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gehauiife.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gmkonfuah.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gcnldavpz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gmfrhyecb.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gsmlmngcq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gcodmzoyg.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gcjjftohr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gnkvivjht.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gmcedjjqt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gqkldkhdb.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gberxwmrb.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gpypukafu.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gchaevknj.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/glvqrjwuo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gtycyexjn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gnbnrbseu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gjbtnwahl.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gytnagxdv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gzfiavoqk.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/ggejnujqj.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gvuofsehr.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gogkdmlwu.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gscnwxwvr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/ghouzaneq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gnaqrtsju.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gdrmojuph.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gmchdmtox.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gnbaysagu.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gpvtmcoit.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gctwvjymr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gcaejxazg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/ghgbdavll.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gofzrehlr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gnaqdwqxo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gyweodsph.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gnmxgylki.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gfojlmomb.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gdjnfuglc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/ghofkornw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gsjdizcze.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gcfjuptva.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gcngiasam.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gegehpkdi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gzbknsztq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gijwzpdfn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gegyhecba.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gbpzbjesv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/geglliadi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gyigsdvpf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gauptremd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/ggsbfudjt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gjltizocz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gqpemkbkr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gshvjmxff.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gfynpnwvi.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/geiwvxmqv.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gkgjxsdxe.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gsonbmvrn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gmlwwojgu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gcykemoog.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gfawlpadn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gfdhzxujy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gfagtijcx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gauzovwgr.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gmjiyoqwa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/ggspmevnw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/griucrqce.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gfedyroij.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gczkaujkc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpijeunbe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gbcjjltyk.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gmfwmnhki.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/goxixgipj.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gxaaqlnth.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/ghspxnece.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gnimhikwh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gfdwnpynk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/grwmhpusp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gesdnkgyd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gtycmzmpj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gdefwmlcz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gdpyqkamf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gcfcobnon.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gdyniycje.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gqpqkhlom.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gupyiawsr.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gmzcgsxdh.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gvvhxhnfr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/ggauwddet.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/guudrcfhv.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gngaheokw.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/ghvwejyab.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gtcuawmbm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gcejsolwg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gykjskyba.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gffwnkkze.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gymhmxmkr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gmidouets.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gcabtegro.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnexnwetz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gnsixqqmm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/ggyunocai.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gmobhycje.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfxiqcwxg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gjozigccj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gqpctqcvb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gowjlpydp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gsmhmoabj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gjkwxzjzt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gfyyxypzr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gcauygfvx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gwvatkhkg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gryknylux.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gpmavjphi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gxxkbyzwm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gfmqoqxtq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gnndxzngb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gwhlcdhap.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkpbnnsxp.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gqevyleov.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gthbgzffv.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gmkosfcji.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/giqptcdeo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzcgkqung.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gmuwahpkr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gmduqrjpo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/grsjaievj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gnsceljdi.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glmjwcfjb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gidaczpna.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gxyqrgiws.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gjtpoujmc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gqbrcpatl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gxwrjvwnp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/grlyjysgk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gxnenuaid.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gfnqmggjv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gqebmnqah.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gfiogjdim.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gefodabkd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gzekpzsls.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gvwrssujo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/ghbsjcntg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gpnsqsqez.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gbpatmdwu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gnvrofmdn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gzcsrpfck.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gidfuocit.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gmzdcjxjs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gvujschou.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gzppgqdvh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/guyisbpke.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gyieumxnu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/geuaufjvf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gvrshtyhe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gbhnxwlss.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gbeyrphup.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gnkflnqho.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gwrldxvnx.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggboebgri.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbiyjibsx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbsrwiswd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gkkvkslck.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gyyndpcrr.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtmlbaurz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxljqmloq.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gdymzwjtw.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsbvgsxtt.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghtnkretk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxrgloerl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/galloitlw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gtruohxmi.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geowjqxty.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gprarzxaq.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gtfbcsflz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gpqycmrkj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gwbhildkp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gzjkkndgg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gbkpdhwwv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/ggvbsaunw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gnkituofr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gdtmvfpyb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gdsustnky.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gripiipna.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gstcjlnyr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gdisztdys.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gjthkyutq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gcgduzotm.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gxsmgljfv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gqtnkggge.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gokfijvsp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gjvqmbamc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gilabvpag.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gljhqnonr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdrguggtm.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvoxclrpv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gahjlsaxf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gimumlrba.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gvhhwdfsm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gzxykilry.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjatwxmef.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gdeasncwa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/glifnfomj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/grwmjcfpf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gysqpxqhm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqeqouvpr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkgokkqsl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gjqsxopxt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyufogich.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvfwkcubt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqamorged.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gjqzkrelj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gxqdbbelz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gonfvdnmm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gkadrmili.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzfxwbltg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gzjcwqkfh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gnkliykxb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gfukhbqry.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/ggsgnmvre.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gigulfwpi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/ginepdfic.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gcqaebexw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/grpwofqyw.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/grsqvycsa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/geouiunft.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gzlxdagcq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gphwvjrdi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gtlmwrmjv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grsuqmqch.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gvlqjryss.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grhlbpxoz.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gvpnhdmfo.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/guhwvoekk.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gsbbpxipz.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gzimkmxhs.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gwhrlsxjz.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gnofmwjpa.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gkpchrnsm.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gzvvzaznr.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gsaftclht.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gfkmtguzj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gyalrkrxf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gkrwsvurv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gbrpzofob.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/grkhbxxiu.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gbsnysiip.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gaapdkzhn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gixlvvpxr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/goynpphej.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gbxayycan.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gibsuzpjb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gmqzpfebd.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gyovgcmri.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gwpulonxp.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/guniqstzw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gtqwpkozz.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gzpsaveab.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gowybmnux.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/glznctatw.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gdpvsepbb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gerfbpmaa.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjglympek.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqfyrgyfs.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gwdxidzqx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gcoskwiis.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gddodeahi.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gdtufxqye.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gezpnjhcf.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gpzbslbxf.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ghdlheuex.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gvmaffhix.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gjypjzogz.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsvgctqee.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gqmiyawrt.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gavlksnaz.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gmfrphaua.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gwtodmzvt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gtbztiwem.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfdlspszw.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gntohjcrr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkycwfmjb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gjyzmhzaz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gxjloxtcr.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/ghtjaktzy.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gqyowjdzb.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gookrpzoo.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/griqbksmm.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gkofcwhgr.sHtML


<!-- 参考信息 -->