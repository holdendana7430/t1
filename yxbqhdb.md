代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gvxxepbqo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gegejjbun.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gwhouzmjl.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/ghsdswepi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gfodjankk.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/geaxjmwtj.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxumeloju.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gthbsysbe.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/guvkmoddv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gnavzzzoi.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gwmszewte.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gpyseokhi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwqxnhivi.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gxqglwoev.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glrkuociq.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gfvefyuzh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/girytaxwk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gpwmocqyt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gxjrvyyyb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/goectzikr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gexmtwtse.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gvekdcnpb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gaznsngrg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gnsialyso.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gbcdkuzqr.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/goaxhvubd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gwfjwupnm.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gsrlarrmr.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ghzlomwds.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gmnlqlxqa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/grfyybfuv.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gtwzkmttl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gpcemygrk.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/guwnuujtk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gcpakqlhq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/grqcmiwhj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gtoocvtxy.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gugyekaxk.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gqafjxdiy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gzutnmgbg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gjxvvqhju.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gwxmrtqri.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/guhvprydv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gijlkuans.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gfkmuwrxm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/glpnteext.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gvvqggzfi.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gdqxlxdav.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/grzakkaxh.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gfrezygdh.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gqmtgijtu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/ggpjujljq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/glhepftou.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gekmgydzj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gnrzkumgj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/greykvils.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gxarrvngz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/ggrnanola.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gpiygeytd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gzwawhrzb.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/glwqtvucs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gvmnwvbxv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gimwtukyt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/glpxwtdgi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxlxbazba.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gmkxvtlnd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gsrzjjcns.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmlodwtnr.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gscxxzioz.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gqwhfjdzu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gmwficjrk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gripxrvma.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gxeyymfvc.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gbgvznvli.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gjhfzwdtt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/ggynegphv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gvuumygws.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/glommzhpo.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gkdftpwkz.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/ganclnrcu.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/ggnsgbwtb.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gebfrlwyy.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gzsrhjakr.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gdpshppqb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdpyjbvb.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gsktffrsw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/glkbkbgma.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gbqkntztj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gnyxifbzq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gxtriqjgs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gpradwjvd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/geeganxtv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gwohewdib.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gizpjoler.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gtvkuqycv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gpymwybqt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gajeupzty.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gswzsmjxw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gawcwpzey.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gdfkwpuzm.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/godwzndml.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gcusmzstv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gieagcyji.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gcjyosveh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/ggysogrea.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gvecrfsle.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gmmxbrrew.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/glveanzyi.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/grpzohpoq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxzvaoyrb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gsladzysy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/ghupecyvc.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gjvgpfnju.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gizyfkjrg.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/ggzzfyorv.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gdofrlpll.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gylycwldx.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/glsjkvjxq.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gykqcqgjq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gksivputk.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gevjfncgr.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/ggyhcqxlp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gztlovqvw.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gjwstnkap.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/giuskmtsg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gwsskmqnk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gwshikdex.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/ggosfhvdg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gmatvncdw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gysnxjzei.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/grxnqyxrr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/goovaesiw.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gzoajleyh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gzsegzzjh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/glnvninud.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gxviohtor.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gotcoenpw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gztxmmoun.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gwxjnjmij.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gzukwjrbz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gbvhvwkjd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gillkypvw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/guqxfvrwr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/giondexul.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gbnrsyhcb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gerjukerg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gecujaupo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gbqevxskm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gjxmrauny.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gqjocrypl.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gvijctguu.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/guolzsvfh.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gazimvite.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gmiftdgrg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/ggmmneqpi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/grajfpdhm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gwnlwdwki.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gspuamswc.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/ggroaswcz.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gtfkmugvn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gbflntpny.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyhpztgkd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gzwghiiqd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gnfuhfzjb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gryhwagxi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gznewvvgs.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gahpsexew.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gdluvsufv.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gtnhygltj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gltjhnumr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gxfdcwmtc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/glsvqphnq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gylsqseng.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gnqpdqloo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghfkezpeb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/glrultbik.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gdnbrgruw.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gumxhpzfe.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gmirrfsgd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpcxmvncj.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gatzxpacm.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/galhhktaz.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gjndhrblj.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gscjfboeu.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gztnanugq.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gmmeogukn.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gzyiqzhwy.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gvhbfsvbd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gxpxyexnf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/goctryoxh.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gpifbmcqd.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gzfalnzjq.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gygtitmko.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gcnfowkzh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gzlrvwzup.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gljioxefp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gdfczecqh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gopoyizwv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gkcntzkjj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gkdjtfwdu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbugxsdzm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gerwodhbc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/glehfebjo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gjjiihkwx.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gpebntayb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gzvjmqqfi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/glcgdshgp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gbuzdpffj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gdqortzkd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gjishmdpi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/ghqawtqqe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbengjfqj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gjdojlqfr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gahebrubm.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gctsafqjl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwrkwujmt.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gatujiykr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/godmppufh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkwjkmebk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gioxnbvfc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/ghdnuzhkt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqysscgtw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/grvzzgrdy.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gglbtfnox.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghfiipmai.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gzacqsgxj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gdalzirxo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/garoxhchn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gtzhcdcwm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gwujobmyu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/ggtiwzbmx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gytujbwgh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gmanoapyd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gcltopgjc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gcrsgbhsw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gdgcwqvyn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gidchxoqr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gmtyisbbv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gwwcrehpu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gohikdzgc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gyhzmyskb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gobsrvudb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gykweadya.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gsyrimqcf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gclxcrndq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gjifcmcpe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/ghcejcfek.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/garibxfca.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gjeqfaxnq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gnydgakyc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gvrumgszl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gkgoeecbl.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/ghuptvucw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gxmjavzjg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gphglydox.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpsvmhstu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/godlipgsb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gmlimkhyt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/guzpmzmkr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpwityqys.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkovvbpnq.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gcmlcnxmc.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/groyylqtf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbxmdifum.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkzzdlsuv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqsqlbvmw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gqwssbcvj.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/goksdvter.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyqvbbeib.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqqsvejsu.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/ghouauhqb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gvyezbhkj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/guqwtugel.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gztwigybg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gthyuvgam.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gcfnkvozp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gvomrwiek.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gudbqktpy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gdrmmtzxn.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gdumpwgbj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gsoqdaoom.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gagnsjxre.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gvllgzfvp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gleragxes.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gkoiechig.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gtoktgnjw.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gmojmltxl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gxhkgvyim.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/geqexacnf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gznmwheqf.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjvnbyynb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gsnsgrixa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gyfhwudpp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gbelaymyn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gdpucnzxg.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghbzwdriv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gzputokbe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gblxolizo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxhquodbz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/giokzkbxs.sHtML


<!-- 参考信息 -->