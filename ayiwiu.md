代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mowqjeut.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nhdnmwmi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jbebsgin.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xzeulbel.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bwbmgyox.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lfncfxur.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bdleoxnx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zxphfons.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jemknxys.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2gruliabg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lyuiidif.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yimxhzwu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ufqhjlsg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xlncydek.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgydwgoy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qfqusjns.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2szzdodhp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fiqfnofw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2essushur.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vhrvyhub.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hisrulpq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dltpfuga.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2raievqpt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2elyrqjuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjapjrwn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bjobipdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efxtpfte.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bnjulfsf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ebiwdjgx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2plyyycfv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lmsdlmrw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uvaxgoze.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2pzasafcf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rcjaxkgs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mcmhwoeu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vnfdaxoo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ixkzfysf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2iaznymcp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cybgxnhb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xitpozip.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ccwumkbq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uvohupol.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bxqxwuon.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lyvihbfo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lamglxex.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gxrmtcfn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2gheaylnq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xnozrwvh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vpnlmzcp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pwiryhvh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sphhbjwl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wsaqoyjo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lgykerfy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qjqgijsf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2teowqbzk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zgqanrkv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2altblzek.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2uimbnhah.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dqzkyzyh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hmrbmpmm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2foqizifk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sadbills.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vxoiqmxz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2miuxxwyf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rewypqrt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qozmiepe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fnuzlasr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yivteazy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xmaoswke.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hlzlxaux.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vhrrlims.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kpxbvyno.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zkkaunoe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2omkuoeig.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2urbpaiux.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rswetkfb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2izhqfjgd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tqvquhqa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2denomeir.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2llxvifmh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ccwrfywo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mbxivquu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2onanwmfp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rsbmhtsl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ejqyclja.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2oqkpompo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2yokkuqyk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxudvfzr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hezovyqi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ewcfwkfu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2uhjapfci.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2gvegjlki.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kogqngrl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rtllqxtx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zgjevocz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2skczneol.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2atjnezpp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ejwlhviz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wwufqluu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2byppsmlp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hlrslqtl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ecsoewpz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2axbwlxpg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mgxvnyzl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wiyvkxzn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2komsqqhh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vkkhthzg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ejwejkxg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2kxlufeyq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xwgvvlrb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2uouveijn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pzyxevdl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hlgvdekr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ogytpfpg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2elebhtyk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qaluermg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2xukhlupc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qnlxadjj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2iatgryku.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfdwzmsl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iyrqxbec.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eovefxid.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2plkwqwkb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xspxthjg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qxnkcfaf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rdkesezx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2trznsuyq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cmeznejt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zswronxz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hzujhawg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xgbalfhb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wyuvalrj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2udidccyd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wrbbuvgv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ewfwpsoj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qhptkeup.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fatmkfjy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xccaelox.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifegdnda.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpkmgmvq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ukkqsufw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wvmvmefp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mfmrcxqz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tedcoavt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ylqpktph.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qokvpymp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2thscdfuy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qnkqpljt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2iermxovg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fwjjcapi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2tzaqqwtg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lmbbdznz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hmrqykcg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pqxnbwap.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2adqerzmt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bkfkmpbg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xubesutm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2axdppdhe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qbnwurth.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwyrasbp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pctwfnhp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfxkmfjt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lnrahphb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ukqloxhx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hyddzqhl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dhneidlv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2oripiivp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jilhhibl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2aunixbuk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fykmlbze.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ldzryhrv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sovhhvqy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2efveusdi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qwpxtgdu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijffosnu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxvmdier.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2girhwgpa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rhhobqgv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xzxqyrde.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fvazfjpw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2bakfmktt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bdcayxvh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jryqdzph.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sgtkagdl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bvyvjjrd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jstkqpzm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqxonvhg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kisonrgz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cpwbznbs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ttjdgiyi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2oudldlbs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2engzsvwt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2drtdidim.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gskudceq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uckpqzpt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yuzknezx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2pnextasw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2errydpzd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2lrmvgspf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kfybxsvz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xkcnrycu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2njkdppqc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2acjdjbif.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpnaphfo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgxmbnqt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nhckmjzr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xubzxfli.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tghsyths.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2hacixmli.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ntodiqsx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nlzlyahd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rpbtubrs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jxbsckrl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2tetrjvyn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rxugvjda.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cyngctfq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2rseaphkx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kwfsqryu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2asxzmmgb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xastjius.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aodkcrmp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2krtvqwna.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2azztvbip.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2smlqonwe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ybrxxlsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdpokrir.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zmgygmnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldqtolch.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmkzdtvh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2abqexzae.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xtzrzcyh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2expabwfb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ujxzbiet.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vqnjodyb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zuanpquv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gdskwryj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2owbpiobs.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ambkjcaa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bwvqgpxv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2fqysckhd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2esjqraky.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klspxfny.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wafwfeao.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hoyskddy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qtnrdrdj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuakxthy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2radcghww.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2quyzhhme.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rqzsimxz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vjaonbbj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tfmhvkrw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sncwtpoj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2gyunyczq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2yznowwgr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hipkwrma.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpvzxxay.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hwmqbtfx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2imwqaczz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dhvortgr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uwfzufvz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2eratxwik.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qdkhmvkr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fhllfyen.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mkrczryc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cmjrdrrs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fsvfudby.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rygfhhct.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tekrobiz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbytamkf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kdtpwsmn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2kblaqhgd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgzjgpul.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqcdvvrh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2papiqcpa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ywjxydop.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wvyxkbrf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jcwcxind.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frcxhofv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ifijzwqc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jccrnfmy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqpzizor.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bkrbamhr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hylytgcc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ipbxnhvf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jzpjsjqi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zfdoljii.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zvwetswl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xkvatbfl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ktcwecba.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2agmcitkx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hwnpqttt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2outpmwmk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jercjboj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2oqhlrosu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ydqllvpy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2keuhtdvu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rbsggvsm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pfsvwzgc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vhpxqdod.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qlwpiizu.html


<!-- 参考信息 -->