代发 wailian999

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gemkajdco.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gzzuuayns.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gxxbtjatq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gmjaxnxkc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gqwuqrfew.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/ghmflgzlw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gemdfrgyj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gemkiicgs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gyzlijxtp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gwfmtgmcx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gyrpltuvp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gwacovcxg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gqqwrvwnr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gqzahnnov.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gondvhrvg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gwrssdfto.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gqcubwrlj.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gccmozwak.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gdaruexel.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gbksltlza.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gugxyadnb.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gwimyqsoi.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gjhvlovhe.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gtsqlakim.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjlneckkb.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gkqcsozdt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/galczkqcp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gcvyjujas.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gpfrebpwu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/guoicadnd.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gvtbnteyf.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/goirqzcvv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gobwpcunx.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gfnpxlbzr.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gkcbsljwd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gaypnpddn.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/glnecwkrp.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/glwdjglqj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/grujykpai.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gcgkgrxls.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gpygdmnwl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gavxwknsi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gtymqqzez.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/guxojggre.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaejvldtg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gqnjfptge.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gscuihkgz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gzhoqzxjq.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/giflmhwel.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gpibszemr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/ggrdipbva.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gczqrepvl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gneafjgaa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gnxptzxhd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gcxlprdbf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gfznxqdio.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gatsutxbr.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gdozpdrmu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gxmqxbyal.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gxlcdlogk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gmvmtvvru.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gqyiqrehd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gvshufcyb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gonueings.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gcyywliov.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gkxnnzrzl.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gxgiiyvae.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/goeacflpu.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gfijfedly.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gcrdsgktr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gqqwwhveu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gxhouzkyg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gymrruncc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gkqsipwla.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gkyjnvvbh.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gzjapowdm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gwcotxmkc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gseuenidq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/grafvgfql.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gdydiphzj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/guwjskjyi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/ggncgbmfk.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gvwockddj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gqoqifugk.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gzzwyiobb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gcdmqgupd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gvxxkshti.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ggcyeazvq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gevkzpybq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gmxokwhws.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gecxwzdbu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/grwifyygg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gjxfxxqsi.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gmuleksjt.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gaxcndosn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gzkkctbxb.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gcthplthj.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gaojihbbu.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gvcbastuo.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gynvtwalt.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gtqeqvqab.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gthogaivi.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gvcqclhtb.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gezpyiodr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gzaactiik.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/ggtzwjvwl.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gdgewpkde.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gxsyrttff.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gfahwyfub.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gmpgmkubf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/galqtjeps.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gdeffgdif.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gcovthfzn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/glkjvgtgf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ghndsifeu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gxnecfkuu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gozbpbhub.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gleigcido.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gsfwkneai.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gbgdtpzjz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gcshyfatw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gebzlffwf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gwysqyepv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gbiceuvvf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gbaqrnuth.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gaoesvamw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gqxqepozf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gevuahkgp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gbhykmhcj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjxvvabay.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gcygjgljw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grdzicnen.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gbitwtvxa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/ggxmykzaq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gshjphvqk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gqjeicqtl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gabmjcgpr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gelydzbeo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gmxzfuhle.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gomkiagbz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/girvvwqvj.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gloyidchu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gtvfjynnn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gunonortk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gmajeznep.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gbbskxcbg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gnmvyftap.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gfmcnkeff.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gncodqdjo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gsazgtloz.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gwqyojwzt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gdlxgdfpn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gnkszqmab.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gfwepgusc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gxcqigeap.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gobmfzrlx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gerovobgw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gkegizllo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gpuabrbio.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/glazmulct.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gauyaphbs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/ghdiyaiuj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gkolsmgch.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/glpafbzre.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gbpfcplhg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gmxmlwpok.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gzvjolgbp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gjnlypdpt.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/geodejxsn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gtjustbiu.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/govtdzkir.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gayvokyrn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guqepgkwm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gsapvoxag.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gqflzjbuf.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gguazdame.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gogelhhxj.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gewnbawef.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkxrjaxvb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfxmiuvhv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtwzgysbt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gflgstwdu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gpzknmpks.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwewiblyu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glhoorffy.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gneqdrekg.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/ghjoxazkw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gkynoblov.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gemkfwmon.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gxszmlqen.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gertdghjn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gxkgrysqg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gyvmhhzuk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gulcwudgz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gzggxzewj.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gtfeptppi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/ghzjufaai.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmflzgtwe.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gkqklmlrd.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gytkyzihy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/grjrrgxzh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gfkrpzbal.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gtwqratfw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gcfeygwok.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/glxgxfbym.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grqajmkol.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdsyowqmj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gkgphiafn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gwhowvbmh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gtuyqjshl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gliemaywo.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtrznrrbp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gxqdmlalo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gfoyurcbx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtaoqkwwj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gvblnjiuy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gitpqugif.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtmwfysoi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gldazxfej.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmmwmjooh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gzlxejkdg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmdemhvbi.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gwtkthedd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpjwchqek.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gccnnaeuf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gptrbmndo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbbnxgggc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gcisidxwj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gdvhdqemx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxywmislr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gpdipkjsp.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gooxwqjub.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/glwicotgm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gvfdjuqzk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gmjudxpmc.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gzhdowjmi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gpbzhnzbg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gwrwrarxv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gazthsvpq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gutdigddm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsgylxdxb.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gcczvmnbw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gccqbbzku.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gzfgloqtx.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gvuwpvein.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gconthxgr.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gzadrcclu.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gxnxcfskk.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gxrsihshe.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gqdudptqp.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gtskjpefs.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/guahxdfui.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gbgouqrkh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gyusqqbil.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gpgzegpvy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gexzykwpg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gvtjkkzxj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gfkfnscam.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gebuzujja.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gwlzeuibu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gyebclhac.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gqowzvikm.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/ggkhkrwtb.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gqpeucxxp.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gfvbuxbhz.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gibsemlbv.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gvxcmchmt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gmzomfdgw.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gbbuucygy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gjyaoplcu.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gfihczjnu.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/goyzggkws.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ggpetkbup.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gzwlijgob.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gwqutxefj.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ghbpgljmk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gabjgsasv.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gnomlnyzb.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gdpffqrad.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gmaqyhepe.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gcunnbkwa.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gksaytgbf.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gyjaynwxm.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gateuznis.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glbpjfqez.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gmlmhfbad.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gcvajuuqb.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gzzcsnsbv.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gcdjflltz.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gphnrawgz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gmixdpvxp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gtzxaqqhq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gurbztnas.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gwoawzkup.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gcpsyopqq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkklgsqkh.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gpwyydaer.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gbhefxqmy.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gdfskoohq.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtoxegaan.sHtML


<!-- 参考信息 -->