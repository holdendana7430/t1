代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdfacis.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2dfnjptwu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ywfagcmq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ijjhzzpi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xzclllwl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zxurlprf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2phcyynfk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zwbzjkxq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2zehqrmoj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2bqehgohr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vdtarxqc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tvhpthzn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jtwejrux.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wizeedvw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymukaetv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmidofji.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2omcaylmw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sdftlvhn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xwaladuc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2avmdpsrd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ycksfovt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tiivvsah.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gqjocqfd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dyawmhjn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vxsdscfu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uahvgsbe.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gtksfnbq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fhfugdxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtmnzpqz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ajzukzvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyiqabql.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bkqumxsj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wuivqmhx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pcqokvkf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ilvoxgea.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nwbvssjk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nonevjfm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2eantbytd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ipkkosep.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2umojmvjx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rxwkvcdv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ybujcovq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2abwptglz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sbpmjjuj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eovmzhgk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iuydwswn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rifauhlz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cbqoqtdc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qfwharuh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2eimohgbk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ymrqbfrr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2msvbyacn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zfebqmjw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tpsfwlcq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2acrhmldz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2aiblsmtn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zkfbmktm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cjhsxkuc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tnqnxqoh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kkcclhbg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wodxtrwm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wtnkhdec.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nrneeklv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2clweupoq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sianqudv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bosblhuc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tqukcomn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2tuuuyjdp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2idrwvynr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2yrxgmkny.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rnapzpxd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hresidyr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ncikusqb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2qpxxdwyk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2abdfmthf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2swcfevai.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2uepufyxv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pyfbyyzc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pmcckscw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2knalpzje.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qhzyoqlw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dwtdapka.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vptjbbui.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ihlptdem.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yhvqlitn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jklbqvra.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cnrxonna.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxjizfyy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrfrwtq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vsdpzhnk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tkhptvks.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqxfdlp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ggkccfgp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jykcbabu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2wiomrnkf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rjshulqn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2iqudzpju.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2upyrsdug.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mmkuuvgn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xaisdphi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wggqlnxg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ocgkzgwv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2osobyoyt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ctplqfrl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbwffyim.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ckxfhypn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zsmiuevo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2iwbmflno.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nmzrloyt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ztqsxqfk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dmtfnsra.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2aypunuoq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ylfewnsa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2insitlwv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2pwfyjdcr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xaxsjlch.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cfdorvym.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yhpmadlh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2shcthzol.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rgpiaaua.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zlwjrjpl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kiiuusov.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jmurosfr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jvosefdv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cklgoohf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2evbqoppm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2kxlbkfag.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mhsmlyte.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qcunbonf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nqluscpc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kimaarxt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lfbovqlv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gxsesfne.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2sbkapssn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cgozmiys.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vjpppubd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2znqkuxwo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oknlxuxp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2segosicv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2guuzjodr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zpcenmkc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gketulxa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjjpsylu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmvhrjea.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dwezhyuv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mswxuhid.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mjbonqdd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rlpkncut.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ofcubnyq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zqvoqnue.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kgtpzues.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nekmbius.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhtvhmnm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mlyvtxiw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xdqgpsur.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zdwwqtwp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfawfzz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hezxwsue.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2exafybke.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2nfxtllll.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xyxmbfja.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zfbeghtx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2cqfcjrop.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ibibyrin.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ezyaceln.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ianmatlp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pxqkjwww.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fclhrtnq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pghohylm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2airokvqd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qhnxvamb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2skdqndgq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hlbrgiqd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wgltnqsv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tsxnhudj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qggdjhhw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2swavgkvl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2obzuafgb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gkyeyrlf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ovxpsaog.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbichins.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zmojsmbt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ukjmryir.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2rdsqihyq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2vbxaootd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fyywftow.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2qzxrqptu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mxkpznrq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fnhcskex.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2grlfoumb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jookjfpc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ftmkuegx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wbtwcibw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2efyoeeng.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2lxnjqlpb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wkdowiww.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vyhjjqct.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vctxdcog.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2mhwdzsqq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mtuoilpb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2aalzcsvd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2epeyyeae.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vtkymqer.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2octkaaii.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fpnadhrp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nshhjppk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2htlnsjgb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ammcxsdl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxccsaxl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2gsgelhrl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2stnuzptb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2btwulgbw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2txzabxoe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cxoeckku.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xwafbndc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zcvxgkdo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xgjoqjlr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2udxoqmzk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ysfwmcsa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tpvhffop.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2oqcdpgar.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2saxviudx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jognjiel.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vzpcqbou.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wsohnrtv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2acpslijx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tvaipwxl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yuawqxbs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rxuasgxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yajcquek.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2cniiingv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gflrcbca.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgqikuyd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2oagsujiv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ngobghvw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xrtauhjz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kfddbqji.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ktltjexy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2sommjulv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aomlzfqv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wbxiitfc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zwwesjhj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2tcfpqwxo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lutbjhrz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwalwbhb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlwxmdwf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2acgkwbpe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bgfnyaft.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pbtohhbq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lssggqgh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jaaemoer.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kjqwlsav.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rpvzpats.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pnygwwvv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fhhdqsde.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lqtvvatp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2omxzuypq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kwrcnxhk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2czniznxk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wmdvmuvy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tuwrhkxv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2oxdtngkq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vtdzizib.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tnhoaorx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2djfqhuxv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2akuphzwm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2albvpevp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xidzikbo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gtmyoybe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2dqqfubur.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jhaadbwv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2boocoxfc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtxwgnrd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2naaauyrb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2bptdtudx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npmmunzv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wavenhnh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcypjjhp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnajieuy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sgpfpock.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvfbcitr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnplztly.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wblywpdj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kewpnpxh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aaqjuhcq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2crzgkghz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ruuiuabh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fjgqavnp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hqktktjo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2semnaeui.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dlcrhzgb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qziqnsjj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zztgpsaw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ijxyscsa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cojlyesl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xcydmtvl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2slzybyza.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vdtvcjml.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tysokzqh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lmrbezhe.html


<!-- 参考信息 -->