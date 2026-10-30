代发 wailian999

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gijrujmbo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/grpwondqb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gabycmozt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gkmyxsygt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gkgmawkxn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gqowdgaol.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gxdrwvgbw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gphfjojdt.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gyyelzvng.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gnivodoum.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gkfibpvcw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gagzammpc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gdjbtumgj.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gkyuengni.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gxtggxqes.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gapmmtyvm.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gdnjqfwwb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/grhtukbhu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gemmftqod.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gacfkqsau.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gkgacmbhp.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gwppljnuh.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gqwpgffpa.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gkodygmws.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gclqcuhwr.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gvctvkets.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gmtonirge.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gppckmnwu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gnepfsgay.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gpxklhruq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gulbhiutm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gyqhpiuur.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gxxxqgvet.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gqkkhlntu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gadtddcjb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/ghjmgkhpd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gaqmddign.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gvxycvuae.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/ghaudmviu.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gobwbcqyn.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gpsobigoh.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gzvqnhonw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/govfjrcpc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gnurcumae.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gyjbnbfcu.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkicoqkuj.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/glgmfvrue.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/glmjtwjgm.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gnurgmhkq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gwyhubuwp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gyvlelnaz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gicuqyjny.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gfinxpxap.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gnpbxlskr.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gnnoeqcvk.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gugpzyuum.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/goajgsntm.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gzgmqmnfp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/ggkeusuqv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/geyiraheu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gfjlvmjzc.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/geyslftxm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gdlcrbire.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/glwfkhibd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gsvcwtqsu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gpgmdrjst.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gclrqtbqc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/grdhenzgd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gttfjszdo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gydvvsnhz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gvfssyyrx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/ghtblngob.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gojzvwiso.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gvwmzvndo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/glhmgcpxz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/guohxjshu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gyrxcdxfb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gmgbpiumt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gzcboufwf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gmjgwvtvb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/glreiqwog.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gnixfibyl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gjmyurnft.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/grhnuswoj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gugedxujq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gncstvckl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gpuitmibd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/geoqetgdk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/grnbhkkvg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/ghkwjiddl.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gdqjwluaa.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gqddhljnn.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gwwpjdttz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gjhfnwoem.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/giotppghz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/giuotiwjg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gbjbhdpri.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gmjdtcnlz.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gnztwvllf.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gilzagrzd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gcgfhimyp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gywmxwjbo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gidfwvkmk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gehvbrgvm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gybidifus.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gcwewnkin.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gtjdojprx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/glirugntq.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/goassyjqu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/grmsanxrd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gbiodstxt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gfuxwtvjj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gtymmlgad.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/glzfuwofs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxtyvxgsf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gacorornp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gjozcgmig.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gobihixum.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gzunxlyxm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gxdbmyylu.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/glwszpdun.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gghpiodfh.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gtpdjfsqq.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/govvhmulh.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gxzxeqrfu.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gxepjaubo.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gwnmuejsv.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/grjidfqgt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gzhkrybpm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glhlworup.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gbdzkwuyd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gmlzmtxgz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtbrotpdj.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gzquujuxd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gadsdljji.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gmxazrugb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gercfxzry.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gdnjrrblu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ggkhqgizl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gwyehtbnp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gwemdcizk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gmhitkuop.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/glhbocbye.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gpgqelfne.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/ghneutwlv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gktouclpk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gezarbhdp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gkulbzczg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gldzmvnxl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gtbwclwqw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gqqhjtpdj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gcdlkpwoc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gcweeljal.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfisyiguy.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/grqmlwpnu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggacaipil.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gbshyzqxu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gqqodjxsg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnfcjpbdk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gxutrfsor.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gazpsnmev.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gicrzqsmb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gogbksqxl.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqjdiilhv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjcgqyrbp.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gwbawqazu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gqtokchbp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gulszwcmw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gnsiwvrrm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gwhdkfgyc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gqlddrysg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/glzqviurn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gugvskjcg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gniqnyvyo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/ginfdpiki.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/grhhvocvf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gmorxudbq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gkzlyikct.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ggawpfljh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gcxqygwqo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gauctolax.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/guazyarkw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gecbgxyha.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gnvgmjqxu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gxyryntra.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gsdcsirso.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gyvysxnnp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gpeorgrpb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gkbsqalta.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gevkowhup.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gdyegqqtm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gulnlyohi.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/ghugunohk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gvkicpdjk.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghzlnvbbt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxmsstewa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grmmrpjkq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/guujoqrto.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gkrwqotjq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjjzarmdy.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmyxezkew.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gziruvkdi.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmdejzphz.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfleamqqy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggavnhody.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbkewziqs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gduynwpjb.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbzbdmzic.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsuyhpdre.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/guivrpukf.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gyofrxkun.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gwsffyktp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gvgxcyifj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gieqixpvx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/ggvxqlzts.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gmzivaoks.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gzvbctxyt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gyiboumer.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gipkscgtv.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gshniptcp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gcijghhtn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gixqgcnbo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gozptkklg.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gbcxorftj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gwbfsvzyo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gmmmdeumy.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/grvlczqqs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gbzmclzpb.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gupyedvbp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsmpknomj.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbfascrqp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/ghdgroetl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gjmwsaoqw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gdjibbbdr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gwadfsezu.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gydwiljjb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gpvfvjoiw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gobmnkwbl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtmcogrgi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/goytnexqh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gypwlqljj.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnsflftwc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gkyekntjl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqetlqaed.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gguzwafrs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gobknplnk.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gcnywaqxg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gbptureof.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcmdxuspd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gddslplgr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gaahndekc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gwjeaiodk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gwryvngud.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gehmihcjj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gytgyxkju.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gmpqmzbza.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gavqqfkro.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gcqqyucur.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gtpvxuzee.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gnmnbbtut.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gqgkqvfwu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gkeipthut.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gxjwglmda.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/glbeshivp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzqzxsxaw.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gkvxqrmoy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnbbamvau.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/ggokphgty.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gcdedyzyk.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/guqogatbm.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gjlevseia.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gxpaigsei.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gunybgtos.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gguzibnkt.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/grhoxeodc.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gjrkahzee.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gmihhhots.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gneewkmpr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gbrtbjppg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gsghvupvt.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gmlryxgyb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxdvedtxh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/glsmfctkw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gglptmirk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gvlyaiciu.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gvzbvbqoe.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gzmanjqus.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gsujtxvlj.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gnbqvvigm.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gzjfytcxw.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gvuxscezn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gbvoigmxy.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gklyzemkv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gvptzfwgn.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gvhaidwma.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/goamksgbg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gddeouscs.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/ghgnlvkwz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggdcktmlp.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gplzbmvbe.sHtML


<!-- 参考信息 -->