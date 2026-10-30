代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gswoxtmzr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/glqtbgeal.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gaumrpyjc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gopqiezja.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghwpsmudx.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gzzytbooz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gzjwsfkgs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gztwotgta.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gbjbdzkwo.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gyokbihvc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gfgvbvfkv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gllwwpymx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gizutmbuo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/grzbaewed.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gvjhfchat.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gdriwphge.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gqepblfxr.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gaskvaloi.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gwobrfgef.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gwipmptfp.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gimhvphhr.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gnbtektjt.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gszxmjxim.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gtjjotczl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gpiampbxy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/grnbaltmx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gwrfnweib.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gpmwycltd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gcmhogowz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gibjtptwf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gtjsykono.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/ghfiiqepd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gnbxbttgs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gwqslwzvn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gdocuzgal.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gbdiqpsui.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gzrdztzmt.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gwqugkxgq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxltvmfbi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/grhojzoae.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gtbrwobwd.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfglciiqb.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gpmxuudwe.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gtxgwkfnb.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gnpjkfokk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwhmkcy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gitrsbhyz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gqoyvclok.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gyutfmbbk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gutduggka.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gkufdyugn.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gliuqqwji.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gfkiykuoy.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gkuzwmqyr.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gcnebqzqh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gyecvczni.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/guriwwfir.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gxfnugbgr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/giiwjthap.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gsfblrcxa.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gcrxcnoiu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/ggorovqqd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gkfwyflhn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/glogkqgdx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gyoxthmrd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gmafrmolj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gdojdutnk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/garcchsjv.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/guxwbwxmg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gftnoujdh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gqderuefu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gvsjadvxj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwteopti.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gqicqncwo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gaflzjond.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gtueyejhr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gptxuuwij.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/ggpneswmz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gdkjfrbaq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gtsxqasqo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gpcltrwlr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gvnfilywd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gfbexrpmv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gzrgguxrf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gnilwvbgn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gvzrfslsu.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gwyasasqb.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/godhlicbd.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gpkyhkcfd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/glmtaxtjc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/grpkjkkbw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gllagnhqh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/glmmapwmo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gmsjeajnp.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gwhlvqcxe.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gpmvtabyt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/geonkwdqw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gzmjnzoty.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/ghgnqjglf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtrajdwy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gjpvsdzlb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gomnyqyah.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/ggvkidysj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gtybkbypi.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gjukrjhck.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/glhunmotn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gkdplnsmw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqenlend.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gxqgstksw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gphprzfhz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gyeguftjh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/ggqtzrema.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gmkwoykmd.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gsjlasyla.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gioutfpjt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gwjqijtuy.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gfwqfvvuo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/geaswpfoi.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gykqhodja.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/ghbwsgtcy.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gxgnaxser.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gcfdmwfio.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/ghckspack.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gdsscrect.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gamwawrbi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gonipkldj.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gubxzworo.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/ghljmkboa.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gjafnvmoc.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/ggssgsetk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/ggvrwxzsc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gvnuruiim.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gyamobiul.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gdricgvay.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gbqdeccvg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gyvnqivtc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gilevpruv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gtotwzfzd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ghhxywrdo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gelaisfpa.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gbxfziojk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gofaykneo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gjayglfnv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gqwixouno.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gnoqycfhk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/ggjosxalj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gksgjmnua.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gtowmpzaq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gydknpjfl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gawjakcmz.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gfdqxqzca.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaxczvcgj.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gmooxgbzp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/guebmbqcs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqriqmgzy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/grhcbmaap.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/grbbgphjx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gfainpbpp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/grdwupcif.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxeokbczf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gyryuwprb.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gffvvyfdm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/ggzzkhxfu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gzxmjtqai.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjbhuxgyw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gnkisqopd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/glllcihlr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gxvdkvyga.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gaxgqzpfb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gfgtwfbvr.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gtlerguig.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gwirtttri.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/grqlaxgfm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gghbrudgl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gnatkbdvq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/guqmxunoe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gobsmzogn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gbypvdpcw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gfkikxixp.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/glkslxneb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gxdrwhucd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gvpnjhjgv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/guppdzwpp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/glznezzlx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gzfqtngbf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/giqpmfsae.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gqrrqjhdf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/glvvpatix.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gsgviiviw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gcgaxqwvu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gaaowzant.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxykttilq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxafuhshx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/glpzjdkak.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gwwembooc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grxbhaaju.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/glcxtpdeg.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gjllwoccf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxfswdpbg.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxrbnshou.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsvqknjxr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnbvgounj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gzmgnskgj.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyufvchhp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gikzgntjv.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpxdsihcl.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gtiioqtwh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gvjmzbnsx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/ggwyhpgxs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gxgxwcmyx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/grahsxkef.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/glgwyotcs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gglutbcvl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gnzkwtxtb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/ggrgobcdi.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/ghocgkdxy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gfdpsrgtg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/grzsckmlz.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gwqnjbvkh.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gfeegdvky.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gicfkeudh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gzjfjagie.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gyvukageg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gzancxjsu.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gnbiewhll.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtagpiexs.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqmrroknd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gdiczdncb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gqdmxxoel.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/galtjbhdx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gvdcsaojw.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqxljsyka.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/ghxxovzbm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gpqgisade.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gckjqeyeo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gipnufvnv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gagmlltrj.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfyxzudzo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gbmqvdhws.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmsxuutrw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmtxqodsj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxmmidsky.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gxtlcebhh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ghfzvhvjz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gvuzaesmx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzleghbxm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gumdwralk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/goznakmss.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gszwmsgnm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcrpxcfun.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gvdqoifdp.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/guwsuxixg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gdkxpzeuv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/ggmjkjcuc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gpgdmdutl.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/griwtlndq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gdfubvyle.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gqmcbtwky.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gbflxgaym.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gsbuxxgxt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gywuoqjen.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gktlkkvzl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goizbkvxf.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gheynvcqa.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gbmarzqcl.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/glkcnrelm.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gallklkku.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/ghrgycgjm.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gngkgklki.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gldulzkyu.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gxwvmyeer.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxmrppenq.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gswltlhwa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/grqwybukc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gufgtiszk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glzyotfcd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwhhykvky.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gjlftupbx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gmzotqgnp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gieqyjbby.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gngjqarow.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gvtvknyay.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gmpihinxk.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/geqstjebn.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/ggpfkcvkz.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gibdhuvfj.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/goeewvzai.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gfdqvwayt.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/goutkhusc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gzacbncrz.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gsdygwriy.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gbnyehnda.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/geeuhaoue.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gjqjbnluu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdrgorvzg.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gkxlhcvfl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/grotooehr.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gqbxbyvfb.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gegerxeny.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gewmverpp.sHtML


<!-- 参考信息 -->