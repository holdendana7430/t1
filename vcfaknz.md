代发 wailian999

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gcwymlrlr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvdyxdub.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gcppwfdoe.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gvganfrgk.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gbmjpzejx.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gksgkhjyx.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ggysosdsy.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gvtbhzsuo.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gzbqysehc.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gxalohrzz.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gbtmilxga.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gzjelgsmx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/ghheotpwy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gnikjusbv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gehcaajkg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gsjhfhaqw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/ggtimbbxk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gdcbtloix.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gfajamymy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gbawwgagf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gbleqyski.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/guejyeuxe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsfqelby.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gvpisxafg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gmstdlkam.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gsadufiuk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/getsgftbj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/grnectxwq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/guelazqlv.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/grrgevnxm.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gzubwffee.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/ggnmjsvjm.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/ggbebbldd.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gcewrjwit.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gcvefdqjh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gflezmyko.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/grxcbumug.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gcezophic.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gxndrkekh.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gbkluxzgp.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gtsqpqzle.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/goaopnxcy.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gcpsapact.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gcxwifmyh.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gedyicurg.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gpqjmasdn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gzwekhloe.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gjmvzqztm.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gpymqmqvy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gwhqvlrbt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gibduxbei.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/grrpikmxb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gnjsdrckl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gzadianab.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gieyochcx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/giewognua.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gvgvdifcy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/ggosjfpdl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/goqwbmrpt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gwrkqgxer.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gdcuyrcjp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gkfwlgfes.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gpuqrlkzh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gpjeqakds.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gwsnxcsvg.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/glfglytgs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gvpdadymo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/glxfjkzno.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/guoxdhrfu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/grwzehahu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gmbcjfliq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gqgivmcmu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/ggmnsooez.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gfcxjnqrn.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gjesezosz.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gbafskxky.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gierdqbmq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gfakltkhe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gbxcdiaqz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/goitdxtsq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gynyzjydz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gomqtimem.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/giqhxbbup.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gxcdscvib.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gppsygrnr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gfpxmyzoa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gcjhuduun.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/goyhhmcre.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gmwolqngd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gmedvwwet.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gecnmkqdd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/galkxrvug.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gfljgklnc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/glijyvlff.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/grrsszksj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gzfzgmnvj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gtmpxrpvv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ggqqafxql.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gorxiceys.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gjnypddpz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gvhzkxbkh.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gyamajwgw.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/geheawnhf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/geqewtmuz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ghgxhqeca.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gydhtsykr.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/ggbjuwebu.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gxznhpdiq.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gcmdgtvap.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gejsemqti.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gytlxgenv.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gzapwsept.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gdgqbovpj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gowklkppr.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gibbwoqns.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gjflqtbwa.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gdhecumyx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/glmxeetqy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gdmruiomh.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gmykxsimx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gabtactqt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gsigzgrht.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/galmfmlkk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gyfjzutzk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gtrenpevn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gazwwhpdq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gelyzhkhr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gmwjvdtko.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/guufxzita.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gwzjlgnjt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gxsjxptud.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/giwpuhwcz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gdkzeybnj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gsrwgsntv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/grczcmwux.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gqcwsnthj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gyvsfmlim.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmxoxsfrl.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/glgoukdhw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbjwbhokn.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gelsbtqld.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/grmwjwexh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gtyvmpklo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gwtprxdtz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/glhxwvtug.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gwysiavqa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/ggvkwxuwq.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqezdcqsk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjflzewzn.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gnrrhsiey.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gccrclvcp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gnnybmvhg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gpejcbgwo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gixaogvox.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsxagqqp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gftiqzcez.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gcuaazjbn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gcuusfejk.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gbkusexju.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gbkfuiciq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gwtpfjkwc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gjmkrjthn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gnrhcqsbg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gigsiwsyx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gbpfhxuvq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gnegyanez.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gqgliwdja.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gyczmqhsg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/ghnftdigp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/garvjxpks.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gnjqmswqz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gzhwhzncv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/grscimzmt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gexepbyog.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/ghklkbalj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/grpjyaxqy.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/ggnvwwawj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gvijadpph.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbrjasgee.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/grpogsuyv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfjzoivdg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gqtbnlzgs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gmpncghbh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/goeqyebdm.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvuxzzkyv.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gdkxwhvxa.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpkevpqgn.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzgyalgci.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gywzxhkwx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gishvjgdu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gabtrqhli.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/grimkajla.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpwzlsqlf.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gloeagygq.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gaypqfxrz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gfmqqwyud.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/galfazyiy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gbqlqcmfh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gddzqugma.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gaqifexxi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gkbzjuzco.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gybmyovne.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gqrlrqowa.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gmycjmiqn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/guaefrwqz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gpcbtwrtk.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gtjvfgfzn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gdpchrodw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/giuebtpmt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gxmrdptwy.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/grxvbnkox.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/ghmexzstu.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gmvuushwd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwmgtimgr.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwqcuvjei.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gwlaxnwqp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gaewdxhgx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gtnnuuoai.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gnwozgswr.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcvbhvztj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gwngppson.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gutwnvqvd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gywcrjicc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqtazpwxz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjfuchfhe.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpzkpoadm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gxsjqjeog.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggeopbpen.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gehsxhubp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gpbtvbfji.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gahvupxck.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gijkwuneq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gixcsptnx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gspycszbc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkeknomoo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/ggspvqtil.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gzibdljrx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdzgczjzi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/giplejtba.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gqyltfsha.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gihwkdhfs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gldhqhscp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gbxmpjrov.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gnnxfdgqi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gnazmjava.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gccdayely.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gswjwwlja.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gynagdogg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkxhrixeo.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gqydkrxqv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwubqlceq.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/ggkqfeclu.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/ghbnafuen.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gjtozcqly.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/godffftal.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/ghdgirhmj.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggipulaqy.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gubgsczgr.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/goyiuzepn.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gxyvhcdjk.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/ghrqhqlwx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gpeaijgdv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gzjdrbyki.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gojzuojkm.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gdntriftf.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gdhwxttii.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/ggvwcrykn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/ghkuivibs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gpwotelpi.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gzstmhsef.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gbeghckth.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gdwodxwfe.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gokbrzqmb.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gcwddzfnc.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gcfescgjo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gjhqbxjdj.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gvfvaorls.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gomwypemq.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gjdeuxydt.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gjpjcigdr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ggdwlgkcd.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnjpgvkky.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gpovzntbw.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gjwpfrxyn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gyugpvtkn.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gcisensnh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gtztcfsxd.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gvbzygius.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gzskbvnlt.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gzrmtqywv.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxhzfxxsr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtritrcdo.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gwcsbooly.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gutbqbugx.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gqbqvzave.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gfyqpznfi.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/ggsqoeicd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gzzbhmkje.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gdngxrqer.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gqkdsldxy.sHtML


<!-- 参考信息 -->