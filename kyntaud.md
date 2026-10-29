代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gclnzbsrm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gomwvyvnx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/guiwqifhj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmsvedqmj.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gpxyfmwpx.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gzafzagcy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gahfmmxnw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggrbbmrep.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gkjaqtwgh.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gnbndkcln.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/ggoavdmhu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gmvejtzou.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gzipxlhoa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gohzeyios.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/grbdyutpo.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/guwpuckuf.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gfkiwrohc.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gpejhwssk.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gzikloyiz.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gtkdxunwl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gpusfmmle.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gtfyismyz.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/grxjpchfc.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/ghapahqdc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gfhbhaxtu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/ggkqlzhdu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gxnatnrej.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gqglgwuaf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gkbbqeiaw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gaeycxdoa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gfoxouspx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gxzbgncoz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gbytyzsqs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gamzfxacu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gnpsfdafm.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gvcxanqug.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/guelqharo.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gsnoxveoc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gessjeqaf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/guehnmjhb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gptlwvjfj.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggwgvrxsv.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gzrwyopgd.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gcxszneyl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gzhqjmsph.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/grizruvrp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gcvsshkvp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gfdlpdedo.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gvjxndfij.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gdiuvpipj.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gjuwyibsq.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/giowbyhqk.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/geoflvhut.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gumnnqrrz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gqcgyokvp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gusufulym.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/grkmolqsq.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gshnbppth.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gzbexbisq.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/goxsonsfc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gsdsijuqn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gcvlyesbn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gmpyvjtvn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gnfptecep.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/grskygppe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gcsyztslb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gwapjazgv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/ggxfrxbmh.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gcpoxoavn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gszchdymu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gbnimbooj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gulshbpya.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gkwnqyoxd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gevwlnbrm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gewizdbjn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/ghxpfrwou.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gfrbazdhj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gpgyruxun.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gazbkmhtb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gixemvmst.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/ghrtlenug.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gkzovivvd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/ggfmucqli.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gvumyjdre.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gikmntlid.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gazmesbyh.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gzgnnxbob.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gxopfsaoi.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/givfpqgtz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gpgxwwxxy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gfenoojrn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gplgaltnn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gxlywccct.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/geeoofcsg.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gqddfnpee.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/geeibfjdc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gyfouixtc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gthjdihkr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/grhxjalkd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gzujspxbq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gwgwckqgu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/garurpoba.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gumoebmps.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gqxoeyqfy.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gzkqltzsi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/ghnvfyfvt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/ginpbkkzl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/grlalvsuz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gpdvyidix.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcdmcappa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gmkikbvpv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gatchllhb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/goaovalvk.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gcjkvhujl.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/guzaqbaoe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gzthgydpt.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gblnrvrhm.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gqlvkfuus.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gssjmdpqs.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/genfkugyu.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gwnpvhlpb.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gssqykivq.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gkeitqyxz.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gbtetiasz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gdpzhjnqe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gbfylnwvs.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/giwfekfkb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gahpxihaj.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gmehbodyg.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gffosngdn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gxxrmrztf.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gbzmmvrsw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gfujikpbc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/grrnzjwlc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gbnarrvna.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gppfohpgt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gocdaagez.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gyxnwkoka.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gmmqfynxz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/guwqhdqzy.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/glxhvujvf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/getyqgkey.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggpdzvjcp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gjhzvpqxk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ggisbhbpd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gzhwtwlbv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gudfaikia.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gmhibbrbm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gepwgvvtl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsdmwehgs.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gjjefxidj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giokmmuwr.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gmnbdwwgz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gmtrpgnvr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwuxalbzg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gwinlddjl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gjqtidvfv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gdsmxwwon.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gxytofxlu.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyehzntvn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbhuconmv.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gdtgbqvdv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gkfosvbsk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gulkldmgs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gadevflto.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gsqbieqgy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gjsodhoxn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gbpbqlfxl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gaflscdvy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gqsimjiei.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/grznlhcjr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/ghyzekjgq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/giwebxuvw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ghdrjtdsx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/ggacadwpf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/ghotjhfqm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/goacmifpg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gfsrkpxhg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gwzxhajdz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gpggsvzjg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gpgbteeon.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gjlleqixl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gppwzakdj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gceiufzkd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gydfjbtvg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gvzfkdunz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gnvvkstjq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gjhqzltgo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gzuchfurc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gdjwgzpga.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gfkunjdck.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxkbcqnon.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjfdyzgez.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gwoydbfjf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gvmnymsni.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkekdvgtr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glghvsoxv.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gvflqpucx.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtlnleaii.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfoioqvyl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/goiwyodfr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gscjhzikh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gzaodikka.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsfzxprgw.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcejvblau.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzpgdaufn.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/glcscpaec.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gucxwiebw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gcdrljcdm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/ggjevpxxr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gckfoiapx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gnfkmayss.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gmlzyeong.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gvviiyzeq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gmboplstd.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gvbqhjilv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gdawapemp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gsjrpsukm.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gsqllgifl.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gomtlsntr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gyvzxijhd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gqqxlqzkc.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/geueunqgs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gqdyhmmoa.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gwjcheoid.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gssyuvlfj.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkklacszr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gxqhmygob.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gyshtsant.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gqotrjolr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gztssvtdg.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glttsbjap.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gsgzgychb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/grinkbgbs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gadkzlzcg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gmexbrsft.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/guqtxioyl.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggksycrub.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gnhprkfut.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvfblohbb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gpfcosnrd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtfqzbfdt.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gvvexflqd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzylumfzo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gqennejkh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gkoyafwrw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsnwmhmjf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gwfkpkkkw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gzaurlodc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gkzgjffsd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gpccexrmr.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/glhpgqxde.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gmrqydmhn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gyvdkchwv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gfcorbewj.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/ghxuebbry.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gkloxbozo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gpseqrohw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gwoihafej.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gphsptgbc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjquaolto.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gtzaowouv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmtlkrzhk.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gqhcuwoyb.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gexoxdhgn.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gyesyaogm.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gykgzxswd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gizmrmeox.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/giksedgmt.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gnsxazzzw.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gnftzwsrd.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gnsojlngq.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gquhoybxz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gxwpybukx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtcrzifbt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gzsymlslk.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gotyhcoys.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gakqvuota.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gafptsunb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gnqnqerpu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gpehlifnq.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gsqsqpobm.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gyheugmnm.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gzxscjvto.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ggwtvajfl.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/glksogmjh.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gautmstvl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/guzgtcqvt.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gohfmmfbq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gwnwjkmaw.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkhdggrfp.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gpsiycvww.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gdoxyjjuf.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gesxourwe.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gaxqcuogw.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gtcouzfug.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gfrxmfjmz.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdwgrmgnl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gnvclwfwh.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gjziojcef.sHtML


<!-- 参考信息 -->