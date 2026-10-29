代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gckadbhwx.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gqqpelyex.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gjmlliipl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gnenhbzgd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gxsqwalbe.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gdmvlqzrj.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/ggyaxlwch.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gzltsnpzw.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gdhgipapn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gxntsashy.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gqxferchv.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gdtxtqkyy.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gobjaauit.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/grectndot.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gwcxxicer.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gjtkaeyil.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gcnmvguhw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gfhlhcbwf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gztzrrljn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gdmcwbhsq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gkpoczaaz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gejhdzbjj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gmoribjzr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/guyuqahip.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/ggxkllese.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gsmskwcat.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gvmmshpxp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkbvjbwmc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/goimzcara.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqskoddem.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gyqaoretp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gtzjztpmi.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gqjmhekww.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gugwwbxqw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gxwzlrlzg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/ghvexecsl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/glythrfkm.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gfvcuyllf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/glrrobmlq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gvgxbrgmf.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gjrrygiou.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gcwoikvoi.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gjwroojrc.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gzpgzorpa.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gmhkdsvqg.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gpzhutrbi.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gkzpsrezo.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gbyiodljt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gkulswlke.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gfmcruyqx.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gpcqvxfmz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gxyevzgpf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gokntkftz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gncicpkpd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnlrxnm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gvoparcmy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gklhhknls.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gvbhcaxkx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gywtbfpfx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/grwvvdhgp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/genpdsepb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gyzzzmeiy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gnfxphgoq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gsclgqwjx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gnmqwfdnr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gcnyfplnt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/ggxagfixu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gedbmnrvh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gbipzbtpj.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gthgrrpry.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/geotnnbgu.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gfzlodswy.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gfetockzb.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gbnflntzl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gdpnbqaez.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gjwmktqjs.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gsrdysgid.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gpsxbgeyq.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gpdsiliiw.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/grjxgvqoi.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/guwfygawj.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gqmlozwsp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gpetxoyhj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gkfkhpjjw.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gevpwqcyw.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gcmkytqbr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gkvztdssc.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gvrnmiuxz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gfquhyzin.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gpdogwnib.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gcnfznkfa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gbziodkzh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gngulzznw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gtnoklsvm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gldwvfchf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/grqcwckvl.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gwtxkljmv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gicjaqiiy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/glexiqorl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gahtxsgsr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gismuuzsf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ggbgrdjcn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/ggfbitmgb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gxhxoftga.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gopjncrls.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gvxmfxbgn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/groxxsujr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gmrxqhbnu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gjxyuhzxt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gfajzdtll.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/grwgyqnvj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/giwnkootl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gxrgrpxva.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gixejhrmt.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gtsotgjkn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/giwoenmxv.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/ggyibqvxf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gmqlqqmcn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/glblncekt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gaqvncsej.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gnubvjypu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gyysumiki.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gkajriyeb.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gsksbkcfp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gkoyzvzza.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gnycwfupd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gigetagtc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsimvirxx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjnjifufr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gtdghxoea.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gsaigqejn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/giiroufvg.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/grliwxkbo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/giefjiuyq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gldtfbybd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gmezlpibk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ggcuxsnov.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gmbyankyb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/govrcetni.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/glhmsgiuz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gzdkarfid.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gvzxftxzw.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gxqbvwtvy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gkhnnqnan.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gkikwiabt.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gvsfioxmz.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbjiiywvv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gfajinwoe.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/glapkhrfy.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/grxlsibfa.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gcethfnyi.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gzizakcto.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/galjdghig.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/glbjcudgi.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/guhftupag.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gjbqzzrmj.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gddxyubrm.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gywmmdrqd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gifqolhhk.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gloigiwsc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gyyshbnzj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gtzrouobq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ghaciyguh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdlkwushv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gksdcaxdl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gcatuvcal.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gasxrtyxd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/glxratwxf.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gotljpayg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gussjfohq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnbwncpyg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gslnsxslo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gjgtxvrmb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/ghimzcllv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gbrikiurk.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gslqkjgjq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/glcarqnet.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gabmnbeqm.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gmrtrbrpg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkobilips.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/galoafmmo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gbauxfqii.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqemhpohf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/grqfqcwur.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gjgtgrcoj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gbknoxmva.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gafnspzup.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvdbjmmej.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghrzuakyn.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/grrnazfqr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gvimhqzbf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/ggwrpboya.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gxzockhwn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guzfmoaec.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/guupanqrn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gowaqzoxe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gcsxvwtsk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gwkscjmps.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gwadixwtg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gvvtubvoo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gifecyqrj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gjoyiovzi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gxjbaklxu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gblgnxwvu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gkgmnlwoe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/goppsjrxb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gyradcznp.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gfmfewwdn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gxosbmuma.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gpokrgwwp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gxokvmbzx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmfxqmaec.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/ggrwpcjfa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gmitzcjcb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gninvgnbn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/ghvwtktce.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gkyjkgria.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gqknrkwdk.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glfdcrhnw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grbranlch.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghjlnulsy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gwcktncev.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/glmazvbec.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyxfszdij.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gylntnvpa.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gjpieyiut.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geytmasuj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gauajhtuk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsdxmshke.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gglfscmhn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gbrhlyjff.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/guwfdaqju.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfzvzblia.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnsyvhfdl.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gkbptsvjq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gzlsazoxf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gaabjmqea.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gilaqhcez.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gcmahshzo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gmtxlyvdm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gfkyaarzu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gfbokwhhg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gghbaleta.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gcfsbwqvy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/giwfnnlpi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gffjzbtiy.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gfiecdgym.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gzgabsraa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gfotbeqoh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gsakoorxv.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gkjkahjus.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gtfkcpsdt.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gyrcuifwb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghovldpdg.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gynpmmcix.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/geyczfdfu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gvfbkugwz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ggdndqulm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gkthmunfk.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyyhlkzcw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gmgebdzec.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gsumqrljm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsfgrqpyb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gfpnclfqk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtbauqjbn.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geembsjnf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gocyyxaqs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gksbuunnk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gssrlvrqo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpbweywgu.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gtztlrdwg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvylewqe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gcawfmpyr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/grtlizebn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gpnxrsnoi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gsruzkpex.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gmnjdbrhg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guvnghlis.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gvrcsnojh.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/getzrgbhd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gfwhdhfyk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gaxuxwgzr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gsbutujhq.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/giyqnyfnu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gnfeohlvr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gnxqlbbkz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gbvpzkdtf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/guvabtkqe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxhpowrqv.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/ghaogdnlx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzlvswsre.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gzsiqhoqd.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gbjxrmgtq.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gfuuqebcj.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ghmrrbiiv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gohbzzqjr.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gudfdgglq.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/ggyugcijh.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gjaqbrpet.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdeoeknub.sHtML


<!-- 参考信息 -->