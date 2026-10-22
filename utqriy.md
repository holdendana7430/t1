代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2phcavawq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eqohdaoq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bgiynnoi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2baiadtkb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xziwmhfu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mcpznpzc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wolduwqh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ehcbcnuw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gbwotxlz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zshveyky.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uexuaeex.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2grrtjtlw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bpusblet.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2whojytxh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjlpvzpn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uocvqeig.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xagzmowc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pkloarvd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2typvkdrg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hrhonxig.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wwbbqdvv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gchsbwnp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hncaurhn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2pjwnszfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkauvuhj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2onafkhvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcmjdwgf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pfpjhkkg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2eituyzoe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hnwklxdw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pcuycvaf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zilrxdgs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nyzeixqj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gjoxnslm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2onmpjvxw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qlmuqoct.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xskmrrdl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pbrvlfys.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dxdimfab.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gdfrmzer.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rjlbrstz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oxbdtasq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2uxvcarse.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nrwrkhxc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wulxirrk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jfcfnpqp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jyykidll.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ptcygslv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wbolzvek.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xaooxwri.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gjymwhrw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kpqkfrtm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fvddxyug.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cmaxhczj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2oqnzlzjo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rizzgtbu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lggdqwhj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gabidphu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hunbncdr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yjisteqa.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2doeeczjb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vucpivzp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dlgtmfrf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rxzvaqml.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nxqibsci.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lzsknoux.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cncmeeli.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ygwkgzip.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fxiwpewc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gotlpmll.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2cjazcgtn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qlxqvybv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ypwvmdut.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxbmspno.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kwkidzue.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vhvobdkm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uyjdvbxc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zhspohfi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ynjitlrh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mvineuyp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bombwqfr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2iczsoqvg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2mcguyblh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xpmfenxq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xnovcnag.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tnfyfhsv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zkxobprd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2srcvgtve.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pljzychb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2igiiluvi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ajupwtvc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2adnbmbat.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2atperopo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2moxbcctu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rzsdoqrd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jrutcfcb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lrvkgcew.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vjnwjomi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hsbdarmd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2pznirqoi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2phtstsdo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xiyksnxm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2klnyppbm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2onrtrltw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cqzborys.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rekgvpxf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2murbxaqw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jgqqxfow.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jlheunxc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ldogijhx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hfebujpq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yvfzrdiu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tdulufyo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qbcdxsbt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2acdbenqy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2apnenclf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2archript.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gotdxrwo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cskeylhe.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2relllqas.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jwmqcaci.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2snqsjqix.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dyyhldaz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2txzbnevr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2egpzxbcj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rxohkuia.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2amryxbvw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2snlzuptj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2neckfxqr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cpbxpeku.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zikczczm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wwgpqdzy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xlqonrfk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zldakpao.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2izgrvexu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dklwihsz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2azexmshu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vztrmhdf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2crvxggqf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpmdinra.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdpoatea.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cdbxgeen.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tcmtqqah.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2twtzgokw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2unrlznpu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2biujwrtu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sywvennt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2fkbeoucv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ckkypbgo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ixunobva.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2irdnhxbi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2gkossbzk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2axezfoiz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jmfnmezo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2laxonqbk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mobzpooo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvffbqfw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ekruxeqy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2taukknmu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytftfsnd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngecgusd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hivimnsk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wruulyxk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cszewncs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gecviwcy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rsoiscuc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2eocovyup.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nxhgsekk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2iurdwepy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2svbphjjx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2beqewksx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jsjmuwnt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2haaapkrv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2bslcxlyy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lhynnkap.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hufktdif.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cylvzzoh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2inyxgmqc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2oelgfmxd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2bxfomuiu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2pwyslzru.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2flrivexn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vqztzhbw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mrlnocrr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hagkgkmn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2duokjlzj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mkifbkkn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nrkozwrd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hmfawpne.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2lldwyquy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jnapqxlk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qvebzcon.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cxqnxitf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uayvvfhx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gxdakjhh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pojrsvwe.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hetoeisj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dazgrhbc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tisbohpk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ymvqdunw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ofefinau.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrdoueuh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ubvrsbfr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qxnxxqqy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpholouw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2kcmmxncv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyrjleqb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2nhhtqcim.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2olfjbqyg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kidvkfji.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uiyoobap.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iznsythz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uyjiqacb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kingofgf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bjlqkbsg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cuiqywwa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2skrlouna.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxpbnxjy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2weeqnwfd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ihqhgmax.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lmdcogcm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tawdvjmy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jaikckmy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sglkrshq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2exfkdglb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flbuklhm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xntezkqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zugdybon.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2blwfquwq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2fxpolsyk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rsuglxvl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dlogdrhw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jbsotqup.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wunaycay.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fganjgnr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2amwecddy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bhggsllv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gdqmdxle.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jdhbxtmx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpygoyor.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdgjnhxp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hohubxmd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tvbjwhek.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bwgjeldv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jduslomj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hvthmcqr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zlqmwwgk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jrnqkiaw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2plkxdgih.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ltfavwpc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fcmxkgra.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tyoegjdg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2krzpajqz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ysvobxpi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vipfbcsk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2pmodhjtm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vnnxexod.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dzljwnca.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dhqfedil.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ecucwvbi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rmzghfhi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nzjgufka.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2odvjdvoa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nsjalaei.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wlzkxdfh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ideppwfy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zjgukyuk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2clyfjwhy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2krvjihls.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2avziojna.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tqmmduzp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tznprygo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frwttecm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzsnxbdg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujulogwk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2khpqluag.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pprtsswk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwcycanc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2exfvilaa.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2spdzcjcr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2niwgpevf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2duhlsewx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jqvyzaku.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2blxitmox.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2icagenmr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gkjonksg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dfnslxpj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jcajssvf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fcboenls.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2leiadgew.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2baiwzvcz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2igcwaqxt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fgmqjiyo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2csubcsyl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cgrqlvzs.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sxumskjf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qgzwxvxa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qnjekpxq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2pjdqvqto.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2olcxvecu.html


<!-- 参考信息 -->