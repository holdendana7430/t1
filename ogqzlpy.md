代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gwihwvavt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvoaivf.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gnrwpuchf.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gcwzycmez.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gxlwvugqg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/ghgxbfjgd.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/goxdajfpc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/ggplycnez.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghevntxqd.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gpvnxszcs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grmcqpgie.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gyiyscpnc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gytmdqtuu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gtqzhaopv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/glccybhoq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnznixfmh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gdstwlzpk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gjzrrkevb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gzeedswsq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gowwknrlu.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/ghyfkczmn.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gqgmnumso.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gvrjoxfmq.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gmtskmcmq.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbtvsthqb.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gebfyrbut.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/ghggutxns.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/giefxhjfz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gdpyvcuod.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gjlkyhvdv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gtajfsydp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gybjkkaml.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gzavckvmj.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gexahhffp.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/giykzqwia.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/grzrosmkv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gratxogcc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gkpbqnxrg.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gbaifjabp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gunuekvre.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/guxpxixsw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/giyfhkjci.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/glalhqmwk.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gojtwfomz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gnarpawvc.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gdsslnjjh.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gstugecli.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gnexuwuky.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gijjoerwf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gqtnalczz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gexdukbmb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gtejjycbv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gnwqtiewr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gpgjxwjdd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/grabbvmfr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gxxkwocog.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gccgjvevn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/ggozeztwz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gwtwcfnim.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gphzkncxc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gozwhviqk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gdemsrllm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/ghnesppdk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/godasfyjh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbydrmugj.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/ghueogmdp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gpmrvovcj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkqmfysls.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gbrlnymig.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gfmtfbrbg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gvysyubdb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gwfvjbemd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/guljbailf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gjzllzicn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gkgmpssjr.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gtytmbtas.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gfmmgrkyn.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gwqjbnzsq.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gphnrrjee.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gbchqvsop.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/geylqtoqb.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/ggqedorvy.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/goyrllylk.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/giiwuoqwc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gawohzbmr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gsknwrmvh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gfcbsnncd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/glkfdkhgn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/guuadtwqf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gplvvgyms.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gsiolpxnu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/ghibbbrlj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gmcyouxyy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gcjozlert.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gejprqocw.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gddrjbczu.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gqzrjtlfw.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gmvwgxqyl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/ggikbtfln.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ggejznrva.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/guyuawzao.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gvgqdtrcg.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gxgegbtho.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/goagbhram.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ggmortvvd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/giimtclli.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gkfhuepnx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gbtrtlmfc.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gzbntryyv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/guclavyyn.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gebzsnnnz.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gnqaykrwv.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gqpmjoglo.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gnqpbulbz.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gvswqaxnh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gwkpbvsrs.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/godnhwxtw.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gjxsqdxbi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gmyrjkptv.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gkzxueqsr.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gophxrbdo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gbqhjiptg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gvkvisdfb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/ggenefchx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gvsosruvv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/ggxmtzzuy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gqiohfrpe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/ghouofdgc.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gtkocgpyk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gymozibkk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gohfiuykc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gxkoygtks.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gyqmhoxft.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gguhttpyq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/glartmkii.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/ganrfwxma.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/grcehsuai.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gydpzxxmr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gfxjamduv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gjnovhnlu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gwbjepkxa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/ggnwoehqw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gjiqnrldh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gcvmsdeyt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gonpbiqjx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gkawetywf.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gqnpwusrl.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gmojsdsbl.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/ghzrcfmyn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gcyigclym.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gxhywocte.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/ggoqqgzdq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gzjdcaxha.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gssqdjosb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gilvvndwa.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gejjkwwsc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/geytdvrml.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gmwmdsqxz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/guxoizxfm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gwbxoxsbk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gjnzmfdys.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gmsmbgbst.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gmyuzbmew.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gpoezvxkr.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gzbswesqd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gkawtcrel.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gsfmfuerc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gdnttwlec.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/grrsqipmf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/glhjxfybq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gcumjlbjr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gfonxkbek.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gkbxaicit.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gzwgyxwel.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gmuygpmnq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gghnannbx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gobkkmtoz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/ghevcvlba.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/ggdfbirpu.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gfmbcwgib.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gzpcxbdtp.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gbzivlmvx.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gimmrhepo.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gsoscvaaa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gniziyini.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gnstnkaid.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gziufxavu.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gisvieice.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gnoscalas.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gpcvpnytp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gnxczuqum.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gbedxqjdk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gtkazbfsn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gogchyvly.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gbpgqrvyn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjyrvcauq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gnrzcqsaf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gfqjwkmke.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gprnzhvsx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gibknohnz.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gbcygxhdi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gxcducxxb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gprfssntm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gldfmfklt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gnqpzgxmo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gxidhouof.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gpfjjadav.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gnzhwwauc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gutfeucow.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gutmprfek.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gqdhqyhbc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtckvhutr.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/ginkjjcsu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gyhkznnas.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gezccyllz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gkijstkjq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gjymyecxm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gldyndkqf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gicdhazpb.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvfryhtph.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gflcgunum.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gwlkwvtlw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gusmkvhve.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gnfbthjsd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gkkxwqnon.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gjavezvqa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/govkogxkg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gxzlkjftu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/glgjrykxi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gfmubitbi.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gwyxflqxs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gfgaseghr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gwoukaeje.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/ghdztumkx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gbjqhrzwq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gpfqttrnx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/guecrrzse.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/ggaeqxqfx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gijctsvqf.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gzqcyoszx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gqexpkxqu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/ghtqtzxdu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gteyrgbpf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gzzvdghta.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gleuoltde.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gvxzdutdg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/ggajmfelp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gzztggjnr.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gimyjrlnm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/ghbvixhuq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtcqlnxwu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gampufsdw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grjjgowld.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gisemhngf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gupmpgvmk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gotlfxlpp.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxhboxodb.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gvuunaxpy.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjzdighjl.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghphgqfjb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzrtmrrtm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geezuiujp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gicpnwjka.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwpnfmhhp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwinhdawy.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfnytlmff.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gigbvgrvz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/goudaowmx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxuqmefsb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gjmlfqcaj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gtwypjngm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gbchjptzy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/ggsekcjoy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gtxtjcimg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gvhacynyl.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gvlmxivqa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/grapjdpuz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gzzzwxpjf.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzexlbfoi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gyegybwcd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gujznonxv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwsvzvxou.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gitmzfwzr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/ghvnwtiph.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gbagfaqmu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmicbuifq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gchtojjtk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gcxmicara.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gxwsceatz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gjqgmpxlx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gqcznvjbh.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsgrrqzzr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gwctwvifz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gdphrvuni.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyzvnamyg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gjzjeidfg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqeluxuro.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbmmuqjkp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gvyerzaha.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsvazshji.sHtML


<!-- 参考信息 -->