代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcxsoeio.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tkuyzzfi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mkyufuui.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2aquvjvbz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2dlhohzzd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ggvtemjk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xuxahpay.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2pbuoaiow.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ryymtjki.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ldgyxetb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qqhqckac.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zjcfwtko.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2pdwnifmz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kenpypwa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ykokhzrr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kjzhvtqs.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sjgbumlc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yoegqybk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2megocpzu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aellqdvb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rovqhqap.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2xqaxzujg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2juinilvf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wzmldsxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzekfvfh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2bbfrdqyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqhmeodd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yoblxpuy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pzlbqtjd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ghsfvxhi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nfjfpppn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ynmrkybj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qhagdlan.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2odsecaox.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2riuqdydn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xrofqxyp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2elwkipxe.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xrkfrcrb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2iqxhtrhd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dvhatzqw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rgiycins.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tzwmjfnl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lqnkvgpr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xocivrat.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2gwuhvpml.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fnjflyqt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2eytzmubg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2llempmja.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fjxhwvxf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gennwpfl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iatzfhjz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qeogsxum.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wagvsoko.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gkadhett.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2sxcnxumh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dmlmwgbs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gbqdowie.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cnxumnpf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mxbkxtav.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2irqvkwxq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2munfaqux.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jqvavfbj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2efqoxvcp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lfouoaxm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2chhrnzmz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2cewglcmg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2poxvxbjm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wogqrbga.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ahttsfsl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ybjyvbqo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bzgxpsrc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wfxlyyzj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2juiwahqz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jeokwyhf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pvantgwm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2upaihkmb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2drlrmhsj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xhzcjpla.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffaafafh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2upnydidr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gabiormg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2thxuqsvj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jtrujlon.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tcoiyclo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2umkcnoqn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2esvgjjpi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2prvqcokj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2pdppndpn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2upgvvrtk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rlrbyqwc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2bmubxiof.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ytvlvbim.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bomhnvyf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lzhfizvx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dyynmjxm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bzyejqqw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2aqfffyaw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hsiwuqoc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nclhqiii.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fumicply.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tocwvxmy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2krskcfor.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jbeclfec.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jhdbyyjz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gxtlthwp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xrstavpo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jdbeqlsw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cftgdndu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mgeehizy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2caqezgdr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tdiasqvw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hoqbsqzc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vdqylujp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2llbbsblb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ybqdirzf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zalkclts.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dvaqqnio.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cmvuavps.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zzxotrid.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2leqjvxjq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yomdjzwz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2amgrwevk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mnzespjx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ztienmol.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jljuzpfg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uabxebdm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cxfeopoe.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gijacube.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pgbmscbk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yrtmmdzf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xmrhzszq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rolqqtis.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jrctqheo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cfmywamc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2pmulmhnm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fnkmdkog.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mncjtcac.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mxxneooy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxtagout.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbwteicq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kqdiwhxt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gqoqvxqe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sfaqhmkp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqxqgesi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2tjdoiajc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rrxnwuag.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wumvuoqr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2coejjxun.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztrisovr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lweizcvw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jeafmgbs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yaoxeioo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ndjlkmyw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qqecwlxl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2iuyufvux.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vcqbufyi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oomsxfue.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lhrfsfvq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vqttxyti.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2uqhhxvhx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oucueaaj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntapxuvu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jueyrfzg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2uywmlnsy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mknxaoou.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bgdfjzdq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2moifdbpn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ilqsbobv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qwzsbixz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pvnirtxt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2txmfnqnf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2iilvkxzh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ctbeowbe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmkqfcur.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hzhlzmgw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vphysukg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2duvbzahi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yopnvbuc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qeurlnhs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2cwxnhhns.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tpvmwqon.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wsargzgt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2webpebgc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jlzenpza.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hyzwongg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fbjcbjjf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jnvuanfq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lsanqoti.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2apqhgnog.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qlzwubjn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ctqodazg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zcykyfjz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2staumhjo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mhsiqfff.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ddkjibzh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bwpqovur.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ejvkxcvt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kwkovqbr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vcjgkguz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jgpfxtfi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2hptddsyx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlfmxyey.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2edhgyydu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nmpoyszd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vapwxdko.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wxomrbfn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrylucvz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2khmgfmzy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gmgfeblq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bxmzxkou.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zdlgfkud.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kwpaobda.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ksimfktu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2nfxqoqkz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hfcrlzda.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pvvjfhhd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2kjeacrbh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fideketh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yfasssfm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lociowyi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2otwnhvyt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2veshoyee.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2lmuewpqg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sozwzrkj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lhegoxpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhhkplon.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2cprdoydq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2basmzuol.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvddyqvf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rogdhrnh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hjxdcgbv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xwkpkyez.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kxdtpiid.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xqwohjux.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mlfqsqct.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lgvpjyui.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rtnganfd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ckapnbjc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2yhhxagek.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2pniiklef.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yotctyhc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2usmmabeq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qwtivovs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xmjhojfa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2nnrmdbxg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxjnstvl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yifodsdn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lsrnnzmj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pdzjugpd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2epcknxjm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cagkrrzl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2sutobixm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wexddvkt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kurglahh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2klopmztx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2pvaxvkoy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bcggeddk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ibhalitr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2naffysdp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vmiavshu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vngzbqqn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yunwqkyn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hxuitqcg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2iohsfybz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lgxmgact.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2axvsptdu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qvjucngl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2juhcxhzr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdbuutft.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hnlsiwmp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2olewyjvc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdsoeucq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tapgpamb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewcmdyyt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axrvlodi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mgkxmeus.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwihmmsq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzlmgkyv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cmjibgoy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nxxrsxya.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2epvcsdkl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gzlaakdz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ivulggtt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dxyageec.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2krmwcvnc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kdixaudj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bvipblyw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dvaostet.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nsvpmaty.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dhybbutp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bhmjxdqq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2vugofugh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2koxybpjs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zolfixke.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yaoqiywu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cfkenpph.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oabnbhpl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mkdsogmz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zyderstq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2goohxhiu.html


<!-- 参考信息 -->