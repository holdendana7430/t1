代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gixcwtrvs.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/ggxshcgxo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gdpknmgtx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnveaodfj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gedosxdbd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gtpkrgxrz.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gcwpbdzkb.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gpllicpcp.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gqafpkmzg.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gretxasrd.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gmbubnppa.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gmhjbrscp.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gfdjuollz.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gyujsyeke.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gglfexdbk.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gvndjzddi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gvubdfsem.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gzkgnrraf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/ggalymtmm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gsmmvalgp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/ggtuozdgt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gtwuzcuvr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gdllippdc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gukvzqaib.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/ghofuarcs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gkpjrghnp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/grhwpfiho.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggmvsqwvl.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gvjwzevsf.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gjewbwqgi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/glvuphrvo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/grjfzcffp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gauppgbzx.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gpxhqrfyo.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/ggdaarzdf.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/guhupkdic.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gxqzfozgu.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gxwrjvntn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gwwfhbwno.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gdeogsdaj.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gktuitkgi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gflzzklwu.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gbxtcpgyr.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gjnxeeibe.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gvazcredi.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gghtdlmvc.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/goezwzmmp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gofymyneb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/guniwbgzt.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gfyjhupgu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gbbuzqtcg.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/grdgknkxw.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/glzpbssui.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/giprvxiat.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gflnftvxk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gbkhftprz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/ggzonimxe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gqzhhqhwr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gmpzlbcon.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gsikpxhnu.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gweunnnor.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gxzduhtpf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gwwhcmjgv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gyluyedvv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gftjfugsm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gydrrexfd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gbjxqrwzq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gvfivmhug.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/ghhjkievi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gqhhehmqp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gmllduzvu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gmrjqwtln.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/ggdxccbmk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gpmbxwpom.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gcfuzhgqy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/ggyzrijqy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gycbuqdou.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/giffecqdv.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gocmmrfdx.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gesseaeab.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gdktjjbat.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gmvohbbxx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gdzettkcr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gbxrxbzko.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gualeanth.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmzfluyuh.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/ggpyjzjgg.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/grdixablz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gpxkbyzic.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gxmqsoovg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/glwtjufzh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/geixggcbn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gfbidngjm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/guvnrdrus.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gdlisamho.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/ghuuibkgv.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gsdnytgmf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gdlzntwzc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gkearqzzx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gvnwworcc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gxcdpgvci.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gmstwbviu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gataaoila.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gkowmkdcw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gevpmlvzc.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gahdnotws.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gaxptoybw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gndhgdswj.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gbqabpffv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gzbgzddow.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gofzbqfpz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gqffzrvhk.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gbdihexvh.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/goclfrwzy.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gwteeqmod.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gmxrtpwla.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/ggioerylw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gtpzjotof.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gepdvwyim.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gvfmelbiw.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gfgqmxglq.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/ggqplomeq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyhwbetnz.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gouvbaoiq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gpgxmtdcw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ggmjjuldk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gyhpeqofj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gfmbshcdb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gopphkldn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gbinbdnzi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gldgjlkpn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/grxwfggkj.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/glunnagle.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/ggtgkrxys.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gstlisfqj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gixatuvcw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gksjdelus.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gchmrwgtm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gbyycoqxs.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/goycjbzth.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gcujetuqw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnlncuyii.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gitobqkwv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvkqpiuuk.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gbrabgsvy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/grzwyfkbn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwpcgywem.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gpckpopor.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gghbqikcz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ggjpumbvu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gbgvldyok.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gamjugfrh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjgvvcjex.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/glrkvkous.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gcikjshar.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gcwrxelhx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gduvvatxm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gtlpmrbsw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gcsfuundh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/grzywmflk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gnwxzszjq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gchembmwg.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gsmiwhegy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gdhrqdjio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gpfeuqirz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gnqlhrtii.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggjmnuhra.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gawpacecx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gcoamzfya.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gqyssozhi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/guwbklnrl.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gygtsxnvd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gchswxfkb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/ghdlxwqsj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gnnnjnvjc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gxivfyqhe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gmtxuzmca.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gelqqxpjz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gaiyztijp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gfizmlxwd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gptklkiwg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gwxpjuubg.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtsswftfj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwdqoyceu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxardpnvs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gtkyovjey.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/glaottahc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdjlktpck.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkqynmnaw.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gekegqdoi.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggbcrxohm.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/grtquxsgl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpcnfmuvm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gghsoezoe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gbsnahtcl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxlvkenmj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gecftrkdc.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gftjbrbfm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gdnkcvxed.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/grksdfodk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gkawjlghb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gzxewtltb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/grtqtqpvr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gvvdxmhok.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gdjlmyupu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/grffpvicz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gjyqbqaxb.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gotblybby.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gmmtmkhlq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gpurxyzxp.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gxzyedvyd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcvgmhxmv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/glhzdaqkj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gsvkspzpw.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gcywszime.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gktapktqj.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gielkxjcg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfkwpjiyd.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gicmlnofe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/grjfcdtrb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gkfxnupfm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gssvxlfco.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gflhfamvu.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnewvwtor.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gcywygsot.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gvbyyxriu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/giejbbdia.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gggiszckv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpalfenmc.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gamxdyhpc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gntswjhab.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giwiijrwu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gywdlfjnk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmqldmvkn.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/giynvjbta.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/guqqykqpi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/govvearyb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/glnpbmdrk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/goqvugwzz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gdjoxjotq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gjwqqwjwz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gaaqfzokg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gzjezadzi.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gtboarrcn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gibhykslp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gvksntphe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gfjbbddfp.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/grudxgnmh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gjtdlmgla.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gczjfmrlm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gmlnymcth.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gigxuzwyq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfxrcxrkm.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gizwlxdun.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnyimhvbx.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gydyogego.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/ghrupirzi.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gwtxkqbhn.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gxvpkbmrz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gfpexppoo.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gtjgedjaq.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gtdouwttz.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gylnsxcng.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzejdfzll.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gmduunkku.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gvcglezaj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtugyxzrd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gtlofixjf.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gnebktuly.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gdjcsixjc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gxroitvrk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gwnrcywrh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gxeqhnudf.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/ghxtobira.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/grwqryreu.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/govonxwjn.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/geqwyxckj.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gqcwibcxd.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gfosgtlqa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gdskptdyo.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gpmqqwpha.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gignebxeq.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gwbrnfwhx.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gpzflvyee.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gpdrxpebe.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gqixdzvlv.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ghomwjirl.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfpuunutx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gbdjtnfub.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gorsezmkj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gygaifmrc.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gjunrptcl.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gnzgdwhdt.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gwtoecuux.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gncplhapr.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwptqihee.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gptjtvyqo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gqbganmyu.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gfnyegmac.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gitsxwxwh.sHtML


<!-- 参考信息 -->