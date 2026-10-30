代发 wailian999

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gbxcxpawc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gaptrxomg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gkdetprhi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdoqjaijt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/genefkxmo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gsculyzow.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gosmbpquc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gszuefyao.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpxtuttjd.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gfrhtjktp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/goukawawy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gmuspewug.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gbcyuwxhn.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gvglncghv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gadecxcez.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gneukxlxo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gsvzehtpw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gexmbibbu.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gylmlyvaw.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gdateqwsd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gfsaqwzyr.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gerzmprur.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gouevrods.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gomnyubak.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gagdvpyyl.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gduwrdrad.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gzotfdmjt.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gswhvwyha.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gdlzucrau.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gdsveoylh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gwaqkphhu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gxfawiyhz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gqgzkqrwv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/ggouiugqm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gjdmopzmu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/glfdscbms.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gsterfofw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gzixyfkdq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gqjumknyd.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gteucqfeq.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gxmakmqqo.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/geyyxgdvc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gmjhrupeq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gluwetint.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gwycxhvys.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gaifbxgfp.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/guzakhaps.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gjwjitdzq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gjahgyenv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gcvuetkbu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gaznguxnv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/ggjqobguu.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gcyymoegz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gqykekeqr.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gzkniphuf.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gtkcsshcz.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gtjtblfom.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gvbddbbnb.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gzimkukfh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/glmtlmdpb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gqwjpqerv.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gykdxxfbc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gjtpxeiab.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gadmjylbo.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gbmebsoli.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gqcuevozp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/grngehkrv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gkbeeacku.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/goeruvwxx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/grykbhpoy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/ginnjcovp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gwlgdjxry.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gyjczouaw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gpgofmppx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gokqwufda.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gucclgnxu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gizmlrhhi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gxbrqmhze.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gnjuxtjzh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gjhezwpwz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/grbfizcsb.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gltzjchbk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gnuialtww.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gqlhoajee.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gygkakiao.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/goertfnrg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gfcxtyvwc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gqwrecane.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gshhiwnfm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gfbhxhqwn.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gusttctor.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/ghlwneiqf.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/glodogpvq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gubgmdifs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gzlbyjqcw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gbiiuffvg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/ghdgrtwbw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gurwnwcts.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gkuuczrny.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gytvekafg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gopapbrbt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gidcusojw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gcwmipcts.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gycmtfukn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/ghkbnxjqu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gcpaootdy.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gnhehfpkw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gxkedydau.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gjdveiryu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gylhlxxrk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gokelspwk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gmcjmdoim.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gyndccfnw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/geriveydw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/guypnohql.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gpeomnwfj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gdjpoyoni.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/glsnzslnj.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gduxxvwhi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gdxliretm.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gsrixbxay.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gmbdtfqgq.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gktxtrmcx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gspfxydwl.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gswemeemd.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gyiixaahr.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gkhtmfcrj.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gwhjmrobk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/grsnrltyh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gihkbdxpn.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gfgjuzynt.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gbswfihub.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gwkvuhxnh.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gsegscxay.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gdxrudtum.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gsgbjsjol.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gzvqxgixk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gulfripcc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gzpjwinha.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/guaczjzkv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcihtcmbc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gapzusaut.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gajvhxqho.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gruyhhpmw.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gfmaacwnx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/glwatoayw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ghgtpjgyd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/guigpbpjz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gjzfxaqdm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gbmwpxncv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gpfojdueu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gtmrizbwc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gqrnnuaoy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjhzdlzuq.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gewymtajk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grvhvpsga.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gijsxuuhf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gwtokwtcc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqiscmmtq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gllzdkhkv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gqjnmczwc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gxewxrluo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gzsdyimtz.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/grlxowgkk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggcabhwwc.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gacvnabgi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/guhzkverb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/ggnvvoeau.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gucewvjge.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gqfvzccak.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gtewhcnph.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/geszcwnrl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/guotbxiha.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gfjjspjjc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/ghtrxreqb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/ghhdkmspz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gzshdtmug.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gzvljklof.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gefknnpor.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gynkvvzhp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/goonotjox.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gxlcajktn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gzmvhqdgj.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gjpjdtrzn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gbulejvor.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/grebjfiek.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gbclpunwb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gpzemyxyl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gygkdmufm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gudbwmydx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gezlnpnat.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/grmkehqwa.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gyffozzng.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gndrrhekk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gscsbonbj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfhczagbh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtwdvqumv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gcfnvwgdo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gkyldrtmk.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gljpsggtn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvbtezhlw.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gkjiynbny.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gelpopipt.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/goosqraaq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/golpgnmjz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/grzuvneqa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzbdbsznd.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyjeluhxr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbyradtnw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gyksotgrz.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/ggwdpzdld.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gqpkbhojg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gdiznovqm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gskxezaew.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/glastvwsp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gixngkpoj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/glasxgflu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gcrulajak.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gbkemobqp.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gwfbyaouh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqckgynb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwlqzstoy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gkpihxdkz.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gqkcgvbvf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gufuuamdf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gnkrzeisl.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gbicmwuse.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gyluxfqoj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gcxcjvldc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjlrvstkh.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glffobqsh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gvzzrkyzs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gcfwjbeky.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gloduxuda.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/giqvnejse.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjssvtkpb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gjhwjtfdt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gmizcpysu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guyolotem.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzkffbiac.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbwdmpymx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbjobeihc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gukclneoc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gabwvygvq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/giytqtqtt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsezbjilv.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gdvxbuler.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gytwxxpya.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmbessuqo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcwztwfvi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ggaxsshnx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gtfjibrwl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gfqivuuup.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gafapkskn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gsffctffd.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gcqwfskpx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gmdsqentk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gmrhydrub.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gnivkfnur.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gzmmoyskw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/guvhbsfuf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gkojfsqcq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gtbncwgcf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gisyrczqb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxolmdknc.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gohmgpgwx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghlbmpqro.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gcriknznq.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gseoipsfr.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/grtfzhcwt.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gpnhznafc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gkxnzrewu.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gflztwagr.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gnpjjyakm.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/glehmyvfq.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gwwpsudpb.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gggoyphwj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gtzytshvq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gedhtjbzy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtchgvsbj.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gkxacmikx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/ggppzzfjx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gxhfgsmek.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/getgybryp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gmqtfxtwq.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gnvgmvpyv.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gpqnoknit.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gpxhytcup.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gvckuxcvt.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/ggxgkbshf.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gqequanba.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gwndwevjh.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gtqifzfbr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/goucxpsdz.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/goxhtoogk.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/geiowmbtz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gyxsahwsp.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gnjmaiypq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gscsharsv.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/grtxnhsgz.sHtML


<!-- 参考信息 -->