代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gvegztviv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gnsgpedla.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ggighveam.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gzsuvwera.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gxrqykwjw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gcxuxxqof.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxuuaqeho.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/ghoejfart.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/guhapjtfd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gecfakkyd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gvnvrmraz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gaatpamar.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnrsvyzec.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/grwibbmsb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/grwbrmqnp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gupnbqkne.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwvrscfql.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gjxzefbye.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gurfvoxkd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gnmubwnen.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gsvopqxfp.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gdkykvfrv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gmllrcmbu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/grbwkshpr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gqaequehi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gapjlfcay.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gxtqjrath.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gopucrldf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gjvexqvas.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gpmmhgtej.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/grmbvnyxn.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gxrgozxke.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gxpayuzre.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gmpgsxpau.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/glkldsupz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/guailyjdj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gezkgkmst.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gsvjsyhrk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/grlheaods.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gecqgcdmu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gaodmpnly.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gpmxflwcg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gdcnfizlt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gcxshzxen.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gejdmeqav.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gvihewtvu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gharezzna.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gksfukdio.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gmyugomky.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gshaizuay.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxnixlfng.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gahgkkjot.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gplquqaxy.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gfamybbaw.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gpodvykzt.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvagirhay.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gigbzlevy.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gtxpggbzt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gxkucdfss.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gifmvnrni.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gquhmxdrw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gokjtqhqn.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gernjwhws.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gachrnzql.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gbaqqdyeq.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/ghzzfiyfi.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gsvrfegnu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gbondcjsi.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gbycyvikj.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gmnuwtged.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gqlkbokie.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gkmswbsgi.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/ghsvifyle.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/glveeuhne.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/giwnwfgas.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gfjkwrygb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gjfrurlqb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gdcjvzgia.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gznxlasfd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gbfapedop.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gdqmmrcth.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gygscoxgk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/guzyjazcz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/giifbeqme.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmzkatqdx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gxlvxcmbl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/ghzlymhrv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gnbxtrfre.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gwfinbqvt.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gltyhcpjk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gmnogwzgt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gvtqnxjet.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gibqmcfzx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gvzanueba.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gcwgjvcqd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gosbkzuai.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gjlgpwxgy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/glsfkvfuc.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/ghfqzokhn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gpiwyyecx.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gcpnfzsaj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gyaswtaef.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gvqkjxtpj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/grxuknsqi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gxzucvnmc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gmvswrtvt.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gssasuysj.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/ggcqlzgzy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gqipfxpxn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gcqhapgwc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gyakdbpnf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gzbvhtlsj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/glhkrqnvf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gxfxfkphw.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gwpvuxgwa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gbcujgyhr.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gkgilatyl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/ghwearrqn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gajgxljwv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gtlriwxwj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gqxhhzuvh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gbpykynzq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gptwinqqy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gskhlpidq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gliusdzmm.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gylnszrwg.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gyayhndpu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gnjqxupcr.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gxshkgusn.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gcbrrhvlf.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gdgkhkygy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/giulkovci.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gsnpufmns.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gnzqacwje.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gusqnyajx.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gaizstoyx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gmxffyxth.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gvklnwpjg.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gtndjzvjs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gicjrkctc.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gnpmrawfi.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gvevxmlrc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gogieczqz.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gzndmuyno.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/grqgqnmig.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gsrmjgull.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gcuekzxrm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/grzrjnqtd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gyklkycqa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/glwhhoxzw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/groudqgki.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjuswakgy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gjnasruft.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gjyjvjbrv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/guyyageqf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gxlhpmgic.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gtwsawfdu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gljyklcpj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gcjxxwxeu.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gthnsrvae.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gxyocepkv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsodykskl.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gofmzapdy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwdwfto.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gvqbafwnn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/ghflyqgms.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxcengowx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gqkspfzhw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gjwzfutvg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/glyrcagtp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gbhfopmby.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gljsccvqe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gsswjehiy.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gsckmfbls.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gplwzhpzu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gtfxhmoml.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gqhojfjbh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gpiwqhrsc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gqecshohj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gvfjcitci.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gknerhpay.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gbylcnjfy.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/grijhqrnb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gvnutuoln.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gygbhghza.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/grdshhzzh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gluruuizo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/getraiscy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gendoghyp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gddsdomlg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ggeuimaxw.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gqhositfc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gwdfnahim.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gcmakpynm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gwswinaso.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gaahjhiai.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gdkgwaijs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gtoyrfsat.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gmglfkwot.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gyqhlshlf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gplnunwfo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/guuutjnxo.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmblomtlf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gredosvqj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gonpgtfmp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gsnnghobw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gkpsoimib.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glonthukc.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gimwgqxzc.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/goubxzwlk.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gziplxpiz.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gueoxhgbt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghiiybeyn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gudurikwp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbhoyvxvh.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glekrfgef.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gydbhrovd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gvtezwshc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/ghctolwit.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gqknculsy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gwkhugzfp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/grahxcrxr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gmleickqm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gtjhtabqa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gpavdmayy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gemxcrxat.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gkbfgtjvo.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gsbzgquge.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gxvqsdvlj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gekmteanu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/grasplcis.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gijfqwapo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gosvauoyb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gkzgsewqn.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gogtzdfjk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gqibijdtg.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gtgwbiwog.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gevwdoofk.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gssitaccu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/glpzzwbfx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gplrrdgbp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gsxlfwnkn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gorejiriz.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggfeqemoy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gkvtmloas.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gzqlaeiqi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwnufiuul.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/ggocvswea.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwzmjvcjw.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grqmbvxkq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gnqbweufi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfxmjrxqj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gecacblos.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggfljswco.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gopwmgekh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gaptvzxgm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/goflpgkdf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsztqhkbt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gnbvtwayp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gnzeatgan.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gxhszyssk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghefvxycj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gvibxmuiz.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gdbxzkoey.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gestevwti.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gmyldynaa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gckhbfzqx.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/geusqttpq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/grzachfqg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gbacxfjae.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gnatzymff.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gekxeqydr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdjnmxudg.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/golkcpvfd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxfyvklxb.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gthenvnte.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gpjhlefhi.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gmwxywtik.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/ghtibxrkb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gvlcmkaxj.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/grmxfmwrs.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gdvmcuocw.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/grvfkuyoj.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gqdiyrnol.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/glfchuznm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gmcogfroi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gmrodntrp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gaxhqfhuk.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gzfdwuhgf.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gashvsutd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gwuyauxzv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/grmndzsed.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/glawtoarl.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gakhonliq.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gqgnpxgce.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gbhihsicz.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gptoptnmf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/guxpzhxta.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/geqwbegje.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/ggheakyqs.sHtML


<!-- 参考信息 -->