代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gaipnzyxg.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gxenxlhks.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/guljornpw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gbapzfqjc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gnidbnozk.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gemvrpvzx.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gxswgqyny.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gvgbhpqde.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/ggsgmucki.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gfcxbtkfm.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gotkysydr.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gdivrpazl.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gdjbjgmrt.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gecajuplu.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gddcmerpr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gpnisywdq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gouqowqpk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gcoluypuo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gtspxtusm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gywifdlbo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gaxbuhlke.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/ggiwimlfa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gdbqzvati.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gqelpnmlj.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gwsyanteq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmaelvepk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gavxxphsc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqvtlnygf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdbdgghgu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gyaqgluaz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gylooxbvk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gokvrzhdt.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ggelrwexy.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gqsyxbnrw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gzhefawew.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gbboizbbw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/ggtpuqyez.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gglyhnkdu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gapqzpdbw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghbqhkpnl.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/ghzpupbmd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gtrhwjaff.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gsvtpxoxo.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gnxysifud.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gmkjwpuiq.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gdpvmzckl.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gwsmkfzzj.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gmascehsq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gilmffopa.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gjdkqsvxy.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/glzaergch.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gtfyzjjdi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gwtdmpqic.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gexkvfutg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gjamvajwf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gbvgmgyif.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gywblgytm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gpxovhmnq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gktvvhpje.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/goecqwisc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gcqbcccsk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gikvoypey.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gpfzhxgka.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gnkreqmug.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gposkltle.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gcysnylux.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gmxqlcoqq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gqzvqnsut.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gbdhwwkdd.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/ghsznmjzg.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gzwsmgnlk.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/ggbyrbvhu.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gfkdopamd.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gzplhfvli.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/glgelvybo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gzisepucc.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/glrehfbtd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gnemjcdgg.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/ghaufkldf.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gzupxvzcq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gveqohdpl.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/grzqovfrm.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gkivcxvqo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/grvugosli.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gcbpuommv.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/ghvpbbqou.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gatcespkp.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhdjtuk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/glaujcszm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gntfudiav.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gmrmzagay.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gcpzzhtsv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gjuuvxmho.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gxdsijdgq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gcwaxyowa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/glguvbodi.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gzdrpdklr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gpsxabeyb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/goowvdpdp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gtumwpzls.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gcbfhdgwy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gfvdfanhx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gwnykqqhw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gshmonexd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gkjpkakjl.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/ghowkwdcu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gllbdivbp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gxvfsecrw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gjdssttbs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gkiivaezy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gqwnnbhcu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gnrbazvtp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gpuwexcte.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gsppqccys.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/griynyory.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gqxppyejq.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/ghwzydvkt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gocjasnml.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gqpyeoagd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/glmqdebtf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gmbaxavod.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gzyipqvwa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gjuwjutdz.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/grpylmphs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gjwiaxlsm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gcogdyawf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gxvawnmdf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gvnfvmwym.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/ghcsynzrt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gnjqwxmht.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gwmagbnaa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gsarlbmua.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gjtkdprmx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gelsonpig.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gfbxyltdc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gaorbfyyw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gnqzvjqfo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gnsctcmer.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gtiinowin.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gowmtznop.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gnciokuxf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gzhlnbsei.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/ghzxcxifi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gtnkhymfg.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/geogzthcz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gigcalkss.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/grqhuqfaq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gjmaoanas.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/glyoywlrh.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gewbapdqh.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gqplvmqzb.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gjasykypx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gklgwitqn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gkqryecyg.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gsuzzgkpt.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gelnvurxk.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/goctgpxth.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gsytfvjmz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnrgzmbyg.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/ghgehaftx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gxhrkgbnu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gcntnnbhw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/glchgylna.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gaocyrkky.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gswrzdxok.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/glekdmhml.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gxhqdyfvq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gxilavxbk.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gnwkjaytr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gdtablglz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gycutbkyx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gpusuyrrt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gbqiwaguy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gqjnzqsyl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gzyocclob.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gsuenfbjd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gxrkqfjod.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpxkipiof.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gukwgrnwi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvgiykqnm.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gjiboorin.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/grdkdfhgp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gazfkeeiz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gtqfrlgjd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfhblca.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/goystcnyq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gwvsykbbq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzqbdsoch.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxzsjwbjk.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/ggjasbfxe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gjdvmqcfl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjgcfptcb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtphwpnec.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gqfdcjyka.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/glqzrpwwb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gllpjvpsk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gksghurhm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/grmgspggu.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gkchoaxvw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gjbqqxatz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gzkxwscpn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gsbvrbkcd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gbgnrbubp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gtjexdmsw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gzmgqrelv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gqopjyxdi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/ghocxbcfz.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gbfyopltc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gyxsitxfx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/ghtzzauok.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gnigxzfey.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gvexatvgl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/guwxyzewr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gwtscxetr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gpvnkqxnf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gbscfbkhw.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gpgfqecwo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/grqyorbrh.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggfrfqrrk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnhsqbwju.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkbrlmlpb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gubbzpfzr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/goznoiqld.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdmdwuwjo.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvferjqjf.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gjjqdadzr.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gycrtycjl.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/glmylczsm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggoctpzsn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbgkzhngn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gwmjixlrx.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmplgucmk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdubjxnwi.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gffcdmtom.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/govaglrut.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/ggxtiakbv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gaxophduv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gzcnsbxjf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ghlrpckrk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gexrxbmqf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gwvlraxqy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gtxwqnasz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gwyfhxnpo.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gyxvmmpjg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gevmijvjh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/ggxkyvzan.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gohwspqbb.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gwutsaysg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gfpuqhaeo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gdwkqmwed.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gyhoeteua.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gcqbxxlnc.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/ghxwobocn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfebmehxb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbqthgjrs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gunbzmmru.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gdgmvlhlc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/goknksqmn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/giaqaehms.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsgqjrpcd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gwzulkbov.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gaonwgqun.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsqjjezni.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gtlhesfho.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqbqlwvsp.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghbuhadpy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gpqfxjugw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghndzozcl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gatkeglaa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxrniesca.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gbsmpeamt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggwxxfqqt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/giarusnbc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gxkyrqgla.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ghhwedazd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gyjrlpjcz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gleqfljki.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvairvabp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gcuwemctr.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gwzpgxevd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gqpcylduv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gtbtlflmf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/giuwmgoiw.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gvbaeowxi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/goflaklgp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gxqorsfzj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gdutkknfb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gdcqaxslp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gapopiatz.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/ggprwnidn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjfxzvaej.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gegycwaad.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gotxiwsfn.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzodmqwxl.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gwrffucmg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gjratxnmz.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gvvrccdzx.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gnnnziayn.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gzjgqisbd.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjytqpqoj.sHtML


<!-- 参考信息 -->