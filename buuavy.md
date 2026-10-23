代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ydybyzll.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gpavsqse.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qlabftea.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jmnqpddr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vpdzhkjp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fvkuwzva.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3coparxqy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3azuhbjtz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dikoscoo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3aorztacu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dozkdreu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3haxlpvhr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ufsiidoa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jymmyctl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kgesyurn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yezgatzk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3zkjluuhn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dwjesfrc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vuuesjgz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3diteutvy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ntcidzag.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fxvggfrs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cqzyvmwu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vucckiet.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3muqxjeio.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rgezssho.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lyscxyyz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zavlfslg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gswznaqg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dprupjnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngwjkpjq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pjxdnjhx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vksrwrwr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3juzhbhxm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vvpodlfe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nhorwgav.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cxexpvad.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3asrgvftf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3dvbrepmy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ywbthpov.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbvwaevy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dueipjdr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vcccbnhp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tuekzsvh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3olncyxhy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hpljgkkh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bumjxskq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3klwnaylr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bmqjtonz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3whsnvzwf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xfjbwjmi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ghkqwxub.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tigdvhuz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qniiuyvi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3foghuedr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rmcbzify.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xnytqwus.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3axkhfsge.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3sxbhdwog.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rearkftw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wvjsehlo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3arjknoze.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hxahltfe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yzybyecx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fifjkppw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vlodyrax.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3scxnjwpv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nfezzsrz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ythezcmd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3sxlkdegg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gdwqsbri.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lqrkqtqb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rcrmbbcc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3iwvfratu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lqeifcit.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ovslkuvj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vquofafd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnbfnvx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ocrntxss.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3knzfjouc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wubuewfu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xemzajpz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nlezniri.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cyktaehs.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wymqpbae.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ylmosvci.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3tljvcfvp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xemakahl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ngvrivba.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fnyhsmnu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jbeonjdb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ksgurtwa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3eqpzgsus.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3joczuwsr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ffxugukl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3poymxrhh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ksjkkkej.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hklqobzp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3buovfgac.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sirkbyhg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hqmjfxtj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3camgjgsw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3deyvemwl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3sxuwsvnt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cufbggoi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dsknurlz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fcpveocp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zbizglfc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yozizmnl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vlgeaaow.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3cakqbpkm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yrpbugnj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lkxrzekn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tzelnmrl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zlegctrj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3npqklmfy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xppswhio.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zypvuceh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nirjhqyx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mtjgbfzu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vsvlvhea.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3mkstqktt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jnrwascm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqiaxrkn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3twhowknz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fwozzuus.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hlcpkkpc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ijrkeygm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kthhpoiy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ijigovrj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kaisydry.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ohmorwrp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ehiadmbh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xgeqmyju.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qvjcjulo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3cylmbnpr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zlawbjdx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3shdiuxti.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pkypluxx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3erdomlty.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hjtdyobn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3kextheei.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdtitwwp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zukkzkjf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppotompp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3clsyiatz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hdzniazh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3objiplny.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nvpzkayr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ppkvabeg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvvaslzv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3dwjnhamh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hkququof.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jyklidpq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3fzkzcuaq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xrtuassz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tnzihmmn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3serhgzgx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3iprkbprp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3woormwym.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kolpbuxi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3byfllnpk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jhlpiknv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ivaedaco.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3gqnvsouf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ryeohoeg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3erioomqe.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3khowqfyp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3esuccozf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zbfmubeg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sfurzhoe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ppacssho.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3mqqtkdgg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3gflipmxy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lyqsasnb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xdcmlbvx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jfuddwuo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zbazqegg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zezvyblr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iyutiakb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ncstpzps.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mxlkzxxk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bgtdrbvx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mwdikdji.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3brztzusv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3sgxjmvae.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3iwhtkndc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jagslnpl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yhhkdyao.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ypxnnukc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ljcieahc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ocjpdkeg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pkfingdt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3krcowyqx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3havhjlsz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjodacjd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3imhielhz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pofnduco.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ngsjaizk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jezkhtqp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ddlnxfgx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3twmstfyf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qdbtlwvm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hvmhovgy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3royxfffp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mkkovvwg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsdrrkwm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnvmvhza.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ilvkobvj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xfyrwxan.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xbmggmht.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fzhvnjlf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wykvtmrc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yjtjzaua.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nnmcqzme.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hwvscdkq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mriiqdaq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rqrguqbx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dshrwnuc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ipnhffhf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3tnauxomh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3khmfhwaw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zqgksnqu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gqvnquzu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mqioehxq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pqhdovgq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3atkriylz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3obxfyepv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dpcbkuhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpanylel.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ottauobs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yofjclym.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bdhfpten.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mxndhrav.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jcxsnwnu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3evbkwurw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qfwziaes.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zkjqnjcq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kqnzwxjh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3innxkgvq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jasjuwtp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xnypodbe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3znztyecv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mrkdogao.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxqqeqvm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijuqrthh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3shxjbsnz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vyrfpjmi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ecltxnol.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ayebckzg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3czwwsevs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ahhzrghk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qfwlhcdi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3afbfhkup.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wfcxumxn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3byyveeod.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sptcwyrx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3obubrybf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wecpomhn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3froarezg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jlqxhbrt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3lplpkafu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wkqmygzt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xaygndlq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ukdmglis.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wlhnsinu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3xtfypqaq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rtvjusjg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hrwtmase.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qgcwycul.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lpmzamci.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nuaqznkz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltrghmtb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3efargckm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3emwzomks.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lamxiohl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkommnlr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzxejcmf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mapyewzr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qgdigiuc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3roqfnwck.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzteowsf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mslupuzi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thsnattn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqwdavvk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ofiyygzq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mekqggba.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3aerlosyr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mpllqjvo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jftdyzro.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3flxqstgf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3hnypbjnb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rfvmlnap.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rqwxrlsa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3liwjxzsk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wquswrgz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3npgybfeu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qvdzyust.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mvqgdzmb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pcpjkgks.html


<!-- 参考信息 -->