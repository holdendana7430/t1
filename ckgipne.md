代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gnaxgvnvf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gfsbuddaq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gpdzblfwj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gbgphprjp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gjfqgvnha.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gdrvywpvi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gjtbufzit.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gajjdndzg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gxchihsxf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gjdihhdfe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gihwmcclg.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gticcnqkg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gqqtfzddp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gxjeshjqj.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gfhfkgcla.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gfixglnnw.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gsetioiku.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gupowykwo.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gkjuzzytl.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/grufrnszt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkleqjxjl.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gqkxiftxj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcyjakrco.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/glboggjdh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gdfaguomw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdqaiabtm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gipskyajd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gyasmltyg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gwhvjwjdq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gogkiudob.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gwimvkoma.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gesvrdjpi.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gzolrwimu.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/ggfmkvhyv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gufodfefy.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtwokorxt.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gkmauleol.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gcdhhcvlk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gecnorzan.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gqyydxjyx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gkjvkbpyf.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gwwapvaem.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gasmwwfnk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghczxfrie.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/glwjjpeua.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/grgcapqnu.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gkglhcbfc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gxdcuvrbe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gjvbzsihs.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gsiyzpseh.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gnqwhylvx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gctpxneys.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gkhuugykn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gmjytdpzp.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/goneggguq.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gztldlkrk.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gqcofgrwj.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gelfjzhhd.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gnmpjluie.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gkxbqtbam.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gvzggwzwo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gckuzlfhs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gagxhjlxs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gpbgzlsid.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gtbotyown.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gqlszktpd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gartapllu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/ghsmbsdnu.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gmdpxlgas.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gzmwpezif.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/ghdczozuk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gnsgpxypw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gsvrawnky.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/glfdfzxhx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gxlhbrefl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gyuxxrrtw.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbhyzhuyx.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gwvgdfqxx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gwazhewhk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gqzajcohq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gvxpaqnga.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/glzwzdszn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gomtnocjq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gltwheiix.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gfyhxjjwi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gacqxxcyh.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gbwabgxea.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/goofhxwho.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gkyenueui.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gluiwohwc.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gwvibwwqo.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gfzomfian.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gyjwrdmqb.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/grirxgmln.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gmeitwyxm.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gjgasnskk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/glgokahbp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/goxgjxzwn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gdpmshjzk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gumigqhuv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gtunckxbm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gcegkbbod.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gmjlhdcgx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/geujumflf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gwaojxdpc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/glaugymun.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/glzndhkmg.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/grmwoyopc.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gyarmawtx.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gvieejqsr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gkxhuirij.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gnksgtlhx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gwowjrewa.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gngnuqoxs.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gcqsvijlo.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/ggbfgbnsf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbjqtfrqe.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gecgyqmjt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gtaednpqb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gcwfkgtcc.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gwwrqhnyy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtupeigat.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/guikpyklq.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/grnnpzynu.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gzpetywwr.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gumefilkd.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gwljyxwjx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gywxfrijd.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gzpdvovwq.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gnppllfyn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gijuvsmdb.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gukpvcrry.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gnghfzuje.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gvhpserjd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gioqwvsey.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gvdhflhip.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gqnxgyiiu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gtgzmwgyj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gtgnpiifa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gjsbmterh.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/guyqjelya.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gatmucjkd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gfqubqnkj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gvxofbvwj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gzvqnsdtk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gmyibmncn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gmmbqkfhi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gdnetdmyf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/geapwqwki.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gbtqwdznb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gnroerrxk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gukeqiyqk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gkncidszj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcvminkoy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gjxvipkmh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gxbkqxxuk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gnscabwqx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gpvxriibn.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gfjzzlbce.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gftvohlca.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gsydavmmm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/glcmewkbz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gqwhngqok.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gsltwxxlt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gubncknht.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gpgxkqitk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gsolatrkj.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gathcygqb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/ghntrkttf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gurtpppbl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/ghpozjbjc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gnuqsalqh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gpiegeyru.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/guooymyvp.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gvjefuhjq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gwuptjysm.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gcsjnnpbp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gwapsgacm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gfjbnckud.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gcjrjfiav.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gkhcfhgcr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gxyajnpfa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gcuqxbgbf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gtpzidtur.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gxdfznttk.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gxtxlaxkz.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gkbyvufln.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gayilckea.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/geevjxdzq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gilevwhvf.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gtjjhvzgm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/glxgvjvwz.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gkofiyejm.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gbnhfggss.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gkbrxrzum.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gvyshfntp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gvdkmavsn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gaklygwnk.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gjydhxemg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfckkyrfk.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gltuhjcvb.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gpqvzoizn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gierghtkc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gfymtxetp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gpmqevsar.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gkqbhplel.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gikjsfkxw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvcdmsaoc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gjpjdwxar.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gvoufvafd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gzikktwno.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gwupgvsdj.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/guvxfjtds.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/guioazafw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gdanpwphm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gwtwppmqv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gebwynpdv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/grzxiyqty.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gokiaixub.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gwdjqildh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gevsvskgo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gigqwouyw.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gwzucavqx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gysekqndj.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/ghgljnydy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gokroawiy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmkfnvgee.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gllwoajvy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gmetfkrri.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gqrdldgvn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gpihevluy.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzeuydplh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfspvgbbw.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gkckcgokq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gsennevhu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/goxfmhrjy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gkvevbfzk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gkvsozmle.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/ghvvohhjb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gurlrdjeu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gmuozsjpg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gxpudbdsm.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gfvqhgznv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gqrfzomhy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/ghjqbkrhs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gctedqjrj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gxzgjjvrg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gchnpposf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gdsknjhwb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/ggxpqwdsn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gkwhcebbf.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gokyefgty.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gklxmfsao.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gerwsbsjg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gzvhbrlza.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gtrgssgxl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gzbumnxmw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gotjfwsvh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gvptevnro.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gmjkmznsv.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gahojiffw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/glyryuxlj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gztgwfbwt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdumgndno.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxqtxcwoq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/giijqnfak.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gfkkvvysm.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmvtvoytg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdlwadmjd.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gwacennfa.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggcliamhv.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqluhmvrr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grnvpfqva.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjfgxncyd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gurspxyhx.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvxzybxml.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gspvchzkw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guivuzzhd.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gnofqvcnm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/galrciodw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gckgdgwxr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gjjssjuun.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gejkklltu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gtxortuyf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/guftvdmpv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/ghgghnpkw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gwncrgonz.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/grlekvoft.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/geucfddrq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gyhrhqmnt.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gijwatxov.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grkzbpuax.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gjzjsbpvn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gydkjmqon.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gfwdgnftw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gmyxpcber.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/geywpnpxl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmaifxtpf.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvfocvhed.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gtubpdiue.sHtML


<!-- 参考信息 -->