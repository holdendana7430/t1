代发 wailian999

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gwyhokfdn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gzaamsonk.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gwsnzsujz.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gevamkaxa.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/glqkdoiog.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gjqkwrtva.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gnhhoufyt.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gnsxrpbgu.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gmyvchixc.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gbcnwmpat.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gjzcikoxm.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gfveqsfze.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gpdbkkvnu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/guzuzebih.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gpaszauzy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gwsivzvny.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gelvdfczu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gverctdrq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gkkspcxbs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gopsigqsi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gxitahwaf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/guwdbkqri.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gmcpuesjm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gyqancaqq.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gtsrjltaj.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gckawwtjq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/grqrkxemh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gcutlvixa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gioowqwkd.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gimprwdra.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gpakibdcq.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gaznnnwtx.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gnxjmttjg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gjwdxseki.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gbvwerlxi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/grmrlhphf.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/ghjqxzmap.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gufssstsm.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gnmodxkno.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gbcdmxgkp.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gfvzwdsst.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gweecgmzi.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gdeqnavbc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gmvgbyblv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gveewjgbf.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gnmfjwtnm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gveoauslr.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gywscqmvw.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gwsfroumf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gaufhlzkg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gqbxfjsoz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/giiheaahx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gxantzxsl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqzrwgcfz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gpbwyyaka.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gpufonyia.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gfpviwhdu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gqwkpsoox.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gsrohbich.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/goaryozoy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gcrsqqlwx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gvpcyykan.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gzdcbuchb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gczetbsrm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/ghqldunqj.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gmiyxwshz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/grxjwroly.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/geivjzead.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gijylauwi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gwxqtscbf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gpywdznna.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gxsasewji.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gotukkovt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gnnvrjdhl.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/ghhehfxdi.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gtcoosmje.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/guxwhgmqw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gdsukhwbu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gizqnblfh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/grrqhddbr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/ggpbtihvw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gnsiqiwcc.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/guqzwjrld.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gyzvhimjs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gordxrdht.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gjtivjngq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/ghoazybii.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gtsdjedtn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqnrfszms.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gfavxbzfl.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gaznqjiwx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gtcnsfhnz.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gponiftkn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gczlhhner.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gvnqalolp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gdwpcvxea.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/ghnignsic.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gactdoahf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gbfwpslfk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/ghtyzrswa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gutdkabnr.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/ggvmvrado.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gymbxymaa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/glgqkqfmu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gsxokdbzp.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gyqcfgyue.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gotbtmiwp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/guakbdzlp.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/giyxdevlz.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gbfrceysi.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/glgcgtdue.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gijzrphgn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gdevgzwdg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gexccnjmv.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/ghweoexmd.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gcptlsivi.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gtgnzedld.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gpkavuizv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/glxaiwsuc.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gmifhbukl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/ggbhganlp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gobljiiqq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gewgsyvww.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gzorchupa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gfcyeubpw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gcvuyjtom.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gnlarmsay.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gwydtlibt.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gvrccmyyw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gypljpdsp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gwuewxsfd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gqcswyfen.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gmlvcdczy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/grytzppxd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gyvhzfuvs.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gzkrlxcxb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gxsrnkqkd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfmrkrhww.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gchlyuyhm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdlddenrr.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/giaqazuus.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gobkszjgq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtnydkwix.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gndphdhfi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gdfkfdxjw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/goprquqtz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gmsjygzcb.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gipyraopl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvxkehyew.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/geduivgqi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/guqckixlg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gjnohuiqg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gendonaes.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gxczsclui.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/giovgoiqj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gvejfmcwi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gsqanixpi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gsyelpxgb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gprccvfwx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gyyoswmsa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gxoqzjedt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gpyjmbect.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gvhngmbgy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gctkhwnwn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gdcbypxsh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gsgoezzpw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gwfxicsfr.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/glpsgfcql.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gwdxzobgf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gfwgmcync.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ggkmekdab.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqwtkyaqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gpyzzoxco.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gugkcvdud.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gdvtlkvbi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gkdpeosvc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gbqkbnixw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gfogtmylc.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gltvcjspg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdqbnsurm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjmeklhdg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gbbfksjyy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gfbicaakt.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/guydnihap.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpmmcgrlu.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gyuesipqs.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyhbofaln.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gppaolzdi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gklorlnex.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjwqpnrpx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gxzbkhxgh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcehxvqga.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsvbnpvlb.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gukfravaw.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gdvawxcft.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gjourbmpl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/ghdjaonsl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gppjnnmpd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gfudeqhlv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gdguvslak.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gqdwszhyf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gdyvhfkwr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gbzqeejhx.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/glfuczkes.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/glegkehjt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gchxqwpgp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gyokjpkxf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghrmysbfx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gjztjfrsg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gzexxemul.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gslitkdnn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gigsessmg.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gyrcahgts.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghrkfqayv.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grekfckkg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gapnkqvrb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gkunvjrgn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gvdmwpdpj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gjxtrtlax.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghmyjpkcb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gldgnioab.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gzlzfrniz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnwdpguau.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbqavyizt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdfqmylhf.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjyiqnvsy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/ggsawmnsc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gltawmshz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gommkvdiq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqmsdisot.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/glgxcxfhr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gbcdhkgkg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/goaouybet.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gjrozmbct.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gsofpnucj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gimffdkop.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gzckxeavq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gnczsivml.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gaajhxerr.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gvlpwxdjf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gbwywlxhw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gjcbiwgip.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gpmhzbcfr.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/geqsftezd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gvqgliswv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gnmppdgar.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/goiwkhrzg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gkfvzsavo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gufnlgkvb.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gdmjwksxp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/genncwrko.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gkpictfpf.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gmqqzirbj.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/grcvtowio.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gjgkeasub.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gddovxdgc.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gahdfsbsb.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/guccuvifo.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gjesgcfxe.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/glzkndwme.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gelmfenen.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/grxaxdeoh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gtvdlfgcr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/giksasdgt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gearlbtgk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/glzjjeica.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbzjabgp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/grscjxkgm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/ghkrvhwpe.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gbpebqrhm.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gknccdqfs.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gdwyuqoer.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gllvtjzco.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gmxzqsstq.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/glmvejjwn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/ggmcuwtsr.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gpmrhnppm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/ggpytcwmd.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/goqrtglxx.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gmekkiirj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gowqpzqel.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gfsopgicc.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gkrylhyxq.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfhqijxgg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gmghgrpee.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkevydaew.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gvrwswhyo.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gwuzojtpp.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gfjxbsaqs.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ggemowkng.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gvvlcdqkn.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gncwduord.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gpwcgvkzt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gcyrapbps.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gxaexcsie.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gsgjxihkv.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gqxmbfjgv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gwdzvszjy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvhmgghnu.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gpjjnohdu.sHtML


<!-- 参考信息 -->