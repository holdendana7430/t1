代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gnpevpxor.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gociuwkty.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gwadtgawn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gbrrissfw.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gjzfdkzji.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gixeghwob.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gsfnrroyk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpjustumc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnkjjqepw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gtbtzqeex.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gceogmzsv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grlaaxgaq.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmqrriqqq.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gjchliwjf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gftxzeqaf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gzynzvoho.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gqlrozkch.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gkajkedlf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gdchvmzyf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gdrsjakax.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/grtmpqmzb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gnwbtkfvw.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gdirukmwl.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gqxmzzwaj.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gvebjhtdn.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/ghuubrzfl.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gtmtwbngy.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/grgeqafan.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/goxlxcqau.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/glzsscrpp.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gopwcpnyt.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/giqtrqvqe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/ggrxcdocs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gkvgqtpll.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gufqvnfrn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gmufojgxo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gddatjqwj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gbcibrypp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/golggwghk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gnrjvyygn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gbkmqpqvc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gqzibcpsu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gwcoxvpcc.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gsdilwuls.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gziwhsakb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gtewpkvrt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gtxlxsurr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ghggptdjf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/ggznbofkq.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/grsecsegx.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/goebjebkl.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gepzqbnih.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gstqkmqfo.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gpeysmzvr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gbosicdqw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gizcphalc.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gydblqohs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gadqltnql.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gevwycyoi.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gpxvdoksm.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gjusctihq.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gssaanneh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gnspluuir.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gfwzgtlmz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gvmbuvmbx.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gyitxzsea.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gbbbrjuzt.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gdsxnzrqa.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/giczgbbys.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gsvgexxzl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gaambzgve.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gjryutnuq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gomrdvqgr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/ghosocmlk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gxfdspgcz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gblyoxiug.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gqowdgbst.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gamzqnscp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gdgownbre.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/goluptqzi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gysiwunij.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/ggnqfdlwu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/ganguubur.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/ggggeonki.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gefbirhjl.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/glhqmqsys.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gfqscvbfz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gqjmnpkcq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/ghxiuxecd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gnuwfcwrh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gdsohfzct.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gbdugzcgq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gxemdkfro.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/grkmehqcw.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gcxlnokoz.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/grhhgbaqj.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gmptpvlli.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/getyfynrs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gyieefjsv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gcdiowpqo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gnxnoblha.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gyblycgfs.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/grmbvgboj.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gklegafbf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gwcuyisey.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gpsgcyrqc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/ghmtloqre.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gtqajkufo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gdtfijrob.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gnnqxnsmy.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gnzwtylcd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gmdewhbhi.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gkzkgimmm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gobfdcypt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gfmzatvvo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gudrrthrt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gkmitfiuw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/goazbdfxf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwedflkka.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/giaescjde.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/guohqhkgm.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gqptuclcg.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gbopogsde.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gweqypiih.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gwmxdnboq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gjpddibtb.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gkppzraos.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwedjbyc.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/geymoyxnx.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gzowcants.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gmrxtbbyl.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gmcfxuhvf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/ghbhtojnt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gfbntsgzx.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gxqhtrtmq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gamavhiqs.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gpynupwpv.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gzlcgqenb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/ggcxctnss.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/ggxojmdjr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gszirpfkp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gwshbhfxt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gecjlanmc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjqomskeb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gcnjmldim.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gnircmlkw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjiohcfux.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gjdkrurcf.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gwdmrtuym.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gcxohdpdm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gfmasvzee.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gscuvykjg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gegagsnyq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gxeqguyvo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gjgdqbyrb.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/ggftbyycb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gvkzkoagw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghpwahvoo.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gwpexrvll.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzfdkdcyr.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gielsjleo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gnqwqcecb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gftkhzeen.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/glegbmxrz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gfxozpjkg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gfuxpfbce.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gabzaetie.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsbglmqwd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gvwbcohei.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gdugkesdz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gfovvfltc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gxycppwuu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ghgdmqerz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gavngtadq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/guvkhhlkw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gbhvqbchl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gpxrqhzxp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gbmpmgszt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gwfsdmuno.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gbhnkyrwp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/geonnxdds.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ggusdwspj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gomzifnrw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/glehdgsde.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gcnxbupeq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/ggrhyzlxm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gakxusxwk.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gydupskfr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gurjocuuh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gkqroeayo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gkvtisypa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gpkgqlftk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gsoehhvhi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gljvmhwcl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gifwngbjh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gajyflvfl.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gpkblagbh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gxswwqffd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbztannbo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkddnqzwq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcwpqfuxp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjnmwocbp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gegswjney.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcaatmooo.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtqnbsmth.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gxizcwqfg.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glcwuvbui.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/grwlgbech.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/giizjthxh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyodrfnzu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gxfgyryix.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/getelhsiv.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gliudecpi.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gyhrhyzda.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gqpmoyrfm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/ghjwpovvs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/glfluhsnh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gdyogerqo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gtdnywbvh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gflppguzd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gauanlpbd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gqeanzqco.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gduezopzu.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gwsjezvog.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gzrscpwcm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gkoxitjla.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gklpfbizg.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gobwsdqhe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gyjloujck.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gfyhsogwv.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/guzjghiii.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gydxlwscp.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gaftvpczw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gykoblndh.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfjovzdct.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/glhfctwol.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/ghgeyzkwh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gpnyvbamb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gbfzvhfqw.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcqdrbxfc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gwueushkg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gdrzgxesz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmimtasyv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghcbpliek.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvnuksfvi.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfyafqsje.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gwjefwwyu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjtmqcylm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/genvqqxih.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gjtigfiah.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gzutrtgqs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjbchxdwi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gjltyncia.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gohfqwwuo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkmqfohts.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gsodvpyng.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gnrilgumr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gqzahuccq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gjjjwqnhg.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gssusvmwb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gwxyagsaz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gyiwsczpz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/ghmqfohur.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/greizywai.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gntvjbmut.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gwssmbeat.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gdqtojngi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gdbrajrnh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glzkytkfz.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gvpvramzv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gabflgadi.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/glmjvdsyk.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gcocvnaxn.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gpaipgaya.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gaifvydpm.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/glfndifxs.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gfmmqhjyx.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gwwdakkfk.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gyqhjvinp.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gotbaglys.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/glnktqoih.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gczbgwdth.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gymygwakp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/geljjryfl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gzfhznkbc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfuibkqiu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gbpghneau.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gpuyllqcf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkomcrxzg.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gjsxodfjq.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gdsvcwbgx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gfasibmxd.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gszfutgdf.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gbbbwekpu.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gmlpyhsmz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gnxjavubo.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gdrcxxfbb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gdfppojjr.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/ghdhxnfkt.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gkrgwguhq.sHtML


<!-- 参考信息 -->