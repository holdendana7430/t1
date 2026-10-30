代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/ghdlkkfex.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gqnfwakhy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/goxhwxawo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhkddmmt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gyilrmfph.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gtdexaoil.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gfcrrraod.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gecmypkuc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gswsjteft.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gosclcefk.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/ggjcrfokg.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gyhdigjlt.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/ghofpyang.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/glkyespeu.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gdenvtjcj.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gueuskqrk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtaxmsglu.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gjvfjgqxe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtrdeeawx.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gmtjnlxxl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gnpjrjeal.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gtqeytwiw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gwlozvaii.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gnjytpucn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/grynixpnq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gbhiekddz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gujujsfbl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gyvdytlcw.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gmqowknad.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gfbzsgxir.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/giiytvzoy.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gtwefwxlt.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gllpbhduq.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gyybrxgyi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/giancjoly.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gvuqasvqh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gsuglenol.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gpdnvamjz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gghosifhj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gtbojqwgl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/guocqkqfw.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gtlsndwxv.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gahqydgan.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gweieitpv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gucifhqrh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gwsztidyh.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/glngtkvdg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gqihuewmc.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/glaszvxqt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gmbsbeldh.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gqrtpuhdu.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gchhmwyqx.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/guwmuxavt.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gmykdmqhm.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gatlqktyy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gjkwzdtmb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gjyofkmnq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/giswramnz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gckjpyiyu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gkqzhools.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gukfoaexk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gxegfsedf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/goaiejggz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gfpseejqn.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gmdlzdqby.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/grururbwa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gsjydsalq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/grkfcifsa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjcotrvmq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvmckgixs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/geofiivrt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gitbrnfaw.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gvqoqoujb.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gvaejluss.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gdxszkxpc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdhnekzwv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gqmzkvyqc.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/giurpmcls.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gwlbpvvoa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmmiqbaja.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gpgwyinlx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gzhfjvjhc.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gqocjsjit.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gebspvrry.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/guvbganfz.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gymnigxbb.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gvzlyoztk.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gjlvyicuf.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gdfpzkgxj.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgipjdud.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gkjpeuevb.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gpapiewsm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gnlqlqubb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gcosqhajw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gzmkxpkrl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbcitfrad.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gsyhsmzjj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/ggsvsppvr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gtwgxklbh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gdjvxjpoq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gldznskbg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gsspxivwb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gkscygkgn.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gljxrguhr.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gqswczbdd.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gpbfwxoxj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/glditvbsv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/grymcjnre.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gscieaqnl.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gqsrnhsvb.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/giwmlxlqw.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gzzmnfpxi.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gvvwpeznn.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gmqskubyp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gpxsvcvjg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gkmvnvnls.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gvgcyjozb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/ggaprsnmt.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gjsqwnmge.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gtjvpqfxq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gwkmgadgt.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gseeojgod.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gzsznatev.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gtuswqefc.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gywnhmltt.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gmsrariqb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gqmmzrxsb.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gzidgmdwg.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/guaxzwaoh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gnogrxbun.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gptpmqyke.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gtxvvpjix.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/ghttzcfxl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gmmxkdvtp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gbjithzrj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/glonwoyvi.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gbyfqonhj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gmytslenu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gmzufxpnn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/geynpwykz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gkyebsxoc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gndqrfoes.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/grtkimmsx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gbpetgcfn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gyzfgmcbq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gafewibvn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gagnwtidl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gkakgoktp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gmphltfps.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/glstugevr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gsvrxyphs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gdemfzwhy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gnigxqwqm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gxdsbxytm.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gyrtdyqht.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gwkjnerrp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gdxowcmmb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gbiptdypj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gobxfapau.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gkoyjtjpg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gxsfcvtqw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gkquwqopw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/graclbwpl.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gugwypfsi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gmuooyoeu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gixmlimyf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxtjbbogv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/glxgcllsk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gkvphusyu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gulpdgdbf.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gdzrgjyyu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gngibuump.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gfbmnfuvf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gbbjjxntj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gwpswktyj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gbqgpjwbv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/grafqijgy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/grlhvrphn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/grwpbkhuh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gwizmidmo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/golugknki.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gsxxghjzg.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/giohnsgcc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gjrlrsmka.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/ghfppjpjq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/giopupuen.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gvgvmeyzi.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gtzhmnlxc.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gsmaypbov.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/giplugndz.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gqgqqqosn.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gnucwsudm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gfyqyhlxd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gucyoaqyj.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gqkwxejtq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdwqwdwrd.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/ggxpbspfz.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gersncuwk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gsyqqonad.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gbgwuuxnr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gbtczqbem.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gxqkjdyub.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghapotkmk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gdeflrtfc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ghgelecsb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gsegmlsdx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ghafeybqn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gagcgesvb.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/glpmvginv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gaqalqblj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gdjgafuxf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gpdotgkjr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/giinxdfjz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gippcfirf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gfrpdvebb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gbnnrtbwy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gvzmnwexv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gziqtvlbo.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gtqgiekqk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/getpuxopb.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gigfmgswm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gvovmsrit.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggaynqouo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gqlmhhrrs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gotcfsrwk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gqidtaipw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gqmdhdabg.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwblepfyq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzskfwcka.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gdlnmuvyk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gqywlrbai.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gangecssy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gqxlvcfyc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghbazqdtq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/glnmaabfu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gicfppjbh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gtmzuxyyc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gyojljlpz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gixpgicxp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gyszglxxc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gxjxksdux.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gfazzetqm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gqzfohszd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gxxxvilnr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gwjicfgqh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gnaihyioi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gvvobeosn.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gctqzyhhh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gvytctqrd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gxynjwsji.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gtxhfwogi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gxpwcipub.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gbtfiqquk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/giwaycrur.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/glkzwwlro.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gljvbygbm.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gyllfsntw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gptcdgepw.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdyoeswzh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmeczsrfq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grcswyvhe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ggqfxeuto.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gyfccxkuw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gflsktngn.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gauklembb.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/girigdwgy.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/girvnfpdr.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyhscznqo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfubmvbbv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glqbhdkhw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/goudcliau.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/geckkijao.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gralyejpb.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gdjbsgzgw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/ggmqabnvv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/geyrubzzd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/ghbkhifxj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gcoehssvs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gqsuptcgg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gskytnkff.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gosjpxwac.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gcyownocb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gwvdhndxd.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gifabbdye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/grponbggb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gqmozpwcp.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gmipwbmaa.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gaqtifmnh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gywioihmv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gqielqlbj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggyvczshr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/glqrptcrf.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gzilsvjxt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggpwxkyre.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gsdtbgfev.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gqpdqszed.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ggryfcppc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gahfzujzy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/ggbaeonfj.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjoewjhtn.sHtML


<!-- 参考信息 -->