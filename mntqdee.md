代发 wailian999

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gfomiyjes.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gipgaphxg.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gwbhqvxpv.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gpnzyfisc.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/grtkwgkby.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gbnzjyand.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/ggddigmco.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gsxbhhgix.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gbqziddem.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gdogwanom.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gfwqnekox.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/grfecykhu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gfdcfeqij.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gffspuvoy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gwgbuviay.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gtkhrwbbf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gbgfkicra.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gzfxlknfl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gandzqiod.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gvnirwoge.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gklzutnjh.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqyydhhfu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gkchweieb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gwgoyscpq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gdakihuyi.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gxltskfpy.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gzkvofliz.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gvnwibctj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gboixdytj.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gwvqvjpfi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/goloeugnd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gmdebxvip.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gojfvsgow.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gezghygbk.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gdljbtdnj.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gzxqbxlzt.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/golsqmsoa.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gfyahlfiz.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gjjdlfhsa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gtebiqdle.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gogsshsrg.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/glfmyynwp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gmsloacca.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gfebaruwh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/guwnupopf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gadqefgsn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gsufmkxvw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gojfoupke.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gdlnkqjwz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gszlscypt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gqztpzyys.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gpkrotetf.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gcjzlryiu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gfeabmhhj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gebfahkzh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/ggczgytov.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gsacxcdhy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gbdgexvlo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gkhtfzjms.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gtcrzxrrr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/glmyruykb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gklfxtxti.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gwvstysoj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gcslptxde.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gbwdabdlo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/glmmblagg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gpsmksquh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gwuansavi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gtnlyzald.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gzrjyzfhq.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gejqzqcmk.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gkoiapjdd.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gbxlypnqj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ghsmsoovk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gzkpblmsp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gpiawgrag.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gpjijpauj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gryywmphp.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gvthyssxb.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/ggfsgrdbx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/geqphjajl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gmmptvhio.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gzexuhrbo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gpgmiasmx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/greuxxggr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gabsasgmp.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gqttnjpan.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gvqkqnecz.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/guhiuxvpi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gsfmiuieh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gdwstrnnh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfjhyysrt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/glyizjrbo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/grqjslwyk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gncdceqrj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gsxwirmmr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gktanzmlm.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/ggtqgxidl.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gegogpfqy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/ggghxozak.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gdbulahbm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/ghxtbmmzm.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gzabifqjy.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gttsugjki.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gepaxfuux.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gvwswuynb.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gdoaafacz.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gxbwgssss.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gnboxonhm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/guofcvjoi.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gqjosotxp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gkaoehjgz.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gpklfeskj.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gsznxmjiz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvzskwusz.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gquzuzfyg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gqivglrej.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ghgpbqcvc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gmcwdqgpq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gltgznlrr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gwxacjate.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gdbuswtnj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gqrpcmqnq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdxbvjrgc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gykzebzwa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/glkwtjpcm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gukawabvd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gfghsufcj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gazydvhyj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gyhzvqgsd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/guylzlqee.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/ghdzrdijb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/geaphdoft.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqfjnctij.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gjwerkqkg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbzgacpnv.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gkmnanuws.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gvmszddjx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghsxtdfro.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gvfwneelq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gzxwyfamj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gvpqwmoqp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/grhlqfjhv.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcexjjlmg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gstrmhwha.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gmujhrrej.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gcojelywv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gefdqrvuu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gtpkatmzm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gyfttamrw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gypfhhriu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gjlbjbeds.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gwkjyuval.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gobhscvbz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gesggoybm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gdddvtljf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/grgtqrbje.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gpslmknyp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/geyfedcok.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gvbupnoqf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/glgnbuunw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gcwmbmywj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gnfwbnmqk.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/grbewcmmo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gjdjuzhiq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gevrmxemw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/glgqmatzv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gnrjzncwm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gtmpjzoot.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gvznnddfu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gssnvygci.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gsbwbrwfi.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/ggqypcgxx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gwoobfmhg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gercdmaee.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnufnxobw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtbntxyvi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gbrtdngev.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gxvkzjpan.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqxrsmsnm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmeyleuap.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gmwuibqbn.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvuxrgvuj.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvuobacdv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gomnolova.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvfwamwks.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gmuhyqfjx.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmqtghybe.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfuwodncg.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfcmpgsxh.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gwanbsunn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gdjobibqo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gydyccnld.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gvcyqfsox.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/geqfjwbap.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/grrrskkai.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gkfxjnwbl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gevoknslm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gujearfhr.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gtmtunnsk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gtqowachj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gggzdirkq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gdlzipmwn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gznvqigby.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gefgbgzfo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/glarzfrrn.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/ghqrtkxeo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gxcklnxap.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/ganxardpv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtialojyw.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkadyhegw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gwfkfvvdj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gyhdobsdm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/giddmbbtg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gzkuckhno.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsmksgsnp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gvghqayzn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gtovlitiw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmbsvknad.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxsagpmul.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gymxzpgnr.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzawfymfs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gvldnqwcr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gojomolsa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/garwgcrbr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gutlxspup.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gpkkelpjb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gpehzzxqv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gvqepvqmg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gbshtdopx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gggwvuern.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gdtzbnsub.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/griyitcxv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gcftvkxot.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gwftgeiym.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gtnpupjha.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/guyinkgnj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gyxfgobky.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/giheuhwrm.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gyvljihps.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gwzuvcngb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gpuohmdrx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gpbdeubhg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gojboztbc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjqkywcek.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/ggyjxnfdt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghgpqtppe.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gnmcnoxwy.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gqczjlsxl.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gtznbtsqv.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gtkgmrzat.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gclggspvu.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gygvjjcsy.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/geveztetf.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gvrfnvdjh.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/guerdrewd.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gpyeoftsc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gktglryeh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/goabcocyw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gkbthdpdm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdumcsbke.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gdlvrymgt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/ghjsjrrid.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gpnnrnrug.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gydedxvor.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gftejswnq.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/guafnvjcl.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gsrddacxz.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/ggrxaaxkf.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gmcecvaty.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/galdgrtfw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/ghcmkresx.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/guosanbsv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/ganujhgaa.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gbxfdibev.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gmubcasmn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/grkuwcqju.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ggtelesrg.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gjmceayqa.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/geogtezpk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gsnjttdwr.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gwdwnzpyg.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gfaonbynx.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/givdtpgsk.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/grwflyyxa.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/glgogzxuc.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gmknnmaii.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ggeogehjf.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gmzzlezsg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gnehiwaut.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gjzwmpkpm.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/grobcdhwo.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gbgddxksb.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gfonjulzl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnpmkqbjb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gdhtrnunl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gatuxayxa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvskxrkwx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/guqfoarxv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gglcwqmyt.sHtML


<!-- 参考信息 -->