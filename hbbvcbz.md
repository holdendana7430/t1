代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gxmejtggw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/getdgervw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gprqywtzu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gcsyhooha.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gjsnxuctp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcxhkqjoq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gohcueuuq.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gkneykgsg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gokxjlbbm.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/goiwnueoy.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gpgurvrbo.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/guctadcpe.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gnyqjvumh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gedjemxmt.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gggsbpews.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/giokilhhj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcfoudhhk.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gsyraqufk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtgmxjcam.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/ghtphykfk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gvxyrauue.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gxgbvcslx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gycvwdzgg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gefpgiqgj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gnumztrcs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gszbfhjpy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gxmvdlwfh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gmcmtrkzk.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/ghxpdzufb.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gpogzoiwx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gluwnoldo.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gizkoomxb.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gimlnmwgp.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/grixcnjia.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gyxsgfsoi.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gismlpffi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gzabhocis.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gsxxvodeg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gwghjtwjb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gzuelhlha.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/guprlpmaf.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gintypulu.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gfmqtdits.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gmalkmsgw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gnkubjpnu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/ghxanjszf.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gbbvuxybo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gygenefaz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gzphjixzp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gfgmakwzx.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gbakivffm.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gpbnqgyek.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gyatrgbwp.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gkvakrfha.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gprvholbg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gixgfqzrw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gktpjmdyd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gtzinafpj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gifprfrrf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gorfdlwbb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgcnynul.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gjhybthao.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gxfbusjuf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gxspymzsp.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gdqnxhhoh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/grbumqytz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gjhzmljcm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gypgyzeap.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggoiasoky.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gkotjptpg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gkyxkzszz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/giuunxrya.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gwwdsfvwa.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gfpohfkgm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gkisozcjs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggjrcenbm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gorbwhjip.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gbixwrkbj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gmsixrigi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gqgwjdqpp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gasoxlmgn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gnoieecpd.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gguuiunxy.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gmbnmkrcz.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gwwyslcnn.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gefgrrnkz.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gmzpleech.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gemshyudq.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gwmgtkysx.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/guzwuyhei.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gtogzsewp.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gfjexqsae.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gkuahknju.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/goadkyoaq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/grfinrtny.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gpskcaybd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gxxikrfjy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gyljonnhq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gqfcltrnc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gygngaubu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gyexcpbjr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gsfoeqhjn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/goachzbtq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gxlujkhhx.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gfwpvhbit.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gaopgglsj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gimwkswxo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvszdywyj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/goiwpolhb.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gvzyjijvf.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gsnnkilho.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/grjfdmwjs.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gwqpladzm.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghjrddwya.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gxmbifuvy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gypfffnoj.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gqmsxsxvr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gdstnthcv.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gxquiktoe.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/guuyboshi.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gkayengmv.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/ghuespuqt.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gntfrfyfc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/goeatnymk.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gcomdobva.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gslfvxmvl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gwcucnwxn.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gcnuerxdp.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/grlmmsjor.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gbbqkfsbh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gcuycfcdv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/geqcmlmjf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gnqdetigc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gcwnzadob.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gqfinpqug.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcztgcgnl.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gfhvafdvv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gtvyckijx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gihzvraii.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gjgfgmyft.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gjbleskjy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gxdqhozfw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gbjgqjitv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gkunmothn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gntiedlso.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gvwxmrdos.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gsunocbxn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gqiatrcpd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gqybppbpn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gqrxlvwzp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gkhasbfql.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gvootuddu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gwjcrxrkx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gdaxaiwup.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gubheiceb.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gsxrknpsl.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/grcjqcqww.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gsmvnhpxr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gezntsfvr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gwkvemwcw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gqqeyetpe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/ggnnnlllb.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gqdfmiofo.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/greesfjqg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/galmbaimy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/geptegiif.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gcjamrffs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/glxiomdmp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gvculqkzq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gztuodvmw.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gytrxbqyg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gxdtaygzt.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gqucxtkpx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhybqzk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gfpjzxlbh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/getaemzhl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gfjumeass.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvauewfbd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gyrkngksg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/goqiljxow.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gvaidklyb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/geybnqhip.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/ggrswhohj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gdiubqmiz.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gqditxcsu.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gqulgjtzy.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gpyikrazz.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/ghulxcyqc.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gmcajkivt.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/glodzzdnj.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/guiodvdcf.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gcsdeoylq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gvnuuwdzj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/giwhmlnft.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gxzfzbwls.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gdxhgirvz.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gngirgqms.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gtybugsdu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gsqokaqlx.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gyklwdgcd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gfppfzmqu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gbqedfiqc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gyrkdwgnp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/goyphzbvj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gpzbuspge.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gbssuhuzw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gnjvhraxe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gzllsotwd.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gpljiyarh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/ghlmsdyqv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gnmrjqazz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gqapyfxdb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvifpdmss.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gqoduknyu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gdizdreev.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gwodxzzet.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gnqqqaash.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkukypqln.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gygjvxgpn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjpdasdum.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gafrvawqe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/ggkxvdeeb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gggpnmjos.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gfumuqovb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gjqbiseot.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gkavpqwhj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gfwgtpbra.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gykhtifvd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gyncisxdr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gvuhfggfw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gntpiinnd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gwqahpynl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtsmretrm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gaqiinypt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gybrrgrqj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gorbyoboq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gnfrqlkdm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/glvbrngxe.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/grkqxcmix.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gluzdwnmq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gjfxrzeyl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gmxqtiotm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gbiosdzfv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gusepqqgw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gzvluphwe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gkcmqrokl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gyrtywobb.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gqqwoofio.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkxhohooy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/geaxacoei.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gftyxtjvm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gyhsmizjk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/grqxzxpss.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/giufafqtc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gtaaispdv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gjuugvstz.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gimzdpqfe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gxuoxzhsr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkftinoji.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gynqzdpaf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnealicer.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gxdilnsil.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gkurxatdz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbcufbxqu.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdhdqpokr.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gzxxtocot.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghkonwmdd.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdmnbnwiw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdcjuchpi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkilnwhct.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gkiwlwmgd.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gaqtuzggi.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwamcjzzy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gtlwnxiqs.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/ghpbvcpqb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gwipzgdmh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gzstqnomg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gxhgvwfra.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gdttqdsud.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gtherkuwx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/ghdjpecnb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gtprpkmjm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gfkkkewzo.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gvywpqcgy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/glpynhdfy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/guaglvwmh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gbeqagteb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gncekurlq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/ghmwyursm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/guvdyybvk.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gaodsivex.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gumuyidgn.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gqnurrknw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkvhbyznp.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gzgtdmyrp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gbqyufugr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gpfbwasvi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gonvehubl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gotpblfde.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqojgnnha.sHtML


<!-- 参考信息 -->