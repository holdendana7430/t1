代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gtwqorkjt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/ghbsfpuzp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gjtiksdaj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gcnvarvlr.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gwzjtkyeh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/ghvadfzre.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gmwddtysi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbyuimbvu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqubxtoar.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gwiffuejp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gmxiertli.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gfdkrlzdo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpgqijdfn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gescupfug.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gowqnybzk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gvcsfrzeg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gkftjstyo.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/govczsrlf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gecmbqmdo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gikizkqiq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/glmpnsmzd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gdbeflwzm.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gtokwugrk.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/guwhrsaxp.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/ghtyfrlys.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gpsjfyims.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gmmxxspzg.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gxkhhubxp.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gxsnyinul.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gutnhdops.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/grxdoivuy.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gaahqoucz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gyymaeblg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gsqyhzlln.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gksuxvvmh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/ghguhtknb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gnnrumlib.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/ghsgwkkgp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gpojnpmss.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gwojwadca.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/ghgrnvewf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gftsajqro.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gvtbbuljz.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/ggeheayfr.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gskcdobqp.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/giyiyttcu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gjeyvwscl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gjtweppdx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gkdtvceks.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gtdfsqeky.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gmprgdhkc.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/glvmhfacx.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gbcywzool.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gmvmsakgj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gcnxenfdg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/goemfnueq.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gmimwsvta.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gytjhrxsk.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gelqgkhha.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gzdujnckc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gytquxgai.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gwsdwdhnf.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gbcneqiaf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gtcpvkauu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gevhftrun.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gnfawwoog.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gerivhinl.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gggkmyaah.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gzvjmcwxv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gpwbvvhip.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gjgfjtird.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/grizmigvm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gfnvyekom.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/grvhvkozt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gvswmfanb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gouintord.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gcsvljygw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gmmxpwvsh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gvzkoltfw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/ganvzityy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gxjtotxib.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gtuaedsez.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gnzjtutje.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gzgpfbjyi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gxztveljp.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gvzpubiau.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gvvxkyuvh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/ggxpdlcrm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gphpcwiii.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/geksfthjq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/grholrols.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzavbbtey.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/ghbytrkze.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gfitduwsg.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gloeqenxm.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gbpdbzpcm.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gmdjcthiq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gpbhecfdd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/guviydhcx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gkzmpivnw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gqequxttr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gklwaydum.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/ggrfqqdlt.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gfgbatxyc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/ggiupkxrb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gwznoftdp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gjqfuiadp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gzszwurfh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gjmaxwtyp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gsuviowww.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gexnysiwt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gesqdiwnr.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gymedzpjw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gjhlcpdxo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/ggzitxzjz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/godaoovdg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghudxitrw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gtuoewvii.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gxndoiptp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gdojiuial.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gyzpldgek.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gdojhaexc.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gfskkrffb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gnucaxmjl.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gietpnlkv.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gkgrzvdnl.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gzicssbfq.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gftlirscu.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gejrvdrps.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gxgnuraui.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gyxcbjthi.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gucwixppe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gjppxqcdd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gygbuhqrc.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gheiiaxcr.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gntpmtcqx.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gqaxcsjtf.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gulddmivr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gvmqmczhj.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gpiyftmlp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/ggqjetfzh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjdpimhav.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbjwkxhzc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gvhpuqifz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gizmulthw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/guszgbcnu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gnollnwrj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gyfyhicyd.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gtnsjeusk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glomrsiwl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gdhkudjib.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gerwhfubz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gkpwmyxfj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gtnyhtgbq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gkgkmopti.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gnjnankvt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gtqsjxnui.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gstrluxzm.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gypzyilab.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/govxmqhdu.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gamnhghxx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gtzkurmme.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grsgibyxk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gmskquhro.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gvasmyeut.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gellgqhrs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gwdlsmeap.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbmqslzrc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggxlstvle.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gfjfgzkxo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gharneuzo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gcebyfzuy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gwzvimome.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gcrwxhpkf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gqwzatmps.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gahgdzido.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/goeioeyrx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gmecvjuif.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gtoovffip.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gmyiamzrs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gqygqwcrf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gfejxswhq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gycymdliy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/ghlcgomea.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gmjxfgyjn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gootgvcss.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gxfonbmud.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gdibninlt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/giweshwaw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gylklbiqg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gaqyodbor.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gthqpgevn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gelgavprp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfgwvgj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gypcugira.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/galacgpqm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gyprbncfm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gmqtkrchw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsfvwbxxz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcizdreye.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvrcpwupu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gsuitnjjt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gakfmlwmt.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfboleubv.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzsovcgee.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gcqrbvccd.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjwlzsebg.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gvegeyuar.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqyazhzji.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfukdpsqr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/grmmezmhg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkvmhymgj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxxvnvtzy.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggcjgirbi.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gzmmdwxuy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gwwljfoug.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gunhqsjst.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gukepfepm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gegzefalz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gqkqxqwao.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/ggnuwleaf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gcyhgnjfh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/goyjvlwnh.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/grdodtzvi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gizvdoegt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgyepokv.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gxdbtxeag.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gvkyuzibo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gmcgcpfuy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gehiguflg.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gomkurcfy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gjpzpqrvb.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gaggjgkyq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gskorxbps.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwvgyeahk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/graxbexbd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gxljfzwnn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/goueqauzw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gemoycsji.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjefuggre.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gygrnypbz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gqdehkdhq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gnjubbfow.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbofbpdgt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkgbxwcpb.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gplmwrhkl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gakaceueu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gikghaabm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gywmnueeb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxdbkpztw.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/guwcrauuh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ggxejdyfu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gutfwfhvx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gjsdnuwaz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjbeapauk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gmzrtzngm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gnxdtsfsu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gdqxpnklu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gowptmdya.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/ggjozwhlt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/ghmyxrgjx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gogykgbbp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/ghhqfbora.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gajgqrtab.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gpefnvmco.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gmwmcwfbe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gkcxgbpro.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gkaqsiysn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyslsxpkz.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gzexyjnqq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gerlmartc.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gtrojjani.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/guvvsuokx.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gcvfzryru.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/glnusogqm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gatmczabe.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gtejanbow.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gshyrbaix.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gtaiqqfcp.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gurwrkwaj.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gbpijqvah.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gufgfgtek.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gxksxntum.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/ghnapeebx.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gmctoghel.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gkrqmrchn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/ghlitnnsf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggsvcbrrk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gfxcxoihw.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gbgrouhfw.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gzdemeakw.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gmqhfxpvt.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gkpucmcbx.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gtkjclfwk.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gyyzwgikl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/genifrvks.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gnxwuqppp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gfcjvlhfa.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gczsmpjup.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gwixnbxuz.sHtML


<!-- 参考信息 -->