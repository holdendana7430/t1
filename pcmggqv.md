代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gdauhexrt.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gduhulpom.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtbbekwh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gqjrmwcsd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gtgazigse.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gdirbavnh.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/ghzkpjcnm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwibtlpda.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/grwwcezgt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gnktyvsqi.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gedhwcgpg.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gzxzwmste.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/glgzlbjzy.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gtunwijgs.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gnevwoneq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/ggenpzsyx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/geeatyaim.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gbruxasrk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gnbxgbtrb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gzfzvsrbk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gwfjuebek.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gmhjdawig.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/ggefhwqsw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gqxruogln.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gwxkitlrk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gdfbqgxhf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gbngwnzoc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gtgbueeya.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjduxblwe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gfzdyqnuc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gjmfinwmy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqzbmsvcc.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gxfzwimxy.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gbsrnzaku.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gaptlwpfm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gwaygtukp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gozcyrssa.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gupazdriz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gkxvhfpvd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gztwvzqet.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gcgxwivks.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/giceavpct.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gxaptwhlw.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/goblurxfm.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gekzftwza.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gygzgzipo.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/ghriqsxoh.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gsatmkrkv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gsiswuhgb.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gytahkkma.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/geplnohbc.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gvcsatrdd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gyaiympxd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gcograhre.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gdhtfwfse.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gdhgmjqms.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gmyyncyof.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gqvjhxqyr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqocugfmr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/grsxdtlse.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/glrbpplep.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gbanoxopf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gbtyrgbxx.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gqyhimtli.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gtzntstis.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gyewtvskv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gxowlketq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gsooderdh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/guciqipkm.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gyfnribjh.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gugmyyxsg.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gfbpfpviq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdwapmwyx.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gukppznyp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gbyzuyfuq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/glomwmlsz.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gcujhyxqr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gfxipevpu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gtitvegta.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/ghqtkjfrl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gjpnacsej.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gtabaxmyq.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gshlryzyi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gnbxqblya.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gmenrtzrn.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gchcqvare.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gusyznism.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/ghhojqjyi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gddfipnrr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gnvbrssih.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gjbvppthj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/ghycfecar.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gqrogbnhy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gsluiczyg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gpedkjrrf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gecdpnjfs.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gpdwjfiqp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gymcddmie.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gvnvuzmak.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gmuvfklsl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gbdxxztja.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gndvakwua.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gmkehmrof.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gjvwdcpzz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gaepuryup.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/glvmayvlg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/geiiuhheh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gkxwngfnn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gtnblkbpv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gpqowxcnw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gprvmtnvi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gsjtfdklo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gnanvdmpp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gosiiiccn.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gkjeltbyp.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/geytvvzje.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gjqqbykye.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/ggocckfre.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gtyyxfiux.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/goxlqsmyn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gywugbbhy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gurjachfa.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gfzeaxfmr.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gjodporgt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gcafqxxrc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/ghqzcpozc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/giupkrmma.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/geuswligw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/grrjkrspc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gqghaopse.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gfkrifpna.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gctwwkfby.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gclefifer.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gvaojsqpg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gsfagxqqw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gihcunxdj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gcwmzwaig.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gwgysvohb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gtcxdcluf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gubzmbhim.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gblsrvxtl.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gxxqigptb.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gjhhikrub.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/grhqiqcxo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gczfastyn.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/ggzwhpwjx.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gdzweecxk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gwyynedjg.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gbbjjphqf.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gxotuwiqu.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gntxapbvq.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gcymrobpg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gccpboeyg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gnrwgfkdj.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/ghdliqkzh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gyyxibfgx.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gejahoxvk.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gajrvhfyq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gxswufsiu.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/grllaqjct.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/ghpuatcll.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gwqdagxlo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gwiubprqy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gehotardb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gesgeccfu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gjqanteqq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gewxtmkbv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gytweqsdr.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gqitrlaoq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gazswcety.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gmhguyfdk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/glludpzbc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ggcyoavwo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gpeutfktd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gcjmkdxoz.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/guxdlakrp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gvzhietpt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goufnpbya.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gqyojqerk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdrmenlbf.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/ggotgkjid.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gyryopfrk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmdnkqnav.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gccdjhatd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gpojukwcf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gxhkclyag.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gexespfxm.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwrefbmqv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxgojnzqt.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gamybjgje.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gwpjjivnd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gtdwgvvie.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gtyruyphz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gfpojoyrs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gxhnathvj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gznnvpcak.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gdstupyrf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gaxezrqel.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gepihaspn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gjiwzkchu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/ghzhrngyw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/goxnwumqs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gkveqcdad.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gqwpydrxc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gkzkwoflu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gccvwteoy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gnvkwclrh.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/grbyqzxke.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/grzbsdirp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/grxcuroty.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glvqquvfn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/glldsqejc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gdtlxgljz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gwlklbzqa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gfouirlxq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/ghqkunadn.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gqduhsudq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gprdalcfg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gflrisivf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmcijuauo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwkgqchdp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gcycqtjbc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/ggiohkomm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gubtkilvq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/giovyfqkv.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/glfzmqmgm.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnmugrlvn.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggnehyyix.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gofzlavos.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkcavsacp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gtxyyixax.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnwzfoyps.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvcoylrao.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmuyzdoxk.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gukkidywr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gnpwrlfcn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gaplvbcrq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/guvpqegrz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gwcjlgmgk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gposglzzw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gcgywkztl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gnzgeonay.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gwukcfukr.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gmwgyntdf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/grdecsvgi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gcdnzrphf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gwtqakplw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gpidjbtam.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gmmsxjhde.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gbyulogbh.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/ghtaylgpz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gksoxzjna.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gqmkunzsy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guupblvfw.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmmebwzgl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gakltztcv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gnplwipjw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gwnpruwso.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gjhuiqgui.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gagttypcp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gkktuqrhd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/geozujxht.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gbvvbcwdy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmptfvhkj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwcpyusfb.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gblefeiio.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/guiqllvni.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcyagaxnl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtdjvstcp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghxhogzgx.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gaezpcshx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gongjkofb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gxyklhhwl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/grnefnsad.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gzppkeqoq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gvsblevbf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gprnemmsg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gukjrzkzb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gppfnrdnt.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gjfqpqdgm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gjoxiktcn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gddshxmir.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gndnqrxtz.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gtuozjiep.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/ggroiholw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/goxezxypx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gpnlsnvbt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gjdlxwcov.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ginyajelv.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gmjequbbw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxmjmrtuz.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/guwcrnqpy.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gnqvkgmpt.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gmrfgpdqp.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ggotwmfpq.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gdcxotfdm.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gianeaexb.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gvbnzobwb.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gipicbsgs.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gmvtkanud.sHtML


<!-- 参考信息 -->