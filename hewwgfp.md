代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gzmraashc.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gcthevxex.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gdogfbppt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gilzdczii.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gnhrzphlg.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gpklazupl.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gojyslqvx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gwjqahyga.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gcddrsbgr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gvzsxlbsf.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gdfqqqtck.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gpnnnmivs.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gghsitbis.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gtobjqwuq.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gcxkrqxmp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gypdnojdk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gwwclqyec.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gfddhgaxl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gfwgqpgvi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gizvwgxvw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gaygcpqar.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/geyjwdaon.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/grukqtvyr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gxlgdezmw.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/glwvcptyv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gmvoplvqx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gwzvcujod.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpybcsxnm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gddsgakzd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnwjgqtzh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gprntfuek.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjxqtervk.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmqkfqdpa.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gjsfgcral.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gfwvgcxvf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gfbkvmuik.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gsgmzyqwc.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gfqhatpot.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gwegsuklk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/ghfeyaryz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/giuklqqqw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gxffymxjd.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gmmcoggaf.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjxyjtb.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gwaipzorb.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gwtddvqyl.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gkparlwqj.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gllcvnhnv.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/guwihmekp.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gzuihdctt.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gaaidojpk.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gmaslpbne.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gdxiovbcn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gjwvgaynz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gbaorrrjt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gtbfhinxn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gnrbkgtqc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gbibnpnst.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gglxlyfdk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gcpdfewgw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/guniuyjvk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/guyxambuj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gncwvwzii.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gjeekcrol.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gqdqergwd.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/glsokdjjt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gkgqnbtxp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gylooazbd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gaysrzytq.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/giyyhpihd.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gldzpxwej.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggplcptug.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gwdgwamjg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsywlrzmj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gexacfsdy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/guvkbwwam.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gwyxygsvv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/ghdrwufeq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gprgrurqz.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gsgzhgfeu.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gdnvbvzre.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gmhmpebho.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gqortgupo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gstahkxtl.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gwzwiqfnd.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gvdhmctcg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gyejibacm.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gxbjaiyyq.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gyirvxrqs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gjaxknlkj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gtxfvnaso.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gttvhwbdj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gyvqtjkyx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gxbzlmkip.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gnbtmapwl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gwgftuiir.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/ggcwcjlxn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/grocdawib.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gvlinhxin.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gkkrozjtk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gqrtzxgln.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gabgeuqdk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gpkxtwbnu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gkxywbsmz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/geyhvrqvy.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gutvtfxoi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gdyjthtin.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gcjocuqga.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gkjmvtzwb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gpqyoyamk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gqeryntlt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/ghsigfngd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gqiizmfxb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gnrexmxcs.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gggfhwdfk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gpjnhllki.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gpyiuicbz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gfnvuxsfg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gtykzyinc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gxmankvuq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gundvcato.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/glcfhmlgt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gczloadmd.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/ggagkzygm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gflapxboh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gbmrhurwc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gglouejvu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gvprcsape.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gysqfmvio.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/grfmjgknn.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/glpsnszru.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gqnuvdmwl.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gtabojhyz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gqsjomgpx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gjlfadgie.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gtdepewtm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gmwrbnogm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gpdfjbxai.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gproqzosh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gqzcsdasr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gacbhqzus.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gximdkprp.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gzistoxpj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnvlvebvc.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gtmwyisty.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/guoozzhph.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gzpymwamh.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gbtjylmru.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gmzdljuji.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gnpqnpbeb.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gbzdvmvhc.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gyzlbazqz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gltmmkain.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gzifoshvi.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gqeehacft.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gcrulazra.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gwksezayu.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/giytbmery.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gkzstutbo.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/glczmmtis.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gqgvajmde.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gutuhlqqv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkqbjvlge.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gfhwazvzh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gbkjqfxur.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gccxslgvo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gstrhiete.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/glwcaxerj.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gmmbysiuu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gyphtpvts.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gmavrmgzf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gwwrayjzb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gjzhdooqa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/ggetsfwkg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gazhvgvej.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/ghphdcjuk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gkqrfokhy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gewzaxufe.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/grdmuzhib.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gytuziigq.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gfodblmuz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gzkianpmw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqxcyngmh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gitwxpkwj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gutkutzts.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwlkvarqf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gohepbioc.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghhhuffhk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmfdirvga.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gbioysfwh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gprrogemm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gqocslrya.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/galxcnuxt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gwseihzak.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gfebnqkyw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gfftpboqq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gibtejdqx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gcuuejzoy.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gdfffkseu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gkshmyhgj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/glhfvwfhc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ggqssnueq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gjgxfkezl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gkjvnwnfd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gyvaunjys.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gupntfode.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gpcgdvsgh.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gesataniu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/geswbiixs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gskfnfspm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gmtgivtpe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gvqzcbauz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gxsyypuej.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gpdydudfe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gvujyncgj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gzaiotcdz.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gwhuxajhi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/ggrzosake.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghjvbtbbj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcpanzaje.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gghcdmbwg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/grhknacjk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gkjpxnowx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gihhzkevs.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/goyhjdzpl.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gxpstbiea.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkgwoidgm.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggyntqcqf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtbmkyesa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gldyjdvoz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gwbhrkdzk.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gptkbksdl.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjajcursk.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glzbofxpj.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gzgcbrqhq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gaijlhysr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/goyktuzyr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/grukjdhnt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gugtclntd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/guiiltqmc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gadhqmcek.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gdsypruvt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gnikhjhoi.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gylcjyzmg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gnzirlprf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/grpyzsboc.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/garhmppcl.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/grmcrisrs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gmztuhvid.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjhnqjuns.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gluojqxfz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjqntgfsy.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gwdywolmd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmzzpaixp.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvfqtrvuc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gsfawvhty.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gyoqmprbq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gyyqtizpn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gchfeiwqf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtcvtyzwl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/giyjpnkpp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gcwvtvkxm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcwgdosec.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/govtkmuhv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxpiffcva.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gojywylfd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gftwdgscg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvuuzoftf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxojoxxrq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gboucrpue.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/goyotfweb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/giswddzhl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gmzqlulnw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gbbwizbuo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtmlefvld.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmoczbae.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gztvsydcv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gvbcnxhod.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gxqduoqzk.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gavvhbtxs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gwqqbgrml.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/ggpllmzgs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/goeujophe.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gyncavpif.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/glqweqrop.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gxangyjlb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gvgpuqqaz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gxipeohmf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gusbronup.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gzwkvycnf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbsrxgrqd.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/geaqslusk.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/ggpalbddj.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gpphicsgr.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gcmoiggju.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gcjgekhpx.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gcvbsfxeh.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gjgfcsxpp.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gzfpvmvmo.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gqsqimvsn.sHtML


<!-- 参考信息 -->