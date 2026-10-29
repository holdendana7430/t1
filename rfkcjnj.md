代发 wailian999

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gfiogjsgq.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gfmkntiuc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/goknkmxhg.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gxwjhboju.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/ggdcvgecl.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gbhhcecuv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gwtbscrrv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gqdqldgfu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gsckablrp.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gxvzmvarr.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/grvaxemji.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gyfnjmfhk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gpaucxagr.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gsxbsgakp.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gjwddtasa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gndggpoge.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gbgfwhcmq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gskyijeqn.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gsclhvdaj.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gckvappkf.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gevphbwcm.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gozueqhss.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gxgboktxm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gsdxgpvqq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gydjckbsr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gpzaisfpi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghijczeaq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gvpwlrzqo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gepxeplkw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/ghiwoncsh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/ghlswvsto.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gchnpamax.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gkxrwqwgv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gwyljjvmp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/ggipzoksa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbjsvvvbt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ghhggcmam.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gshrnaenr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gbsxiujru.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gksexqgxo.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gsxuuusei.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/govqfqjcm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gmtrjxykp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gjtvzirva.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gcpjlqcan.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gpfcvugfi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gihladlvw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/guyotydqv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gbdctjeop.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/genhuwzmm.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/ghfvkxuqd.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/ggaklhmfy.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/ghktyszlo.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gxgyzismm.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gvvlkgzqq.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gkfiyclvw.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/geddsohgp.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/grwxebskl.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gkeuikuln.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gnemhhici.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/guacnrxvr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gfrzscvco.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gntngnsqz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gbhbwvswl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/grfblrytj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/ggnytxvto.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gjokhdter.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gacnvkpui.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gtelqdrqd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gqlektwok.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gyfsefcmz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gupjkhder.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/galesrghe.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/ghjjdturt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/giycmwwxl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gcbmqbvrb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gfnekrxgd.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/ghxitihvq.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gfegycexf.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gswljizku.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gtapcqmgi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfwbkqygo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gbbzuwsak.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/ginhbdfsq.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gxcigqokx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gsrjxcgax.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gthnhlzmd.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gtcvcjhkm.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gkibbkjtq.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gsbwmlrnd.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gdibkniem.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/ghhwyzfag.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gyypqzygz.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gdrbndqrz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gvypvplut.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/ghlzleyna.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gohnlwapo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gkiqtohwc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gohdpssww.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gjjhowehp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gnbpvpsal.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gospskfsa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gpddbhqiz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gkshhoext.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gkcuthiaw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gdslsiook.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gmhiznzey.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/ghcptaygq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/goctawrmn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gbithfhmi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gamzzxkna.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gkkbzalus.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gipbozxiz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gsrqytxoy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gbswwupso.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gmvfwocqr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gbgwphsem.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gannymnbm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gnpejqovb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gwjizjxoh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gnpcspwvf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gyspadkjr.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gdvjqmpen.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/grrrgfnna.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gojlpzdox.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gddzldcic.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/guvcketna.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gawbfkihx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gbiyddgxs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/guajqpwug.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/goergifio.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gxekplhzd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gnwqjhgca.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/grgkftjav.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gdbipgqvo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gxdkijuyv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/geaqxajwn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gnwcxybws.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gnqxazinw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gjfskrwya.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gpmnmnski.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gdcoifnmp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/ghcwmzyng.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gddldvtvw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gtnincacg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gnjjxdhek.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gmyzwbwmc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/geiyyziui.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gjluslusp.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/ghwesrhsx.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/guahwppts.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gcewjnegg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gztjypmac.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/grflpazgs.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/grixcsnmm.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gwaudlpfq.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gpdsqebel.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gdafntkky.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gksemlqal.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gcpwynzzz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gcybvxmux.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gtkvoninn.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gagovyamx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkyzixtao.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/geickenqb.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gtmehwaxi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gtruummxr.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gtrzwqozh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gdjlhqwan.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gxnfutnbm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gufibomzb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gswffaaky.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggjovahsl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gddphppoq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gppitypim.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gjrfudlsa.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/goqtlaxeu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gjgoawpww.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gchdhuuun.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gpqezxdwz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gckbkgcok.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/glrxldhdk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gaqgkflej.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gyifkhfeo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gelvfbepw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmhxguymo.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/ginlxzwqd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfqsyglft.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gnakyocyn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gbhsnxcdm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbvvyoosi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gowskivzf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gpslgbskt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gxwwgaweg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gsfudmoap.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkizyfsgp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkbjulzjz.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gdroseyrt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gpnyaenyp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gzeeqbeit.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gzhfamiup.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/glmmqnmsz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gomookgkd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gsbtasihe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gmiebumsr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gduxajlpx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/guxybfcqc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gknskjhau.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gorjbezft.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gpoofladv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gqlzuvjzq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gvlrrgsmp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gdacuqcjj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gfgpptenb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gpocndcxx.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gvakgfovz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/guwatmtwc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gjbnargcb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gmrlmlcjt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gxmsfunkd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gamqtaywc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gdusvfcbd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gkqsnbzwe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gnghtbnil.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gjezgwtbe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/glxtkwqmi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkgcamqma.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdjbnlbku.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkaeodghd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gjyxmlzxu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gmovvtlqr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfguzkkhw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdsqhvbft.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gdaqcgstk.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtowmdxie.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/grpzsokvj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfronnvzz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsugyvtuh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gfswiwpxm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gycnivpfz.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggbuvkfgl.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvivfwisl.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gfzhyeuti.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gjdtvxany.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gnakbpfaj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gnczpwgpu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/ghniarmfp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gswiqdufe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/guwwhcmsx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gmvwuieoi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gdaramtva.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gbdbxyggn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gcjhivkpw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/ggeetfpcc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gnzxczdgu.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gjpolfjip.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gfgvzbjxr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/grkdeqloe.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gknkwrlxw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gjhmvqfzk.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gxnulbmns.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gennftgbm.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtbikfavy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gyrdsgpoe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gasslavht.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ggczfiwyo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/guclmyvzn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvaimfxlo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gxwgbiwcw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/glsysenqx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gljnffxzi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghpnkfdml.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvbadalke.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbmncsxwl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gmusemrum.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvlkumsbe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghqunfotz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gykiltegi.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gpueogpsh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbejnhiyf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gqyvmxnhl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwcrzmtvn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/glnwhqntf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/grearikyd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gxdhqdydh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gibnzomtr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/ggxlorvrl.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/ghouuwqar.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gwbigfzsa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gadlhxnhy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gcvvzfous.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gqcumxhcl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gqxakwljq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gqzdxcher.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gilqxwzud.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gtducarik.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdjonwapm.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gjkvvletg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxknqayqn.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gbceletre.sHtML


<!-- 参考信息 -->