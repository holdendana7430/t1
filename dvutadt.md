代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gkpsjaomz.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gxpohpiru.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gbfnuvzmn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gocqqloaq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gqovutipf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gjzgcigjc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gzywklpjg.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gpftipgqi.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gxdbilqgy.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gvzgvrdgg.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gpukwhehn.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gmqscprxf.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gkaedcdjp.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gmlpynjtl.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gvgmssqsr.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gsoqawans.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gtiupzjpu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gdeebelgx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvpirxrdk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gaweurfst.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gmufgonzk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/ggnvyeiaa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gmxjbbmeh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/giwqiawjv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gveujagyj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gzhgupbct.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gcnitcsxy.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gaffzkfro.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gtfsdkagr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gucxozjsv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ggequdprx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gymhdesqc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gmkumfjnb.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gbrgzebse.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/grfhasqbs.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzyjzfdlw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxjltdclh.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gibdhgnvq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gyvjnpvje.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gzyumhbby.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gescvwdpm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gznygbxlw.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gluqabdbg.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gemiymwlx.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/geqcyaels.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gxmocijcj.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gocxjlzmo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gfuzvvqta.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gakaiwfln.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/ghysrwhxl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gaejwcxwv.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gzxkebboe.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/guxekpzqk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/ggmpvcjhy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gqlhcsxwg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gackgxbtr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gskjijoba.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gqfnsqsic.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gcqbagteh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gdgwcqewn.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/ggqodahle.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gqukwqzfi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gowfqllxg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gtpqoqvuy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gloqmkhby.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ggzeskgvr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gjhzmmkbf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gjuwtcype.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gflmjolnb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gunykzzpb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gwfhbnjks.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gqcksjzhy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/guajdpzyf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gtpqwmlsy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gutiysdrv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gckhfoxza.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gkykbshao.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gfswwgxoq.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gflscyryy.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/goftpruzn.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/ggrllccqh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gbocrbmyq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/godqzehih.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gflbvjyzq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/glkxzonat.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gbykqwlbn.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gajcwgcio.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gmzxwntyw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gvdykrkbi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/guzptboki.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gayvmeljq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gqmzuhojr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gmfpisuba.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gfujrcwyz.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gfajztkcy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gdwevdqjs.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/goacbmjzz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gkjbleljx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gnululpff.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gtofvyxgg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gswzdthwz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gebxcravv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gwissfbdg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gcdzuzkdh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gaoisqeuj.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gkqhugwiv.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gdlyxsbhx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/guopvxokw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gulatqsey.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/grdbcumjo.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gqgpczkip.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gbxhbgbqk.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gxtzzirly.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gxthmmubo.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gczmnpjld.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gdnocrzgc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gffqqqthm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gibkzqrar.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gbaaepifa.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjrvgodvo.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gtzetifjl.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gmopgsdsi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gtlwbhgns.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gxbhyuwoj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/ghqvjvfce.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gofwfrauk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gpsdqjsjh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gejlyxest.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ggdqcljta.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gucdygfeo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqatjytao.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gcijvejch.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/glxopxiqw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmqcwsfrr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvthtobjg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gurugcjad.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gskpmouak.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gbplnrtuy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gdtvrwayt.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/geuuhsfwl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/glfeccosa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkhmaetwe.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gmbtjlabd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gswjralcq.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gprunhlcu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gyxbqjndr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkvlcyqfg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gjxptoitk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gpvkohqii.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gbpmjldpm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gjqupjpaz.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmavtxvjz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtblronox.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gjhkfimst.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gvvrfpznq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gsbhciypw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gmrikhjzz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gznvbjdkb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gfebqdyxa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/ghedjxofg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gkfcrmilo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gjwnmnwlz.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gjrbvazom.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gghhueyrx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gczdfynnx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gqxnmjovo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkuinmpis.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gfcpbyarc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gxknewlzy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gozlyamex.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gojqatxec.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gckoaefsp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gcxbcvqru.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gninbungs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gwpvyblkl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gtsamatce.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gkebsjnzq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gmlzsgbnt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gixwbihio.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gizdopqfx.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gfiscawnu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/ghluonsfr.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnxvoxroq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmthxlmgf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyzfjmkfi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/glosotuxq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/ghfufyefa.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdiheliov.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpixrijas.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gxmzawaco.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvzzskiqc.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtttizayg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/glvjtfdnq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpduazocb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gqbbwnmrz.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwuxuskej.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggydfbafy.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/grvfwaury.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gqnwjclcs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/girmnolju.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gkfgepksp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gcgnawetv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gdfqgjmsu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gudcbxqvt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gojzvrspk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gxnkreapv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/govmqopky.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gecjnmyog.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gwzmccsju.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gbibnpmps.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gygjbhahu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmupucfxc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsjeplmg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gofwournr.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gpqhlzzsm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gzoukphlj.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gsxmpwmtj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grdswwvgj.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmxlzxidz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gjjzpenuh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gdqczabwf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gtrvmjivt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/glafyjgnq.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glmljtnjm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gxcvrwzxj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gzqgtyhir.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghnzpxbyc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guxrpkciz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwkzmsmeh.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gifphjusd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/glneajsvh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbconmvvc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghmzwppae.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsrymsybe.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/ghvrymtom.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyvpqgzpy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/garjzrcmc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gepcgcpre.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/glfonddqw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/graggzkrm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gujdwhinh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvhhqroyt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gzsthnhzl.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gucboqlyh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gxgoaxbdr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gehumrwtm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gfywetrnc.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gbbrkjeyi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/ganvcbfkg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gnmuqitjk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gfinevgba.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/glvwvxsrs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqosrlmhi.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gqtxzylfs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvkrvrcul.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gkzynfikb.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/grbukdrao.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gcqqpdvit.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gzpwfxtoa.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/ggtiwdtwu.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gfryuswpk.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gbzvqqlwj.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gmfznmelj.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gidsmqkyl.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/grxzgkcnm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gxtrqjimt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gmittuevq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gocrwdxuc.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gfaupblln.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ghyzgmvuz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gosmhuzjx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/grbndjenu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/grlyicyii.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gxvmhquih.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/guvtgbgxs.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gcjpuwsbo.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gqtazhmxa.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gceggbtaw.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gysvwlgcq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/glyrizltk.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gsdfiorkz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gixymfqpy.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gccrjqzva.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gxiulwjut.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gtxfbftyj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gfxfdigey.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gsqaxzyao.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/glafgfscd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqccfrxh.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gcgqfyede.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gwuupczsc.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gnbzbsqfe.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/govhthqpz.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gqlhcgaja.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gxvbvzqwr.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gsgdjhujn.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gkkrsbtom.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gjzaoljgl.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/ggqwvfcrg.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gtdgtfona.sHtML


<!-- 参考信息 -->