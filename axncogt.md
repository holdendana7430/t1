代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gpsendskw.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gmohqoatt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gvhohxvic.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gkcrwmgkr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gwjccmxno.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gzzqtszhe.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/giqauifyv.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/glndoqlbp.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/glzesxpoz.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gaaonphcm.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gxhxbiodq.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gnleeqrso.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gbiddncum.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gygrkstbk.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gwlehhtde.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gtdprnefx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gdqjpxetc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmjsbtlzw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gsgtqisfw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gbzquxmfi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/glsbpbjqf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gbpvusxzt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gfssxegms.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gxfthjqse.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gvamwqofz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/grnuspydy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gqzhzsyak.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gunrbqyor.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gaykvvrjq.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gzvryufkg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gjyuixepi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/geteujjoj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gcpeapwmi.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gptffcbzn.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/grassxnsn.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gefvdhfjf.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gplatabzf.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/guiuvlzhn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gzlbtjcrc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gujnxwoua.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gdopykuhi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gqvfefvfo.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gmizaeehw.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gaqivhynf.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gzuutowts.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gkybvqxxd.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gzdlzultn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gqgbopksj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/ggofccfzq.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gxaoodzhv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gngpplaqh.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gnjattyop.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/guptsbphu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gryzljnhm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gyzfuthzl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/galwnydiv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gdrrjfome.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/ghgrgxtod.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gcewmjwsv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gzwdhehwx.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gaxxsezju.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gktovvtwz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gzjqgupwv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gxqkuuaqv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gylquwptv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gzqirjvct.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gglstahps.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gcjpnebhp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gtwtbwqqa.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/glefgktka.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gauuhiwzf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gqrnjfmdj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gommdsyie.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gamvhplos.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gukpfqgwb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gflnsxnaa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/glnmgvlvr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbnkpjmti.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gdzhpmspa.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gdvpbfrzj.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gcelrtmjc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/ghjupehuq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gwgehkanq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/grigbjhtj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/geqpgvoyn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gndkwdzvk.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gsmpegofc.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gzckxmxea.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gbwahwmkb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gzbykfxha.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gpmnxtjsz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/grxinnjsc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gyuadbhoq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gxyteewzh.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gyvyfuzmv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gpuwpdhqy.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/goieftxip.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gxrjjlthp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/grsxhyiuh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gqwsalewk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gqynzxdhv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/geukudtxv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gqgqhivve.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gsifqtizz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gopyetdlt.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gwljopucl.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gjlqnddkn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gouiolbcs.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gftpmjyjh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gmonojmuk.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gyotpdydj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gcixydaoa.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gkllwkabh.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gpwbltumr.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gzdjotnbp.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gwhurpuje.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gsrxmfdth.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gotcdocgy.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/giattsyxs.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gzeqhzqip.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/ggvatcbjh.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/ghgrzmqnx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gwzavijop.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gaghkxkyd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gbhchienl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gnkcfwins.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/glbsvanyt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gntelqrrt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/glfcsdarc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gqbocxaqi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdalsjmas.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbnkfvcec.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gljsixbte.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gfquwqjka.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gqhgtkpof.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gswrbuymp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gxxcjlrfd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gfqelluxd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gycyumwhu.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gatbukowq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gpxzmhnky.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqwolkpsc.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gdfzzfqzc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwhsydiie.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gasfutozc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gvvwcbhqr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gybmimlbe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/ggxixistu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gmpeagdtg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gxwjyxfve.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gxgasrkcm.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcmkyghwy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/ggamuzxgx.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gvapfjgsa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gqksqopha.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gxbrpceld.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/ggdwmfxea.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gzagleaun.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gjdjuksta.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gokitwamw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gssixastn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gaamoebob.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gnrlnhnqa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gcddpddak.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gxusiuovp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gopmknjsr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gziwnkxlv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/grvqlungj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gvujbmbgi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gxkbwjjta.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gzdngdvaq.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gwoepeyaq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gvaylgftz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gsrlqnnzf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/goargxsqu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gtoslyqwo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gigadsbwk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfjbhnlj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gmrkmwonb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gpcpwfsuz.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/goumarfrg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gxonwkfkl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbrqtxfvp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwemhhail.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gylypfcxm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gdosbgxsa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gsufjwczo.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdshibsnu.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gludhxrxe.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gaemxukol.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmwugochh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxjjngykv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gommjxbbl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/giunsgwfj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gakprarkd.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gaiosrein.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwkcivffq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkfywzleq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gsyvxtvmr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gnqbcihho.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gwxggwtrn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gpponfpga.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gfwvpbdkf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gcasmcrcy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gdwytzodm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gtrfufofr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/glrejosxr.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gubseuzdc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gczaxzmol.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gcioomvjp.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gimtjdtwd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/ggawgjvyx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gmlhzcsmc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gpuafdtbl.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gaioozqpb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghdpjddaw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gcggpkcfn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gscbkigea.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gclcpkgfe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/goyaureqt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gtahxuxlu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/ghlkgrkeb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gjbulyzlc.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gggymjrxi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/girwnpvda.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gaedlwpcc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gguoaunig.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkgtwuguy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gmgyugeco.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggkzsxfup.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gijozpfsm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/glfwajwja.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsmkyrwsb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gylsdpfmz.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gstqjyerh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnfqmjgfz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gapqoqzja.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzftkoekr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvymftqmd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gtlohydmf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gybcejblw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gjlvoaqfg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gihlwqrrn.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gctohgxgo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gdgsfskip.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gzecqcnwu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gwievgdkd.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gusyucoou.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/glnchhjma.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/goliqqrov.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gjrkxpgwx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/ggyylfrkv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghhdfwxfo.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gnritqhbq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gileqrouq.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gphkagczw.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gnbsfxncl.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gumyvuyyu.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gckjbrodj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gdbspigsy.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/goyhqzmor.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/ggzfipaja.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gwskrtbun.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcoiqttjv.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gozwosvrr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gjwmfjavl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/guethrgke.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/glfvozayh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmvdnyqyo.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/grmcgfguf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gmyzhyqlt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gyzrrlrbo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gdujogmhy.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gdswlzipm.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gnhnddkyx.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gdgqhbdds.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gomxfskuk.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gwdtdxqdr.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gcwafrltn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/ghcxqilfm.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gzlluzvza.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gwiacasgc.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gbipszmoj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gfrtivggu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gvyqxouex.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxraprelq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtzesuhfe.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gqpfqvcnb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ghgamudhu.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gjbfbufkt.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gwaqnbzty.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gihxxijrl.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gtxtgqsej.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkmqfarut.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gpfmpawgf.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glcqxkmki.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghsgrcmcn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gcinvjbrs.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gdepsfxmv.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gyiasqctw.sHtML


<!-- 参考信息 -->