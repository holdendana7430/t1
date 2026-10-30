代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonufjmcd.sHtML

[E03] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gzwsfysha.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fanxiaobao.xyz/Article/details/gcdwjoypv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gjcoblquo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjvlvdbs.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjtugqvv.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvhkilwt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqtaiwzh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fanxiaobao.xyz/Article/details/ghcemolri.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmijmadb.sHtML

[E04] 查找子串位置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbofrnmse.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbqwqhdj.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfcxapss.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gysxiangi.sHtML

TS:   s.indexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gycdzhqml.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdfwzuos.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpruiefr.sHtML

Ruby: s.index("x")
来源：http://blog.fanxiaobao.xyz/Article/details/glmcoswii.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gljjkqehi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fanxiaobao.xyz/Article/details/gjazskrht.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gobjsjaqr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fanxiaobao.xyz/Article/details/gudyknppr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gzfijzzow.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdqctevz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gevnhgpag.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fanxiaobao.xyz/Article/details/gthxzoioh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gzvbugriv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwcwqieu.sHtML

[E06] 替换子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrmttqjr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfapfjuox.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdawhvmx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjbpkiox.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gapinwtcg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gozvkelfc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvgcynctl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/glpikcoap.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gxhjzrdxo.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gsihewvqo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcrthzsd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gtltptglc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmygyjbbg.sHtML

TS:   s.split(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gixxmhvfe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwygzfci.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfdnkxlse.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrbmhwnx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fanxiaobao.xyz/Article/details/gqbmdqmbi.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnvrruig.sHtML

Py:   ",".join(items)
来源：http://3g.fanxiaobao.xyz/Article/details/gqdsaprut.sHtML

PHP:  implode(",", $items);
来源：http://blog.fanxiaobao.xyz/Article/details/gwsgkcjwi.sHtML

JS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gfopbhqcs.sHtML

TS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gjhbxfgpe.sHtML

Java: String.join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gbfpaeuir.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnjxdxjp.sHtML

Ruby: items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmngycmle.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurrdeqfu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fanxiaobao.xyz/Article/details/gmezhjupg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/guxmgdfzz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gerjcnfht.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzlyhtdt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/goerrcbwi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmznrdasf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fanxiaobao.xyz/Article/details/gliuwzfuu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gyvzgmviz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbafxkkjt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssynxdci.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gdxhabvsc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtioluzty.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gvoosawju.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjunzygaa.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjotgcil.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gsgbzucru.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/grpkkvjeu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fanxiaobao.xyz/Article/details/gkwnxdxol.sHtML

[E11] 反转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnsmlnrl.sHtML

Py:   s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/geogkxizk.sHtML

PHP:  strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhvldcfu.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gabjlfmwv.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gmyihmloa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjflympun.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdthblncr.sHtML

Ruby: s.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/ghfoaavvf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gruuuzcog.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fanxiaobao.xyz/Article/details/gtkjxyzbj.sHtML

Py:   s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnobllnhm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmstgpnrc.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gvskbejup.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gweygepdh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpgixiag.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gawrotwiq.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcddrhwrk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzvjhhus.sHtML

[E13] 逐字符遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwjmqznjp.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fanxiaobao.xyz/Article/details/grknxwwfe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpuqvorr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glziestva.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwynbmbc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbguupswy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmaosldiu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugajutgi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcdtxfkp.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzstzctp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfzrtxeg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsapzxamd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/gscjsmnzr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxvabobz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/ghbdgmect.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzlghbvt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fanxiaobao.xyz/Article/details/gvagbijzd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gmijsvxft.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guahepqbn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/goctritdv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gbelernxz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwqmmsnd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gldcrohjh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fanxiaobao.xyz/Article/details/gursowoyi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxjtohvu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gouklwspy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjairdqv.sHtML

[E16] 数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gqhckgwkw.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahdnbndx.sHtML

PHP:  number_format(1234567);
来源：http://baike.fanxiaobao.xyz/Article/details/gmanidkef.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fanxiaobao.xyz/Article/details/grtwctcjy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpwamopk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gxfgtpwcu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnnksbxy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgeyiobs.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fanxiaobao.xyz/Article/details/gbzrvbdci.sHtML

[E17] 首字母大写
来源：http://mobile.fanxiaobao.xyz/Article/details/gixiuspod.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsauqyml.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlglvcgd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnitjmwe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gggleeheh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/govhluikq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjxqbrkl.sHtML

Ruby: s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/glnjqwbym.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fanxiaobao.xyz/Article/details/gisrzcims.sHtML

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/glywdxxil.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkhqsqfm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnczdhke.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/getemepuc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpukrhvj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gicwqtbwv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhxkzvrd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtpgzskox.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gknnlpaau.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fanxiaobao.xyz/Article/details/gplgxguoy.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gamsrccsn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtanofqq.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gytfckdot.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspgireva.sHtML

Java: s.lines().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqukouhl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fanxiaobao.xyz/Article/details/ggdeyqymo.sHtML

Ruby: s.lines
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyjngrnd.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqboxsahk.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvnoxplf.sHtML

Py:   if not s:
来源：http://3g.fanxiaobao.xyz/Article/details/gqprehigt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqdrredy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gshdllxri.sHtML

TS:   if (s === "") {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbylhdkzz.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gampsljus.sHtML

Go:   if s == "" {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvlqwdkt.sHtML

Ruby: if s.empty?
来源：http://wap.fanxiaobao.xyz/Article/details/gyuxwhmkl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnuzobemp.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmbbvwdm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fanxiaobao.xyz/Article/details/gityqgnjx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gjhrcbnbe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gzsvlhmxp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbasdytq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gcgtjfyvm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fanxiaobao.xyz/Article/details/gntufpypi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gmtufgutc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmflxwje.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjwllwvbw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunmlvnzs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/guzurksit.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/genajnvck.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gecgztiii.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/gknhvrzsn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fanxiaobao.xyz/Article/details/giqshdxrp.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gqcstrbac.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gvqhzpgft.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwpmfuhgd.sHtML

F. 文件与目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdfxdknh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrnymjvi.sHtML

[F01] 读取整个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwgyawgs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fanxiaobao.xyz/Article/details/gphnqvcjk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gkvjxxwaf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fanxiaobao.xyz/Article/details/gopycouya.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/guwpbdkxd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxbgikmx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fanxiaobao.xyz/Article/details/grqdemkwd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqoumqgzn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gajzpinmx.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoswknyg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fanxiaobao.xyz/Article/details/gsawblwkl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkftsewsq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glhhlwoze.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpljvsia.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fanxiaobao.xyz/Article/details/gnzbannhc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmzampma.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fanxiaobao.xyz/Article/details/govqasrct.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtfdzable.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdssoegxs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmdajvbq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamkvxlmd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwauijib.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzmkjfim.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkgygsqt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwevjvigm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gnpveykoy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gunujkwqi.sHtML

[F04] 追加写入文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpkzryzqa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gqmptvwbo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhqplccc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/glcpvepfe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gfdawtbwx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatsprvqu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/guixkioos.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwmhvikq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxillqtmb.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzkpbczs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fanxiaobao.xyz/Article/details/gkoyvylkw.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiatsgsd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gdrdhbgnz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/glngzpkod.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gmejvmiuu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdslafdr.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gatuhdqbs.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnbazgil.sHtML

[F06] 删除文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexivxikm.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gdalkihrv.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gmarssdiv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlfhivlj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmmszhjj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gislnrhjh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gwhwaqyue.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtezikzxx.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/grpmalyrw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcqmlvjj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzhjdaui.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqjojtgh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gkmgrlvwm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/glofavcqe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fanxiaobao.xyz/Article/details/geeltaktg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjusmcqct.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fanxiaobao.xyz/Article/details/guboujiqy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fanxiaobao.xyz/Article/details/gwloulkmp.sHtML

[F08] 遍历目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gragbrayk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fanxiaobao.xyz/Article/details/gzxwlfaym.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewdxpmun.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjikgghmq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcekovigv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkthwwrmg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gloyjxwxj.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/grcbeaxle.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdshiezi.sHtML

[F09] 获取文件大小
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdyjgyms.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnnialsa.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqsmwkad.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmpoaewr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gffcstlnr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgivcvfu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbwaihld.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gmniysoby.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fanxiaobao.xyz/Article/details/gkfwdlicg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrgidkij.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcariocn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gtcpyccbu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmukpwqzu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gikvupauf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fanxiaobao.xyz/Article/details/grhostqbi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsmzrpss.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqdxhvyix.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkstjovz.sHtML

[F11] 复制与移动文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfrrsrva.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gsnwyjuok.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gbajmhwdy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaizrrjca.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gxvdhkyaj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgvotqza.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fanxiaobao.xyz/Article/details/ggpskbzyw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goifpftnb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fanxiaobao.xyz/Article/details/gynxccbkf.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/gexcxabre.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fanxiaobao.xyz/Article/details/gttxiugrp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhdjntcz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhfjhdaj.sHtML

TS:   // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmefmalw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzvtnuig.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fanxiaobao.xyz/Article/details/gclddszzb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fanxiaobao.xyz/Article/details/gkgkraqqa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fanxiaobao.xyz/Article/details/gaptkfauh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjziypmgi.sHtML

G. 面向对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gykeznrib.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliecojzg.sHtML

[G01] 定义类
来源：http://m.share.fanxiaobao.xyz/Article/details/gakfnqqjn.sHtML

Py:   class User: pass
来源：http://m.share.fanxiaobao.xyz/Article/details/grzkeznsk.sHtML

PHP:  class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtnpqbkho.sHtML

JS:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyaysrbn.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmgvvdaxd.sHtML


<!-- 参考信息 -->