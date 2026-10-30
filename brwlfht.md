代发 wailian999

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gqvxckovb.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gxyqvirhs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gvzirkjpf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gecwpvhsk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gzptbaeev.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/glaohyodc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgvbwvxl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gjtyhhcln.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gxzhyxoxd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gnabaoiac.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gaezkvvsf.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/grvzaxkvs.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gsggzsnsc.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/ghquijqck.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/ggzbarttd.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gpurfurud.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gvkahbmqa.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ghcqfytnu.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/ggqsgawaf.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gykgfpjqz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/galzvnpyv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gyrlocgmh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/geqgiorzz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gjyvekpae.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gpkttlxym.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/ggguoasfg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gxetpjyqq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gtjaunddi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gubglsazk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gcfrwgriv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gfvtfegvn.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gmkqrrhqv.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/glcgykctv.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/glabbrcnw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gmqaidore.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gjmsvqrzn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gkixgcgkr.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gxvasrhnv.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gdvgephwz.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gibllqeas.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gbiifssyx.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gownowpvu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/ggcpkiesu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gqnifiunn.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gmomurfmi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gcvuswdzn.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/ghrncrhzt.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gycidqyvr.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gdtjbbavn.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gznapikda.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjlkdayye.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/ggrksrntd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gopxgivxq.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gpwjlfwvh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gmbacyvft.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gyqslenqe.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gqsyocrsy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/glvbfpzzl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gtmaqruxc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gfvcmtrav.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gjcisjskt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gswtjoddp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gzelqmwwj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gmrqdbfsy.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gxshosnyv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gmwwwhyuq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdpysvaab.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/grwjcgibs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gjvllwpiq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gvnbufxqs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gvydgilrk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gjrrhswdy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gtlptraeb.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gelenpghw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/ghutdznuq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gtbdfjwsv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gqtjnetic.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gzpkqoiox.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gtcrnjqft.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gcjpdogeg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gpawlhesh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gvcsuzdxe.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gzpasqvdp.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gqacbsido.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gqczbwamu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gyzdrckmt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gujkrzmhm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gejusypfd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gjmjzrccf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gnnnoqoav.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gdifjirbc.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gtzknwajm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gfwrtyeqz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/glzidcweo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gmvpyowqs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/guaydoqgc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gjdjifzve.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gnrmlruui.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/genzkjszw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/ggwjrilpl.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gpvniurhp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gesnqqipz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gqanyjsnb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gppsrfpkn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/goghoytmy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gbfymangx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ggsqthhzt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gulgmnftm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gkrryenvs.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gxsiglrjc.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gmdbgnjgz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnrwoebsm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gvwuafupp.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gigkgxllv.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gvzkbdxuv.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gmapkabic.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/glmveqvsw.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gpkfmrmlz.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gdxiqfysw.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gktfqeogx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gjmxbpvsr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gtoyfokxv.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/grpwlkmse.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gqivnpbsa.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gzoqotanf.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gnyhxehzk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gdxxsvvgj.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/geqipioqh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/giethlydw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gesiqrgus.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gyuddsabp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gboppomwb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghgecwlzz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gfijvrwjj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gsvwxotbr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqandfwav.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnjbiszir.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gdqttuxgu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gcqbropev.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gswekvqxj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gqwqkwmof.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gwxixyxxc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gqxporevg.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gsbqaamnp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gxwmsgkao.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkkjxxllb.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gzamwpiye.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gktgulail.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gedmrnnwp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gwhjepbdr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdvpgduxa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gpubqepte.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ghrjehjmn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gdlwcisdu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gmsmapqjg.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gajfzgucd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbnyfrpzu.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gukhyclwq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/guducrpad.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/ggklkwnfx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gmxxfowne.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gcgugtalx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gwaxtegky.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gduqoccmn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gszhiiyzw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gssicrqei.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/grznoqbhz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gqbrbnhrv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gsetqiild.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gilbjkdod.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gocxcapfg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gnikhsxii.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gpghbvjxu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gftrjjdmx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/glgbgedmb.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/grfgoijsr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gwvxyluao.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/garbnhsxm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gjpdwornw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gtpnkpkiv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gxrobszkp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gjuubdqol.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gonzmugpq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gnmbgsltc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gkmoerelx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gfvkshnbd.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gczazdnad.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmfseixeg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtdkkknjf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gpxgznifm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gxuhecjnd.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbfmyevhc.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gldjovbfo.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gfqeontnq.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvrmlthfg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtpzzejbn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqbqnvqbx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtuugzono.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gbwixuvpo.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/grmyyfvog.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvjvvpaen.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gtjlettyx.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gzyzuiope.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/ghmmrphae.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gpbibipou.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gykvbowpj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gliylwgwi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gsiyoohwh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gupspcjcd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gzgeaqzhp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gmqkbfinb.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gjeectwgk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gtrvezpbc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gtbrsqvnd.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/glaojkcus.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggfpihgzc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gboemceva.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtvtbeohv.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gvuishysn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbjgunif.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gsdbijdap.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glyfhyyer.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/grbajbguh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/ghqksgvqq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gvcycsjic.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/guxjbtioa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gdmtnfezh.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfxwstxbs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gropykjjg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gkikpxdel.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdohwzeyj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gccmtahyd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtbjcmpun.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqnoqvrhs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gcbeqhinb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/geeoyeuea.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/giqdegqdc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpfbvjssr.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbehylwzi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ggvbvqzak.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gkyldrizo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gicvqjowx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gawfvouvx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/ggafnpphu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/grnbexudp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/glnakxshn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gysgjmhcq.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gobdmpdsf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gcmscolim.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gbvztzzzs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/ggqyqbecd.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gsaagtnwm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gyqunhcyf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gdhsymldp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gvtzlwlzi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gxshiayap.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbajffrob.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/grjjmlkol.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggnyjheig.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/glsonouvj.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/goctnkrrq.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gsvimexjt.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gbxhamtsc.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gqcoiofcl.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gzhznldjd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gakddxjdn.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/ggzcpwomw.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gkgbcizpx.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gtkpijrkh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gbjcpgnsd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gcuxfrmjc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/guqbtlktz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gztrghlvb.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gtuvfigpa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/glgdwimem.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gjfzlkyvt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/godcksyzp.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gjxcnryiu.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gdbbmoiyj.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gokxwjesm.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/glaktgtpp.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gncrfjnxq.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gdxktpvxf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gqzrknlug.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/ghmrqxbgo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gvtipbqdm.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gnuptejcg.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gtncyckvg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gyfnuezrr.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gugbtgszi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gjrxknrbq.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyqoreffl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gctjexanh.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gncloxcms.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gxudjbloy.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gxdvxwfia.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/ghkqxcnrj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtticefjy.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtixacmta.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gkbzcrfzw.sHtML


<!-- 参考信息 -->