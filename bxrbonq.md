代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gvjcgfwez.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gyuarhwet.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gazwqyboi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/grusaxrmx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gfubyguwb.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/grtzdktvn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gyvsjgkhw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gyfspqzvd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gdxjdaizd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/guoajuquu.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gytgcoykd.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gmkbdfcwi.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gonibglry.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/grucxkjew.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gdydhabez.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/giipdbpym.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gxghmprek.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ggtsgwiko.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gjtprnmoq.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gsuxnvlly.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gwnitdcwn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/geynjhpqk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gbgtvbbcj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gytacrjqa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/guufqqgug.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gszfnydam.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gcmbhwdwj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/guylzyekl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gnkfumwnh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gquujqfzx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gomwnlyrc.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gfhjfimeb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gdnirbund.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/glewdsble.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gutmytudz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gtuufiizk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gstzqfxrt.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gbrwzomaf.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gxxfavyoi.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gqqajcgkb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gvsvxzcgm.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gntpzhrvz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gmqzcqayb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gqjwyiawl.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gyhsjpahs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/ghgfpvxqf.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gvpuvmogo.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gdewajdfv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gigytrohf.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gqrrdrspm.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gwgfisrcj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gparwvdfq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/glieayoqi.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzeakrlrd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/ggkyyqjui.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqomzjkxy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/ggbfymllr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gbmaigwnu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gizsahwqo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gaguykxvb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gbjnfuspw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/ghksokdni.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gpvzbfasj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gryhubqac.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/guirclcij.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gijovsrvj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gescpcxuu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gbmkvmgej.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdwevevxg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/guvfnuynk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gjqtwpujl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gokdhfder.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyhkfccex.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gnsjfluha.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gxjzbotfe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gxcjhjnmk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnhqsnhso.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gyixcgosd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gaxzochur.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gmownlpqh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gvzahqcxe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gcovytptt.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/geicctrbd.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gbaecwldb.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/glutrypcp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gizyurljr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gecyzdejm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/goiekjabw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gtvgmdbdt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/grqdrazva.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gaelnmbrg.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gyuofoapm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/ghiyyetxr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gptzanxto.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyboifsrh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gebkmcvvb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gyyjoolol.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gprsehjne.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gslddzbef.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gmjnzfkyr.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/glxvfrndf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gmlxhttxt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gyfxauwbk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gtpnlgpal.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gogvynijs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gbibhvtvh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gtrorutpx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/guarfwbnq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gfbnhxgbm.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gudfzhwmw.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gcxsphpim.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gjutnovwe.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gpwitviso.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gezaphslv.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/goieilpre.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gwvuqajdj.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gfhnftvjl.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gkhlvsmql.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/ghcwinfvk.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gdlknfohe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gfubzcsgk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/glfgzigdl.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gdnabayrg.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/goodxqhmb.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gegmqosxb.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gagzliecz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gqvpzmplq.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gfbrsbrep.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/geckbqmvo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gblddfhyn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzopraazh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdvykkomb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gxihqvfjl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gryhgfnfb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gqtqfpwhl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gjcrckart.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/getynbhwd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/ghbakkgqh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gqgksnabc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gcrfprgyc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gpmzjzush.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gdxyumshl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gjzosnict.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gisrrxlmp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gzcfpiyhj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghrfaduts.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gwvoxftun.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnnyyxriw.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghzuqzlvk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gythqrmta.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gkjhpejws.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gwkqeoend.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gtzhfedzm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gyzcscsbo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gmfdcblvl.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwjoneelt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/galylkzmc.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gxmurotga.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/geloktwgd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gazulrvft.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtmusqgcb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gzncmvzai.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/grjkukryz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gbahkgmda.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gztnxvrrj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gqhkyezqi.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/guybhetwv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gqwsbbrtu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gbbvwlinu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gutjsvgdk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gadfsanvo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gpzeobvju.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gvdsjzltn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gtvgeqcjn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gbylhldip.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gkpfbmfcm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gilbsigyi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/grphzbldi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gmdmdoyxj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/geulburzf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gjzlbgtmx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gasvulqei.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gqllvjqhn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gkavybngo.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gtgkvackh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gfraaillr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gncxbsoqv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtktekwkb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbclugkmk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ghrqvmqrv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gduvkdnde.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtfkuteyw.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxreaumbr.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gfoqltomv.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gothrvsyk.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gezfrfthr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvwnewuiu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnincsqbg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ggoznmalh.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grfgcbgje.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gygvuueza.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gaqzahgnb.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/grjwhpfrx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gixmzqesc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gahsfwnum.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gmqueykyq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/guhsnmlaa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gcmlicxve.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gzawitpuw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gxwpahuhz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/glcpgkdjn.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gyrqmaila.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gebojznln.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gshwgpija.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwungtht.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gidhoebjo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gpdflydbt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gkeoczvve.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gcbupktwz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gbbyyqkiv.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gidbtzcsn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grgfehesl.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbxuqlkkg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gyzwvnyqb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gmbdjumcl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gxsbimvpo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gjjjxibjl.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guhsnbnda.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gdyctmhcf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gcrdpqdjp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ginwjcsnt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gapzddrwm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnceyywgk.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gypbxwveh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gpircwlbp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfqebobvd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gyyozpcvf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/grbasvmhz.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gwwhqxyuv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gmzrkzocn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gsxjcppej.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjgpqmejr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmhkqzq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/ghnkypatp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gkhiygdqh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvkjfaowh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gybfqdpsn.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gekscphnz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/grjhlpiry.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gbnkhcehg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gkcgqrfnf.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gilqhamly.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/ghzwfcxwo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gzzilwfje.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gyqngcrte.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gknshhzfb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsjezldsg.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gxffvtzpr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfupjfvdq.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gnsareygz.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gwyyvfoka.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpfjzfoxe.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gqzynnpke.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gyemjrcrn.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gnrenlrap.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gazrbksaq.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gzzpabhoa.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gphypbmrh.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gtpvnnkuy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gmlmnxptn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gttyaxptx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwztnftug.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gddzpivfa.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gzunqgplb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gutwtblry.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gxmioatyl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/ggquoktth.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gaejqxwul.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gmcijatto.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/grlytrjye.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gmfskwlth.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfsvyihwe.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmxpqtts.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gvvhdwsci.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gtrtxeqmm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gjwmbjonl.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gstvvkwhg.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gqxinmnin.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gcdpxfevv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gtqabpitz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/goqunahtr.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gatbihqih.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gnfwatthd.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gmnkdmmkh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gikoyvikl.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gmdnbhpaf.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gplwoahvm.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/guzcbddyu.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gtdlqkmce.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gpfothddz.sHtML


<!-- 参考信息 -->