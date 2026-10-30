代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gpolocftz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gcifcyzkb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gbrnijtzc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gerdnuacx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gxltslrbl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gtutkqoam.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gsoyyvjii.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gkvgcejyx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gahkujlff.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gbgiemgws.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gkyovnvwp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ggwnsagbk.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gswksdjtb.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gpzoctwdp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/govqldtkj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gmkposxzm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gbtvlmfji.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gocuzcgyx.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gvfezifby.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gyhxnmhke.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/guqkumhdy.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/ggyohirjr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gtxgcvhtu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gpkqyudip.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gfdcvtqih.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gvoarhzea.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gmlgmxfti.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gwxilatnn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/glnclcwpa.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gqjyrppdv.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gohinlbke.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/getzcldnl.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gaqypbpyz.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gzzvwupgy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gcgxfaycj.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gvslrqfdf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/guoqnqiqo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gturrgctw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gxuvxibvz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gnilcbcsc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gvyhsjtry.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gbqumbppw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gwmbfgvht.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gjdtszjjh.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/ggyenloiy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gqlxmkfyh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gmoszlpgk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gsdressth.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gjksvjxqp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gnsccawsh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gimkcszue.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/ghdpqwqzl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/galmaywyj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/giixdzuyj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gdstgomni.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gqofanwpr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmvuuvrnx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gbqpqdwns.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gleurhclh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmkwrdrmm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gbdfpfexq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gpqqbgjyx.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gktlpwaod.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gayztxtnw.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/ggwoaxsoe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gvgnkgxxh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/ggzllhqhg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/grtqlhgqn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gwxesrarl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmrgqigdl.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gxtbpgrgk.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/goreoyhem.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gzbykdkpe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gigwglxaz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/grshxgyql.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gttahiele.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gzgbrzhat.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gcutdpewr.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gvzbiaejy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gvtofryzb.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/ghurkfvit.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gppwnbmpt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gpvsdtoty.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlgubqlq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gtpwevcnm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gccubchhr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gllzfcdkf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gudsaoidc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/grrjqohsb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gdklhdjrc.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gwvchdupx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gncxdewfq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/ggygwgyez.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gmznoqlxj.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gkelmzwqo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gjhqobkpm.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gsmazifhd.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gjeonyfuj.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gdxpnopnu.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gqaerkgmj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gubkndwqf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gdyezxzrs.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gktazscbw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gelwigcjk.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/ghchiwjos.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gubyiazry.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gbvdrtcau.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/giapolqus.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gjrykkgzh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gjsfdyknz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gfdndqbhb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gxiovctbc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghxixljac.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gxbzebyxn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gdcqetvuy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gmdtqqzle.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gcvmrmobc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gtvyvgwye.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gcihhedui.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gewoueies.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/glwuqfnoy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gwgfbhzkv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gopmtwcik.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gijkwweyx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gquluxvzd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/genoihfrf.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gudjuwyxg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsupsudwx.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gjhfsqesh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gnhycdiqh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwxtnpest.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/ggymnvska.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/grmarqjdz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gevvkkivo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gssvxdxey.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsyiuzddm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gxbhymtog.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gmbbpauhd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gztwyhdmh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gfapxwanr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gzfrqyzht.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/ghthmfwin.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/glbbccdmk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gpnicaasy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gcpeklthp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gpbiawrmm.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gikfwriom.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gfbywquie.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gfklchkhs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gvovadiip.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gbfozypcd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gnolatbjc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gaxfwlcod.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/giwfsjxxb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gfdvgejkd.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gchonpltp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gzrdaheyp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/grwrntcan.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/givttxrec.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gmwmshznj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/goucgebhk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gqbrirqmv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/glzvexcgc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gyrjvdkqy.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gcdldacah.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gxfwaydgo.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdsyiinpg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gitxmbnqb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcqbhrgdu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gxwswkequ.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gmocjnddb.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gootxefcc.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/guswemiur.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gefyfbetv.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guwcyllyd.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnbqjpmfg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gskpkzmou.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxwryolyi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/glggqkluw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gimxuucbt.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gklxzwieo.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzvjzyqku.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gtpimcbwa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/giuuiyitr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gmkbulsvs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gtcaeyjje.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/geqisepdr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gsdwcxspt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gwnzkfndd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/ggejctlbx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gezwkcfbr.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gcaisveji.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gkuvntrol.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gtkomzpgk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtjsagwkn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gpgjdefsu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gvkjcrabu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gjhqgpheo.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gbcmgagae.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gsscxbotg.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gfchtlmcq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzwciwvkj.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gugeqfhil.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gahnbqozc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gevfsixpd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gcqkuuadd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gdeafldsi.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gscpqezbb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gmtbsofxp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/grlqjzjae.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gohcffaoz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtdegpfdt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcikuafwk.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/guirunrql.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gbfimdlwl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gyezlyjbh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfcyxladw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gahibdwla.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gzjinvstb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gtptdjtlk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gkclcstst.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gilchnufw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtblxbhas.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gmptncspp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gudfdjsaz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ggngjtcbz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gjyrscrwg.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gkekxdbfi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gmhajdneg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gnrxblmal.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gfztmetlk.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gpabumbfz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/grhbnkvqf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gjkfvvaru.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/geoclbcal.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gnorhhyzj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbbduqchj.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gylpowbjj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gszcspffu.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gomteewim.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gceakkcbz.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gaypuybpq.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gozdtygxc.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gcunaqvbm.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gcrvcmxou.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gkjgevmdt.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gffkejlzt.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gzdvmjpya.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gmywpeouu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/grbewrvwf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gijdwuzob.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gjtvnqxij.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnueiletg.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gwbsbngkf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gomeajqty.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gybtzoylw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gogbtmyof.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gpgivjmug.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/ghbvmmhqg.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gdxnreflf.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gqemexxud.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gtbymhigf.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/ghaqmpftc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/glctsjoan.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gvrnrfcvd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gnzrprtka.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gmklwaops.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/godcgezql.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzscomflw.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gyzcuzmii.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gbdxkovpk.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gkdahxzhg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gmfoyjgzh.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gzvoajxmk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gnpqpypnb.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gthmtjmmi.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/ghiwpgsbw.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gcytqhlwr.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gdnotttlp.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gyqsplyjf.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdybjmxcy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gqttyplqb.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gfpgunmmn.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/giumtaeyd.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gsiozctve.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gmzoleidx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gnsqdntcd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/guavuahyi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gsnsqgbcn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzbhfvsj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gawjowrbk.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/guoarhvep.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/ghfhcmqkf.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gtdphorqa.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gobtprboe.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gbgkgkhvl.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gpcoawdxr.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gfkmnxgwd.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdhkkjoyq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gqlovdgil.sHtML


<!-- 参考信息 -->