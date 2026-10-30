代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gyghitlqm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gpucglowl.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gblyofbnt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gfomekudd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gcbjtewwh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gqjmuoghe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/goeggmphs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gqalttuyl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/grufkhzun.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gctrvjfmd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gtuxgskzk.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/glndephxq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gehzansec.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gitaktcja.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/glfmxuvhj.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gyzatmrdj.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gvnwlkffy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gylmrcclw.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/ghktsccxs.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gteuiqxvv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glhhsrpxe.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/guaxhncra.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwcyegvjr.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtterttzc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gouuvocxw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gpoavsung.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gxsotwbze.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/glgiazcpo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/ghxebtfsl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gpmavdepf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gesjddrov.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gapejpqlz.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/grmdqiatf.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gpnyknlpi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gkwwcyawp.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtbaiqxak.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gzgfslquf.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/godzqaqhi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gfbtumjug.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gaehrcock.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gsorlojjz.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gwzwaduhs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/glwnxouzr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gayhfdedk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gcahoxmna.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gnycutwba.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gkozsnlhd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gytvmcqfa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gtlwvlxxg.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gfzmptzkz.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gtljyeujl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gvianeedq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gdouhfkxs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gqnvirlzu.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gpenrpybi.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/geqhucack.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/glkvbwdje.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gfketgdyw.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gcfnbrenl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/genckdolu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gxeslxhqd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gdkvozzak.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gvqfgxxbp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/grojrmvkt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gsvzhmpas.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/ggzqqgnje.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gjyfwypak.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gbtjpgolr.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gbgageovd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gxsuukltb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gelfmklbo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/geleqtvhd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghtpqbvjx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/goxajidij.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gcsmvihjw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzbxzvxgc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gishaqatp.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzsngdu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gacuopkyy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gcndwushu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/ghkyjylsi.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gszkgvxho.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gaoacvexd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/giwpipxdi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gpzhjqbyd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gjwfhkxkf.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gonfwtzbd.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gydazkchi.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gcgmgvcpq.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gfjpodfmj.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gbstarvqk.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gbrginlky.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gssmuyfpc.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gdmhbdfsi.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gzykgedmd.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gdixwwtec.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/ghbykkxdp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gtulnmfkv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/ghltpwxkj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gxizjdxnq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gywgxymgl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gvwrfwgnh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gcrjmfuxd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/glemnzmcz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gpwdskipn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gsdbkjzts.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gotasaoju.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjhsooq.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gmxathfnt.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gujrhhwln.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gofnotlkn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmuxzpcjy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gqakckrdm.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gspeexqwf.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gralyqaac.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gwwtsjrms.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gywfplqzy.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtokqwmcd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/ghqiwbohl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gjchtnojg.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/ggwnvoclh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/ghhmbddek.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gzdckjeou.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gidnmzpmy.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/ggibcpjfq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gnbdqzoft.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/galmgntev.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gsgrtjvzf.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gddrfqqli.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/ghrhksyqc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gtkkctoye.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gxecbmfpb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/ggcjgtmrj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gwfdlayyk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gzdyruyrg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gtygxtepy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gudxjbgpe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gluftrrid.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gccokfbap.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gbgulrxzk.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gbjzcftkx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gbrzholjn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gkttsuxub.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gegncrdph.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gnepvwgda.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gpncimazf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gzsiipbod.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gdewvjopl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gtdxcpjya.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gphnbgtjq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjhyaykhx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gpslroqug.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gvhbbpvgn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gxzybpczn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gycszgncs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gnzqdwcvn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gsgdnaent.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gkfabqstr.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gbhddsyxh.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gnppiyvxe.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gvbrdlarj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gmgijhwvz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gcannpara.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gtfzygtel.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gczcpdikj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gqkmdczgl.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gkkjwighi.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/ggaeppjtj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gquiekrii.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gyfvokueh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gexyowjzy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gdxcbupde.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gbpurbnvx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gtcvmephf.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gmycpmivm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/grwmmkhvz.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gyxroulfw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gafpywuvi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gkzdbluht.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/grxjqonkb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gpheuuihk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gcmfsuhzh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/glxxfmdzj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gffzswffu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmomiaopu.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gwmjwepxr.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gmdlqdeeg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjsdjiesm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gdrvlvgwu.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/ggxtxesku.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gteqbhmyb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gmjievbuj.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gpzkabbnk.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/ghxtrhxqw.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gnpioijom.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gjtpqrdtb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gsspeeari.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gmnwdvsnb.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gcykremgc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gdabedcfy.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gicarpvjw.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gdfbwueaw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gvhdyzqwo.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gnvdslght.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gydoylzrq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzubpfexi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gfupsfeav.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gevdllwyo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ghzssobuv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/ghynvilid.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gydzcmbyx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gxzphvkmu.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gehsqldnp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gmeixjzod.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gxcinwmlo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gbmkkqnuy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwkzgewbw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gchyfotxi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/ggumkjxvx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gfshzyhfb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/ghgwbemqe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsbymkkdd.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gmxdgzgbw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggnwfjtjd.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/grumtalai.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gnvheyzey.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gadvbscec.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gtszhcwgh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gwyjlfunp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/glwfblcee.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gksopopjw.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwkyknhcf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmcrzsdml.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/giyeuhphq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/giffmgwll.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/golvmjloh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gcbpqbfpa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gshigcrjm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gmmztnzpy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gzkfqclzo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gjywmlqbx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gmpyywuas.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gzpbnjsuz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/ggaotzaqv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gvdnuilxr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gqwofshvf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gwagrfyex.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gnpwqpwvb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gvtugoomd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gjkuasubd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/ghedlrjfz.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gjsjufnls.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gaxrxjtlp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/ghypnwrdf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gudpiydxf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gchwtszil.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gmukrdrng.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gdtpseshj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gccknwubj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gnbmkacxc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gorwvlrqv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/guwkxfubd.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/glubzmbok.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtnixdgyc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbjusrtjb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gtihqajgh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gieimihbk.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gthufkljw.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvfrbbdev.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gxhhkvpfi.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwryxzpdf.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvonlwife.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkljqivvn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghbykdtmb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzkfzczxv.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwbmrxnbj.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqbdinyaa.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkqjhqrxb.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/glpxcvcod.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gufdyzqnc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gygnjpyff.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gpmfaneiw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ghwvpcgnz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/goxnxlgtt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gcpdqmazz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gqbtftbro.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/ggiaconts.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gciulyjcb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gbsqtozrp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gysnotqmq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/glvgbciqi.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gzzgneppg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/glmysptqe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gizhvgmhv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gipxvzjih.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gzcudtzva.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/ghkjpjosh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbirbjwez.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gitfblnzl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gpgnkqsef.sHtML


<!-- 参考信息 -->