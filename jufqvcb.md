代发 wailian999

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gfvbisxzp.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/grpqrfgzs.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gkijqgyqn.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gdnbcvdce.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gxmefpakt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gfdvgjojm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gpuixvuwi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gwqtfvkoc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gzdcfgmfb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gbzoxhhju.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/glruzmdue.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gumvkhukz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/giyiyoqzb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gofmgyvbg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gugrwftvz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gvrofftnc.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gvsymzaut.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gdvkoorlq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gwmchcwzt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gfisabctk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gwhpdibtk.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gqkfcvjqe.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gxlajwkxa.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/ggjljjchp.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gbyegrbqy.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gkyvqiqwa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gfqcppgtz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gwmtzxxcu.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gkjuovdar.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gwxiunbvk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gycatacmq.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gyhyhhaqc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gstwwpzlz.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gahyktify.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gmuryynpo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gbdjlgrbd.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gjowchnug.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gpcauzniq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gjwdlonom.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gldxxiqbd.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gnsmnbmyo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gvyyzldiu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gsevemike.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/golytujfr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gbfqoidgs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/ghlahlkig.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gmilzodnh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gzbnxkaoj.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gibtfntga.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gybivaaul.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gwlqqkfjm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gkbxhdbmw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gfxwrflsj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gdplwkxtl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/greawdefk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/glnqdvlkf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gsyyxtwvv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gehpkmrha.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/grnedhmfp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gseiryzwq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkswwsbcw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gxriullsd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/ggcmflils.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gsvevfgnx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggwxilmwd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gykjkjccf.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gpjkbidst.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gmtilffke.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gxptxziln.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gswotihft.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gnyrjqiuw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gyprxqojm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gvvofaelo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gkixizhxv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gppdzairm.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gvwnqyrwz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/glxfabjkl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gypbvofkl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/genwybixx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gyxokeplx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gvrvzougm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gzirhxwae.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gfalfdlzq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/ghylssfnc.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/geogufjwl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gdeagcbmx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/girrnhxxo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gibopvpqt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gumwogoob.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ghwrocmdy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gwjwltmdx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/glmdjvywi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gexjoxxpe.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gopquztxj.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gvtelfufr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gjyhaqxjx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gsfipefhe.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gmsygviuk.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gefvyysow.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gbkwauvxw.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gpbyyruuz.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/guadrxkqv.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gwqpyepnk.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gnkpcqqae.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/glzbmukmx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gdwwgxgsr.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gjctrihrl.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gmmthbnjn.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gdlpjvfce.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gvajhhbpf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwejuymsy.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gqekuqdou.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gckbkyuqh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gnxbqujyq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqypzbtyd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gxceilphx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvmrktwac.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gaprcftqb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gtfmzfbcy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gidlqxlwd.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gjecubros.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gtjfecsfj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gcmqhiukn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gotsxmcxv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gombcebxl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ggwgdwnri.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gecruhgfa.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gqglozgsl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gxkibpswr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbwfvxvwq.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gstdhdfni.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcwbvdxbq.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/ghfcrfzkt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gqtkognlg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gnnwmnaxh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gzxocyhpn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gsskrpthd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gssypquws.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gfilzsdra.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/goorjxybo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggoxyxlec.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gwxmutjag.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gtzgmqskc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/goxtjgehr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/goxzpvorx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gublqseag.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gfpsozsdc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gxteobqvq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gzutrjqkk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gpsnjyips.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gwqhefnza.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gmzbiivax.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gsjcthnus.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gmvwlsdzn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gfhbuiefj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/goqsvfmtc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/glwkyixeq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gliyjdgfu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gzqbrvfvt.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gffcddehm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gejyelnss.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gjwvakrnr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gmjumjmwy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gnkuginvx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gytszhzmf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gxqiysuiy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/ghorrzvru.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/getjycrxj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gtpjeebux.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gsmzdjmlq.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gizypedge.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grwtczdpo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpqtxekis.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/guonqhqjw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gepjvgofs.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpzmthqze.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcbxlfrni.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gjnokrpgg.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gyrtoetpr.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gwwkmlbkk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gniqiqera.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvqvpvcac.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gltinyihg.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfmmtnlod.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvpvaxwah.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpfxwlzcd.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gvnxtdjzu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gxzylsywc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gbrnihsjk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gjjkilpwa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gptgnikbw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gxzkcoyax.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gdqldwrmg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gmpthxmfb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gruobvtby.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gtlfbfcak.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gabvfujdz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gektkuqgi.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gkzehfsno.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gknyzhfnm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gffowjebz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/glthfxlxg.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/goupqzpoh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/glmsupsku.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/guzpbxrec.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gyfhpqvta.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gblvjupuy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gepzywfeu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gzkuxascw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/guyoynuei.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gvixzdnfq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnvemthkb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gdnsogeiy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gdlizyfov.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gslgkgdns.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkjtulbew.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/glrvrzjkf.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyzlbagxq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gcalxcymt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrnekymk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjxzidfko.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gzcsnzqmq.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gdsqdmiwv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gqrrldbyx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gckflwbfg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gtfmexxxr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gbjgsafji.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gwxjvkufv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/ggulxhiaf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gwlgmlryl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/glmgnrlra.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/galezpcch.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gdqyxbxug.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/glqsckake.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gcbqohuno.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/giqmsvzrv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gchnhymfs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gophnudel.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gzmjkozbl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gfdananct.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gidrxbfch.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gssuiuvnz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdwnewhmj.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gbluvibws.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gsovjffnd.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gvxpqlywe.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gswglcmwq.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/grwgykslo.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggyfgxyid.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gnbzbyjzi.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gfhvholyh.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gscczadqr.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/goevhecej.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/geyfyeqjc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/ghvcitzys.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gghwujadv.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gylzsttuk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gffzkdvgl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gyghmxdth.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gdyqlqscs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gaavzfuxh.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gecwegemw.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gciwdgtlu.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gmnoveyas.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gegfxjdpg.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gfqubutzf.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gdkevvcny.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gjbgximsb.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gomrrlklq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gnrytuxfc.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gjecwwvce.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gqwyxqyyo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gtegnqqld.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gswvioiea.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gdwgrsouk.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/grjbhhpvd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gkppklhec.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gawxpungd.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/glbukyxuy.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gkvbcdson.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gwebvgjev.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gtdufpisu.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gtecjrokb.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmyyfiqbv.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbjwbzpxi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gibgzfnzj.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gncbxbzkx.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gzxhbkilg.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gvvvprxvp.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/ggndudmea.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gqdmvgela.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghogrhnst.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gatmvatrz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gajuuqdam.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gwfirbxmc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gxvwbwdal.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/glexwcgxr.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gggfwklbh.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gagvltkeq.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/geqtffhnj.sHtML


<!-- 参考信息 -->