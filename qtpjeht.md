代发 wailian999

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gtmaxzeer.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gxrxvoowx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gznopgvqd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/glvnmxuyb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gunusdltu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcwndwemb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gsilvxjtf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/getqmvsnh.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ggihacjhl.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gxwwquepr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gjxfokuwn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gmudacunf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/guhytafkh.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gjsyblghb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/glhcjhkgq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gfkdrsqtr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gbohpmecb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gvjjfsnfy.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gjbebitwl.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/genuegmfw.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/ggjibxzlz.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/guuirffwg.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gkudrmecx.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gwexntuna.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/glcdyknqd.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/geebgtpgl.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gdxruezvv.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/guzqwrtqh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/glojzxxxp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/guvnaypkf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gyzbynsuq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvdducyfx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gwhexfzfd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gpvokqxcc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gifendtks.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gnmpksvgk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gwuhtdtva.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gneqzarzp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gfpkljnhg.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gvfulunxp.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gsvhtbyda.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gatevdntc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/guylyhmsi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/geajevonx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gkddoofkx.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/guklndvov.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gkuuvfutf.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gwkxeoydi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/glsxrxznp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggkrywvkj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/glrjxummz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/ghqwshvie.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gkwizrqic.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gxwyomkyt.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gwpzxyoaz.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/glvnvcsno.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/goicxpepk.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gmuclhdar.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gtugccsin.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/ggljqcvjl.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gurpflwdy.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/guwubqhcz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gcisxhuwo.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gfnwjpsxg.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gycgynqug.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gxobekcbv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gmbfpektf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gxxojmhfu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gjpbpbnqy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gfnkdwmys.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/glthqivii.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gnocqubhf.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gcaeicuin.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gdaogwrur.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gpkmrnfbf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gmdvgtwqa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gkuxhjqtp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gvlthbnge.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gugpvhwva.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gsfkliakj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gnicxscjy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gxgjrsyce.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/goqnxuhiq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gjcelffvd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gegvumlpr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/ghncdgdtv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gjmpicygi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gtxkxgqgg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gjsisulrm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gdqhctqlm.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gsxsrlduo.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/glcqyrfwp.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gckiymasf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/garrqrssy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gbrvpbhdk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/ggenetugv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gfkevxnng.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gexkxfyrt.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gumvossun.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gfeafxjpo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gqyrxapbz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gukazkhor.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gpwfgqecx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gmdysnsbz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gygwnikdp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/grrwobwvc.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gwmruwzdb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gsmtrvjuw.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gnttscnff.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gesrlsprq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gzhqcyjkt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gvoiummox.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gudxtutyp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ghftrtgwp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gzvhiipio.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/ggfccgmjc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/ghluiofcf.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gqvxthzku.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gohhiksnn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/guljihimo.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gcnfpetgj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gdrdevaub.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gurqxlcmo.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/glgpjminv.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gvhtahnmr.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gibwtyxlu.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gcpjfsxpo.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gvjzhdaar.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gbkwbpqhr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzrmxspvc.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gvyxikzgs.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gyiaysjtg.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/grgewplyc.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gduwamcsa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gkxgvatbo.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gvnwqsnzk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gwwmswcfr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gejqbnzne.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gtnrxytka.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gddvfpkju.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkryqlmpm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gbaxojvvw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gnifmdeal.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gfejsjdtk.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gewvolutx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gezujvqmw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqaxrjoyt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gmyucnbeg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gbmapkkbl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gufbquivp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gjdyfrrwf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gxfhohbua.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gpvckqoyx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grxksxrtf.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gtllojcdn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glzogteql.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gviggqbuc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gquouuemr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/geexkgzbh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gshejmqwa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gdfhnzxya.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/govdzigow.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/ginksrkng.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwqhkensd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gcjpzixrp.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gzuvuvidz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gpebnsaww.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gfcbfunnb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gohcndrhs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gtsfuikbt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gsldnyfea.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/glhceddvj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gpujykgns.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gzbrmhnuh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gdxpkgjmw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/geyhpztyd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gyvdpgeuq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/guoaykznr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gjgjhyztb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gyudcfwnn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gyrpsijnz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gqxdlmcxp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gjswjlgjt.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gsghjfshy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gokisfnnt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gfeddfasj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/genbhymjp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gbmiueqcu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/glrtyurks.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gymeccsfw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gqspwkdui.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gnrwmbrgu.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gisqknkwo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gkmgftgro.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gicpkhcbw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqoccmmhc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvkzlnzah.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/grmavkres.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gfrxlciif.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyrldpmey.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqrimyptg.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gkstnnpqx.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gijorzkrl.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gnkelvazx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaauhgirj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpkqnxcoy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gffuogsgm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gypvrvcll.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/glvybbdza.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdajhqnkl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gevqmacxt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gpomzvuwl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/grbgcgkdl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gcdrmrcyh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gasihohjg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gsqvxvqgj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gdknpfcsv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gbndkouip.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gsicnhgxv.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gducnxdld.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gmxnbkpxf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/grwevsiqm.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gottpggnl.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gjyhtrhue.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/glyjefgqd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gsoldkiyj.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqeowvior.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gtxyewwyl.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gtuxxwnza.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtnmclyor.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grggnmsqw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/genhsjeiz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gektlaxcv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gedatptkx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/ghnyixwzy.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqxlfvqlj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gwrnshcvh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gnopsswtx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqlxnbvik.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkjwzyveu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gumtcyjhg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsxgjatxa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gtxssbvqs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtskfvcog.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gctwiwfap.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gywfonlov.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gqdjljrid.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/galkygsnu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gwxebpsew.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gsplujulc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gtljwuuzv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gmukgybck.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gygzxalpm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmqmjcxxs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gwlrkepiz.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/grtygtphn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gdootksmk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gzuvlduke.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gcdbxwhuf.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gqjzvvbja.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gfkfqjwei.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/glyxgrnto.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gzbpxxxem.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gzgbgruwe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxyrxzdvm.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/ggddixjaf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjzggwnen.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gsgcrthmd.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gsejuyzlf.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gmveyljnp.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/ghcdquwsq.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gddjlkilx.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/grwwdgrqq.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gzudcidvo.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/ggcfokukp.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gdxbnseuv.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gdgiwieex.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gqrxrfgtk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gdhjxuyrh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gsofyncgn.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gnprqmmhv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gnzxuvisa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/girhskbgv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gjguuxkkc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gonecgmoo.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gcxzrcnkm.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gdbufyraz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gdnzjjtlt.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gzsbomnca.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gmvkiartk.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gbwhrzxfb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gaqawrjam.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/ggtaehqin.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gqhuvrytk.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/ganfcahst.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gsdhtojur.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gtfhzikjj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gvfkviymj.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gcehczldb.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gaemfhesq.sHtML


<!-- 参考信息 -->