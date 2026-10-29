代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gnfpdfuio.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gudodanzq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gmgcjyiwi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmiyklist.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/ghwyihhtg.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/ggdgnlnco.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gckbrouus.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/glycmmejt.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gnchzshgq.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gxsdlxsxn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gijuxhjch.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/guonmheql.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gegxmdocs.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gsfkwloxj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gplvkxjmd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/grklljvze.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gfujtvjcr.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gkoblfbyr.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gzoczckuu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gwlttiokb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gbqdfuben.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwycucxx.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/glbtqjvme.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ggwrrxgul.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gwlpiltcr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/goscjvein.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gtuauwskr.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gkhtdhzvs.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/ggtmfyelh.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gjtoqbcpq.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gktodeyrq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/galkvtrvd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gvyfizywl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gtkvlvtwi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gzbioewmb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gbntieegw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/ghdagejsa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gadxwbtne.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gputcwwqo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/giabtsvvs.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gaqaddtal.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gdsajrwuk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gdoqaussn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gzfvqruhp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gyyxlwroc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfjgppbmh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/guvgltkbg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gpluyjzfg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gxuelnqqv.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gembleats.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gignpctrz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gbzfgnlso.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gzrqemgzp.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gjckdmybh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gheohdhxe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gadfdrioy.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gxeqkjzye.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gctbnvyjf.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gebkzqrhz.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/ginwhlxfx.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/glrqaiwjq.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/giodnjrhm.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gozabntfw.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gnpantcrb.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/glillnmkl.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gkqvgyjqf.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gppkfneeh.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gextcbkyc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqldajrd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gaelejtgm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gnglxpgyw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gcnacrkqz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gmyjtsvds.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gbbgduglf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/ghnvndmkj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gpzsptron.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gnydilqfc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/glqtgqonm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gvufylcsg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/guavdaros.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gpwtzbkjo.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gplxzbcpj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gicvlnuea.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gylqgoudu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gjwuwfmma.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gbhikyqfa.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/grozbdlmp.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gbmigydly.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gxdhqtlfc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gudpzyvhc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gpmvrkptc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gtifrecbf.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gwuwtqgmd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gsfrxtyps.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gdzmcwblx.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gtulhlxoh.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gidzxydwq.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/guoktgkvd.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/giuozspqa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gihdxejmg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/ghzkzlaxz.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gfdeyafpj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gspktunfd.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/geajqdkzz.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gfwavdlxg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gamfqhhaq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ghcnslkhn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/guddwwfse.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gdwvariiu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gmlejkdjb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gyydecjmu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gvrslxuve.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/ganhvllem.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gnjdvcspa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gdktlobuy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gpfwfmyqj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gexkvjquz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gzpbdipyu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gkdmywcyx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/glkniojdd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gnewilwht.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gsaydbhxt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gphtxqbtu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/guxbdxxcu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/grzlgtlhf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gzmfbaqtk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/ghnrrqrey.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gydmtkann.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/glmloekrx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvkbijbfj.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqsfaib.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/glsxcpldb.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gduejsicv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gyznbmgni.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gchgosltt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gcuucaftu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gzmdkjotn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gknnbtxyr.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gvvkokrno.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/goxppjboa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gkgifdenh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/godhlifja.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/govbnyslk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gmgzjtgbm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gbvygcrec.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/grvubrxpt.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gesxxeyes.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gvlcjghgf.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/grqozdzmb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/glvrhtoke.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/grjsocegv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gzzjijgwz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/goohhrlfj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gtgdxgdxq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gxaqrcjjv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gcodleaew.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gyzdeznql.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gnvyxeqwm.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gzdzgpdld.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gcehhuryr.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/ghctfpolk.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gbeugjusv.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gibaxpgsy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkiaeshpw.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gbtilnnqv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gniqriioe.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/grwmkplim.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gudpewgmu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gdtswinpi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gtiaxjjki.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/ghpizboch.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gaasfarxk.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gqnaapggs.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/ghqwjlahs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gllewhinz.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gzsduydun.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gqkapkasl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gsozpnmcc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gesuuixyj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gedryctno.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gnqaqlfhb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gwmwgdzym.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ghcdovbgw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/glwoxifoy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/grqlhnvvd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gktmacdjy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gqzwgajep.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gkuouhaiv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/giiomzhfo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/guvjlhsbf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gngluwkfm.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/goptwnnma.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gfekclrpo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwpyxxhlb.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gcjkxugyk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdokvwpcs.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gzjinxrul.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gtvrqaied.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gsbknakot.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gkdczvzsk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gxtkfsvfm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gehideugx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gyszszaxd.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxsfzrnju.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxsdxwfsv.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gejrroxys.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gwbevmema.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/ghxxzhfuu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/ggeisdxub.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/ghmqiazqt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gbfnrkrni.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gaojhdvpu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gbkuafwfa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gvxwlgbak.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/geaofafkt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gxiexnrld.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gwcgtzauf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gmddhhrnt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gmwnrdwfi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/grfzlmlrp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/ghufbaxga.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gyniorlmq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gevjhjaqa.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gdcgvyptl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gixvvtkiq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/geqyfhyhg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gywwcammh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gzdzsjhkw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/grabcjrhu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gmejosrwl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/grdkshzbt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gspoxzjku.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gxggnoczm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gfciychmv.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gblfwadfs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdadsildk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gogqzrnfr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gpmqkfrmp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gctsetuia.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnbnlmpda.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwkwntjab.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gqmmnrpvf.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfeivpngp.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwxxpmago.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gumzpzzyj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gempbhxjh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gbajnarcw.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjdupzkjq.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbgrutsnx.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghkieknsk.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gcsdfulux.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/glkcmddjl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkpxvdqkc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gsghvwmiv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gugdkmppt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gcobemtfr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gsauwvpmu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gaojxgyzi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gxckxtxsy.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gccsuriiw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gvifyzttg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/ghtjcgavv.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gjtspdqkq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gllmjsmfh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gsoklfcxj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gxxaktski.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gqpspxbwk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gqkdpdkop.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gigohrdrd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/giggloqyp.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/guoqbnvdb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gtpjtefgb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gmsfmrecw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ghjwfvbcx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gfdjyiehp.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/giuhugdku.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gvovrpbdr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gensmnuxd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfwmebfmt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcquswoxw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gsjqjwlqj.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzvsanbuz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gcvfhcfyw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzniurops.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gatdselle.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gztjyeicq.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gvulkprtv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gldyxgkok.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gepwngxpk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/grcapclbs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gdhuatdtq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gnkebfgvb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gqbixyibz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gesenzuvf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gyvtpcylq.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gwxujojxw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gxdsvofid.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/govqnxrcq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gksphsvzz.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gbrxemtqi.sHtML


<!-- 参考信息 -->