代发 wailian999

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjqhsxdns.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gbxyhplmf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gfuguiggc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gxnxxdlup.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gtdsaaexc.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gmszubtnd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/glujocatg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gpmwmibhs.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gqqjqysjy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/ghzehsyku.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gtaeytzme.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gxvlwwmcv.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gruaqklkk.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gvozqvdhb.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gixuhbhsm.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gvfczafhq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gzcjaoyfd.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gwnmwhshr.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gwgccxmmd.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gnuljswix.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/ghovdjqyp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/goghrdcjl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gzzwmywig.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gdbrzuqxz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gaovpzvvg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gktfiokli.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gzkrdmpii.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gvpbyngzc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gtlxurqar.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjaihurrq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/grqpnszpk.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/grtsruofj.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gmjejuqlr.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gsshimrdi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gkpqekevx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gwxyjbafi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gznqpjpwf.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gpadgzcyr.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gwsfdyorm.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gvciherkj.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gpozixeji.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggsuzkkkh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gqmaezdim.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gpryucxpq.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gxhxdvuyc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/ggqzfgosl.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gwhjfusqx.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gbxmnppfz.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gjncjszxh.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gjellcvmo.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gwjvuqyyu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gcfwyppoz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gfsoppdna.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gjvxviotx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gwmpzysss.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gcswuocnk.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gfsdmrlws.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gnjqptkuq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gehhdkkoh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gebtyggxq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gewcughdy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gwzzfmyta.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gspihnvmx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gsqmmtxmf.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/goigisdfx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gagnzdkya.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gpqhffebv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gbkvrysaf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/giclkzrfy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gbjuehqpb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gdolwjxcp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gbztziioc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gshsngwja.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gchuwzwgf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gfldqpngp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gdxvwtzsi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvoznhtgh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gpaxzsgmq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gwrlmgytj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/grsumetla.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxncuedou.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gulgvuvry.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gskgyufdf.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/goaxvxryb.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gccfbhshr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gmhzlepiy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gujckzjya.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/glcsnjgqz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gawtynnom.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gqzbatrpp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gobyrlolq.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gjkwzfsty.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gdwqzakav.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gbuukmclt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gbinctpfh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsoswvumt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gwvuhktwh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gqypxqiuq.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gsznpvhbu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gglhmlarz.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/guycqevfd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gsiahdppk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gxsvuzzmv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gyaclpsmd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gtmotdecb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gbghslcni.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/geafyyrpi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gvlvvjmzd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gukdwvddq.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gttpinlaw.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gwzvarmne.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gvcjazyju.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gabkoxmet.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gucijlhzw.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gghozyoos.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gfvhohfmn.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gyetemirq.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gzaznamkt.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gbsbcmfrk.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/guvvzdxvc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gduqmpimw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/giqmknbcm.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gkvtyopsc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwhrdsetz.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gchfuomkh.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/giuviycew.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/goozrrvpw.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gdkjlvgol.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gwkizqilt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gjugpjugu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvaufwksb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gcsqjckmy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ghzjoozex.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gtduifetl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcpdsoyok.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gagejfevb.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gvybrfciz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/grsyuyfsh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gwfjgtrqg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gfagcnzdz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ggmvozuxx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gdiigayqd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gohaakwcj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gcscohinq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gkbnmndyp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gydgyxqew.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gvankglfl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gypzzisiz.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gmpcxnqix.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gdgzixbqi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gtlpoivxh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gtfqbgrfh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gueibflvu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/grjanbbfp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gxckuxnyg.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gebomamkh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkgqwhrav.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gxtfanejd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gtogoaquq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gqtqrdpbx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gmkhqlriv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gnfqvcuvz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/goettioti.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/ggpmkmqpr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gmfdvoapb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/grfijudpi.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/guxhtzfcj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gaylhwhbn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gfbgnhgux.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/goxpwfree.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gdgyedfvx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gcntbfdyl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gtkebgtlw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gcnntfamc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gmtfeeawv.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gxcsioxcv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gjowjgryh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gtjukxfio.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gpdoeroxu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gfotuvofe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gednlpqto.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gbkiiezrf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gachkfelp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/ghzglefqh.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gmjojbimz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/ghbhcbsha.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grejrxycv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gksulbnfv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gofleyncd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gdjdcgjwx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gpsrowhga.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsmkshzmb.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gluqapuwn.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/guvgfaqww.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbrgunumw.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqeanvfpc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqciqmuhh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/grmzfblax.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdvhgivkf.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwjeudakt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzwewensx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpofacwqu.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gmryepkli.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gcwjeerga.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/givlooudd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/ghgoilzff.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gjfmtvvrh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gfkqhtzfk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gzjkhqjxf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gawfydaab.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gwnmdzyjn.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gfklrwkht.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gryzdhuoc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/grxqykoeh.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gmmsnrzlh.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gdehmrxyx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gfcsthtdl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gvvakjzwf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqbbcchzm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/grulatffp.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gmwkvlfjr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghkyacjkc.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/godtwcaax.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gmfuvybwi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gfzrymxtp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gzionyees.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gyszjagrn.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsucquwbg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gszknclga.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/ghjqlanht.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/giywlecks.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gepvdsxek.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gvslfkouq.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtqfdgany.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gtpwsvpgw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gmmppfpee.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glcyalfzl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyymhdaol.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gzmwzhmvu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gydboiion.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gupumbrig.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggsgbjgfz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ghgqixjkg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gxpwibthy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/guxaghjsd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcfmqjijf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gbnyhrnid.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gtvucrllr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gckwozwzn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gwifsnayb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gpbgmxhrn.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/grahmtspn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gnfeebded.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/glaccjuww.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/geadotvkr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/ggcrhyhla.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwjhgjlzf.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gakiaqzbf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmrdalwrg.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gtbxessdq.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/giaghsavb.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gxneuudrt.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gighzyegz.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gkzpjldld.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/grqbpfagd.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gpjxbczhq.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/ghdmcjrqp.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gcuqajgoe.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gubnghfnb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gcrggbnhk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gedtzvqje.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gyxmghikt.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/grxlrhtri.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/ghjqjfibk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gjxbajpda.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/ggnctqmiu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gvsnhohds.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gditzsgxz.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gkybmoqer.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gmyfjahvr.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gyrxnpmfu.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/glczqaugv.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gzjhvgrpk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gkvfmxhog.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gvzqqmwfh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gdovxlhdt.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gofjynndb.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/guvllnrhg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/ganlhrxyd.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gbronnbgm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gdvgnrhrr.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gxecglqoj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gnqvllafw.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gjynlmmec.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/glyshiwzi.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/ggzypbkuu.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gbnajkrfk.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gkmsxvonm.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gbamahvrp.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gucxoeagh.sHtML


<!-- 参考信息 -->