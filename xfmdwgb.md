代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gtshhkvhp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gstdkwvsy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gnsiyzguy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/ggmnbssmv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gxxkslisr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gqykopzty.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/ghaxxugtb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gadgwhozi.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/ganvelfer.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/groowzowt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gcxngzycj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gevoclcix.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwuwyzjcj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdohxxtzz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gpaqgbckj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gnnpqyeaz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gzvkigkst.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/ghqndhdcv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gnhtfjgny.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gbbdrwslb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/glaphslpd.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/giixcencz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gcspwfxph.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gwwdqmruh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gwyvteors.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gzqofoqjq.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gjipbfqrc.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gvglfaygv.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gxsarqoth.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gtxdhgsqc.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ggdnybzjw.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gypcnxkzh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/ggqbrpmka.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gfvjfjdbn.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/grfmjgmzy.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gzovxdvlx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gpobwfvtz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gpncxtvoh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gxosqoncf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gmzsuullk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gmiszcgpk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/ggikztuhc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gcgxbzqei.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gkedasurk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gmizpqhpo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gchqerohb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gdvspguaa.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gjalzvgpx.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gvjgptqgh.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/glnubypun.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gtxnupwvx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gvyswzvcz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gopecavoc.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/ghiqacerh.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gxnmpnlnp.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gavngidgh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ggpwnqoqf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/glbseslwq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/galdrkgun.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/ghczpwhmw.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/guqyubart.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gnqttvhjy.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gwaenndxf.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gzfvlzzff.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gdmltpngi.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gkypyvefh.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gmhulehut.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gcuyioyvc.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gmzsfuczq.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gigxigeir.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gugzbpzle.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gnglysrjz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/grslajwhd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gmmdmevnj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gmxyhybfl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gpztjqtoi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/glbzuxroj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glfehwhua.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gcmuaejlp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzshgcdaz.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gcwwykaoy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gvxnnopfy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gtvnnzfjv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gpsgdcwxy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/guoteupth.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gnpczxrpn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gltvgqnlv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gwmpytvpk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gbcovanqf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gbobvjcyr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gtsqatazn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/giredflim.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gisvptfsf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gofmhjdrz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gwmiwwoju.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gppawzsmx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/grxdcsgmb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gxlczmnul.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gbzcosjyx.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gqkmnafdz.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gtshbdphm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gqjfhobzk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gynsuolgb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gefknmxuo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gxbxnduro.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gjtfltrbt.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/ggvjngtmf.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gieuvfrkd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gmiwothcy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gdjrphixl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gsumwzcuo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gnvqrvral.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/ggcxduqgx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gfxxeiltq.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/guthynynh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/glddtzzeq.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gzafosjtu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gmqynxecp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/ghxembnzm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gexnoveof.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gglzrvthx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gadgfjduw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gpygsknpy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gpjbehxbu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gitbnsoxh.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gpzqdcqhp.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gvyvhdowk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxgliddki.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/givlgnfxd.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gdjazhuvm.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gpehvesok.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gptkchyvk.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gzgtjvwaj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gyiceaozu.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/ggafvyrgu.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gpvcsxuhs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gguzukhna.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gkcknhdis.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gilfusxnh.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gxbkjvvgf.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gvqzwzliv.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/grtqtzevq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gqwrduzub.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/ghinpetai.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gwykzuugo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gignvfjqv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gkwrbliyu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gwzsprcam.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/grzvgggrm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gutnehxrq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gejvhelvh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdmsgquwg.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gfphqrvga.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gcenezuxc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gdnakebmm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gkxlfvkzf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gyvpxqyzx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gxvplinfh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gyufuntps.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gdtgzinrm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/ghevhypaj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gusqanaub.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gblrqxlxk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwdvgxgcn.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gzmskeqti.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/ghlfafaug.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gryatgmqn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gxffnnojn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gzreuhune.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gkwifjpoi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/ggnhxlucd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtbkulgfr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqmiwdtyq.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gdqfydnjk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gaorolftf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcobiqxrs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gyutgswpq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ggtbhppbe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gakqhqsld.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gbmpiunfq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gybnwgbyd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/ggmgrgjbd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gxfuuzbds.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/grpnitxks.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gauaadkgl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gwmsmazea.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gykupyrmb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/grtwmrzwo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gnsfzaaqt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gwihngwfb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/griridano.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gaxirztcq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gewtfictj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gcrxdrzes.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/guelpkyso.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gccljceox.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gfbsoyzjs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gvhoizref.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/ghjifbzcf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/giqjlhlqs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gyihmoshy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gyvprrghj.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghwoyrewc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gollbqghc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtkotqkik.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gkqtgxnmh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gicqpyedx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzfdokjdf.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/grgcnsxbx.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/ggkypkrtf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmvnmknlt.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpgmsvzpo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwlnxzvzj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmguxfpkk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ggeucnrns.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdfptujhz.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyneuejlb.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/goxgmskbf.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gnuezkviq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gszkudzvv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/ghhcgnnib.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gucmreinx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gdrhdubnc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/guoircldx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gnmeduprs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/ghkqzdifw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gnkxviqhu.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gkllzeyqt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gfggmsnzg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gupeedmon.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/genixexko.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gjpaqttyq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gdxaecxdb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/ghrmyspfr.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcvazuvtj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gznkjsawq.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gshqcnyll.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gswbpbkok.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gttjpdmoy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gwkujhdhn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gofkbpige.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gwxpxynut.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gbbdujmha.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giebpplvx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gmysflozp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gaakatnvv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxoxypdmj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gyrturkab.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghuceuqos.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmvuqlamq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gmllsaeso.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gznjmzcpv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxgmtisgl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gloarface.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gchuocfnf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghewgrttt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gmyqcebcm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ggvkdyzvh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/giyubrpki.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gyxhllzdj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/geabncykg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwbtvfoyq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gfhsrhmmf.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gvsosqpqp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/glnrisywn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gjsgoukbh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/geyudivaj.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gdspgkopz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gqpkdjmvq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gdccltiaa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/geonogikl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gjeniknmz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gamjqglcz.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/glbihpkst.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghobrgzbf.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/glpvnbhmr.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gylbflmnh.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gyklvxsxm.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gigtpljvb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gaecmdmre.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gjjrxfagz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gkblfspjj.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gtknglayj.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gjouyswbo.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/garonasvk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gumummesn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gogzcvzly.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/ggeabzton.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gqkuoedzv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gkarztkzj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gmqzzzojs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/goecvmxxj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gxapueezc.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gaeerddtz.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/geljhhwdn.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/geoqkoytv.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/ghbijbwby.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gwwtmxdeb.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gjsftkgyf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gockqiafn.sHtML


<!-- 参考信息 -->