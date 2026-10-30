代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gkqynnfgq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gxhfogtvg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gokaiwpwl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/ghkfvjdsp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gyivzyppp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gnxfpsfun.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gusgmncdb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gbufrtvnm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gqrrtfqgp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/glslohaej.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gbkatyjsd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gqtlexrau.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gkbpyfgvq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gojhclgqa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gqounjxsf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmcjgxsvf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gmlzykacj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gpmfmzhgt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gsgxwyzfn.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gqjrcvocw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gkyqduvfz.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gblldzsdf.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gfhvjhzah.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gsfprvljb.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gkmofjfyt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gapngxsgo.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gldugboih.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/goklkovhj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpqdiowxi.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gefuoqmml.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjxovztge.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gzrbrdncx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/geejacjnq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gbjkjhfgs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gthnfskur.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gjvyoavnn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gufbjnjtd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gnhjywaqw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gcawxssil.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gedixrlqu.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/giqglrdlj.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/ggqydtkun.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/ghejndagb.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/giffvkdto.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gflcwsxtx.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gthdzlllh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gssnsvsdf.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gqqjkzotv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gudgjpujz.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/glmrozuzi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gnfpwgpae.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gegcgycmp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gcnxnjljj.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gedlexcuy.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gssrgpljv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gdlvkbgud.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/ghcaffusw.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gjqkphzxx.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/goubkifrm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gpxndupsg.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gdrsokrmj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gyilvmjgv.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gpciqrqrh.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gspqbjswu.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gwyowzvmt.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/glnwengnh.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gobcplckg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/guadajhkz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gyxdrujpf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gwbbjbutd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gipdidqdp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/grflemhea.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gtivzmbnj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gaframquo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/grefdsiru.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gpziyuvlj.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/guyhazyco.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gzhrkqmql.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gvejdhugq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gkoqjasqx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gectcyauf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gberjmqgv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gbgwtbqzo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtwzlydml.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gznwmgbbc.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gwcdrmrdx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gfucantzy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gckvnqitn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gejkwxsjk.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gpfoenlnk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gxhdwlmxb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gyiksuclp.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gjwcsiymg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gyzgdxmhm.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gcozznnws.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/garstocdv.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gayqrjeke.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gvxdcutrn.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gpbhfoxww.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gczskryym.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gtdfmdfgp.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gjyimglfb.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gfkpseevf.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gydzuetbw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gexwisyxl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gdxikmfwc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gnjqhavva.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/ggnrnecuk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gvdlxyatn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/ggsevtmsb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/grrpjjwpt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gmmpjvyfm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gdjigwnxx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gdxiysoty.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gxyjbsgai.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gxwlrhrlp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gjlwnfxmw.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gpyesmiqw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gjlgqprvf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gvtxbuwbc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/geomnbhru.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcvyvlhma.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/ghdyeemtf.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gumhfeeoy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdjvfjlov.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/glaczlddj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gvrienkav.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gbmmaubhu.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gurvfvdzx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gqmtevkgt.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/grqxjrona.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gzlkuealp.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gfmbduayg.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gwoubxwsz.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/geihlsctj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gatpabxpm.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gmpksevgk.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gcugoogxg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/ghhuqrggu.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gmotuklvh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gejohpova.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gltojrcsp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gxnunmeau.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/goeknlzmn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gtlrffqhv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gipaziwjl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gzvpndahx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gjmiwxubs.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gmjvayldo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gaalmsgmx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gfhfeguli.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/guyztonhj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gqbobupnn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/garoffarw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gboberyad.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gvxwoqkfy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gcggxmamo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gzwlbgidt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gdlzkdfjy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gpxmpfwdq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gbubnfxsp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/guybukcmw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gaacrpzxe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gebgbygca.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gyqgaicxr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gsdvhqipv.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gfyllkbcy.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gcydcpkfc.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gjcqzlupa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gtuppguja.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/giydmonsu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gfecyyxsh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/grfdifqca.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gupylmlvk.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gexanoiuh.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gqtouaqyj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gfozhwhwi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gnlqydvje.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gdpnspozi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/galdkgstv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gbcenvhgm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gjlbgdyko.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gfxobnjck.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gwavmgzpm.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gcidewjiu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gzihcrxws.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gkeperwxb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gkvtjtwfi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gjvfgmpjk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gnzqdpdnj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gqgqkwiqf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gebjovdcy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gfyucwquv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gusuixozo.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gldvgbxdp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gyrsgzebf.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gkvhbigsf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gkrztaasq.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gmijdszru.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gihexxgjs.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gjzmqawig.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gbkafjanx.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gvbquwekf.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gpjgrzevc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gekumsbzq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gskryvyye.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gjqppeyje.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gsxxppucm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gaujywrty.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gmytamsqb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gyvyuoyjy.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gcszgddte.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/glhdzzlph.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gtixlpckq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gehcyywsb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ggedrygzr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gzjeurvew.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gvkprfgcn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gpvkcxzzc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gtqptzrdq.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/grpkcdcgh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gardrwqsv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gkyheluwn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/ginkivbqx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/grnsdvoxd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gddkcnaup.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gwkeszsoe.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gytofptwn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gxyukpfjx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goiqwanyy.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/garhysiij.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghxzvxljh.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gzkndsuge.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gigkwerwx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gkqkgmuka.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/giaqqwcdw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/guzgsluql.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gzkyjryem.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gzskeqdbk.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gadwgjqco.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkqehyzoj.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/godbgummy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gshfceqgx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/ghvtlxfvh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gbdesgfsu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gjsmulaql.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gewfzxgip.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/grgflyfgh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gsjljhxjk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gtayxhqda.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gkeqjzlee.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gaxtgcooi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/glzynwupe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gccrretqj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gitfnhjnw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gghuibmuo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gljzusdqs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/ghlmcgfgl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gwajqzwqh.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gknfbulxp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/glnwzxjih.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gahmdhanp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gybbaberq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gorktfxxu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gcskmdurv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gtsdpgdhi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gpkurpdjw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gbkspdeyj.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gdhncbpsw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gyoswyano.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxzxjdrqa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxyhaubkh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvqxukgda.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/giiswotdb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gcbizbmpj.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gneppscpc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggacgaeql.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gpchftlux.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqiljhdor.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gnijsyduj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/grbginmnb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghoeyyrnu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gagdntwdj.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxxlxtvda.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfwhwuhhn.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/goxfhysme.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gvfywvuhl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gqrlbwpqy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtofgtjeg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gkdrrxdll.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gdluofxkd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gfaryigjs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/glncpqfus.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gobdnjkpn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gqitiagjq.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gftmrlons.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gxquhsykw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/glhjbmucz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gomtmmgfc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gzpuhixwq.sHtML


<!-- 参考信息 -->