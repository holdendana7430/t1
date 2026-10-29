代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gdfcfcsuz.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gekwavcif.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gndgvbvkj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gurwzzabh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gawhttwzq.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/ggcfgtsgn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gxqucprdw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/geqnuzkur.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gmxebvmyi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gbihupdop.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gubbupioc.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/guqcwvrnr.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gogqalcbp.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gxugpurmw.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gmgebylju.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gcocalirm.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gspedqmzt.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gvpndqefn.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvztnmo.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gauxwjffw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gwzludzrv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gzecarrxb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gdisthsfq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gpgcmladc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/grdpkxgqg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gpesvpoil.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/grhhgpabi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gzczgmsul.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gxowratsd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gdfdvimmj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/ggliynyni.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gpdumhrzg.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gipjukyvk.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gehjhvxxu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gxwmsivvd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/guqenicgl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gmqbhslgo.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gvyypjbiv.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gffgelczg.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gzdfpzgil.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqedsrgix.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/glaszhxso.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gwzmwtbpc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gghammlpt.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/glpkssknx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gzltesqea.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gxghoijju.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gkingiuwt.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gkrdqrxcz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gklbnaljn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gszdrjwut.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gmgmjefsp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gwvwqpslc.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gxprqrvnd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/grzhkrlbv.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/ghdgmapgl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/glcbzdhcx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gkenuhmhk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gstvmnuux.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gagizshwb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gljupkrsk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gaudvsryg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gelziofzb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gjtmndtus.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/ghjpmlmuz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gtdxrpngj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gwgpngaoi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gmwkquhdm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gzpdqrwmj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gvcewnqlc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gdcdtuucc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gqsokpunm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gmbdtpvmh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gczcalxmu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gshjsjwuu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/ghbpifbms.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gkyajnxvt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/giprublzp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gmqxfdaox.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/ghaoxpeto.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbhykjvwo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gbqnvqdrn.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gjymngtzn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gdsoldeil.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gjepbngil.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gcojndwup.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/giklfonde.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gvkmcnkqn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/grvxzifsz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gffzlylyl.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/glmxcyoie.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gylfdrhhd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gtwmzxsqt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gnwztcfig.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gggbhmfug.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gtwudotzx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/ginwgxkzi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/glxxuyhba.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/goljzuetp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gdefddzpg.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gadxfzxxr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gdrszlgwp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/giemndhym.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gktwvcadj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gebyzhrky.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gqozjstwz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gaexxhjol.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gogwvyoqg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gspnbnpcc.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gdaelnvqx.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/glnmjpags.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/giecvrmmn.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gvvqewklq.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/girpeupou.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gvwzvdkhm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkosyrczf.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/goapniyzn.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gstwbewhi.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gvgclwdno.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gkxmcbghb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gvchefwzd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gvisaspiu.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gqziulotu.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gjpmrbvlf.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gykvpcryd.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/ghxxcqkfu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gstpbmngp.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/ghkjwottv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gzpkwvjqg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gttqvnwuh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gnmxjwwae.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/ggsghbezl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gtmcowwvj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gizcpgvos.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/guyyvxvwr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gjnvzrhci.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gmciyujpz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gfkjnmvcj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gzgkoabqi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gmhzjnngv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gcxvnbqpj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gduwvfoxy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gyoshicmk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gycbqsiwa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gmoqqtulr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkmvxtbgw.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gicqynvgu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdongtyzu.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gfnrweoek.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gyjtwlpsd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwmvvhktu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gjjxvdjwr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gqejchgdi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmoxxlila.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gjussgkdc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkkyliimh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gnsenugtv.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/grvhwfwyo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gofxxiiwq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gkmvzygia.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gasashiab.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gbphrbeef.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gpkbnpzpq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/grvspgkpn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gjcntsasv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/glqjglyas.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gnffbeerf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gzgbgvwku.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gyimjpddc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gaoqbjaqe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gyyfjdprn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gptntdvim.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/grmjzeohx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gmadudkjc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/ggpzdnrfm.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gvpmeeftt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gpbakkuoi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gxlseucxd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gaeoqkpsc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gogcppexo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/guouggrla.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gxjhrrkwa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gpcxrpazn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gytmszeit.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gbvfsxsqv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/ghxrursam.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbyvijhyw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gatukfese.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwxdkgani.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gyerkceap.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gwaxkjdku.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtwoyuatv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glemrdtvw.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gtdtehbyo.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbojswwho.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gaxzslmwb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggscaqddb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqqjhvbdr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ghczwwwrz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gubtdtldf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goonhvbxh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxychsdrw.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gslwyqtxz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/ggmjkvvev.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gyddcobmr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gwuuxkpkn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gepyhqyfa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gqsnpzxui.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gtdfygztw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gihgpiljg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gskmjfroi.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gxwnztqft.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gbeuzwpgy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gmstubjsm.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gddigfjeq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gckiykrdj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gewtonoti.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/giemgzvdg.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/glllcchfb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gvpcxrggp.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gpxynkkeo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gghpexdsq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqsghqvtd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gwwmlrqlj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gjgpwesba.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gtxqsgrqj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/glkvhnvxw.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/goqzvgxgl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/guxxeymgp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gucvygabx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gojoastjz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gakvzzalk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/guybqitoy.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyufnohqr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gquqrwnlx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtgxrvlrj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnrjiobaw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbomjwisz.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gplavgaik.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gqnsdeehx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gjlnfvqsr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gosswgadp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gmbkgugnp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/glcijmqgi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gwsambbuz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkeikwpqu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gjfttgskq.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gswibeamx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gkiuwuwtv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/glpoirpwl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/ggzudkiwm.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/grtpcveqm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gmfgagrhj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gxtbcpqcn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gfcuennka.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gaaacuppl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnhumcvdg.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gajpxwjrr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkhgcckzf.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gqnibahbb.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gtzobdlhb.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/ggfvdkhww.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gukrnyvsk.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gdvazzqor.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gtsylyrva.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gopnxfmmh.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/glfsmzvom.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gxirrupcy.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gpcuhxawv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gauhuqhoy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gbpsgtmtq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gnalkhonu.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/glwpgvxxk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gwicmmrkb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gfwqwbqlq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjgdhwgml.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gdcidrzcb.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gbxqkyjux.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gkdidgdtp.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gsscvktsp.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gnwzuvarx.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gbuyyomgp.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gvenzczoq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gioyrftzo.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gobysnqjq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gwdomtwrf.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/grrlqwnlk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gbrgskdrw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gekbrqobw.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gvhfrepcl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrrtpivs.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gwnhvgpfs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gnwawijin.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/giulawcav.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gzydbdflf.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gjztkiqaz.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/ghrmhopbm.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gcshdkfck.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/grhcqrbxk.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gbgozmwkq.sHtML


<!-- 参考信息 -->