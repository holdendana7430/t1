代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ukowjpds.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3abzlthbl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tfjqpkab.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3olgyecta.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvurczpv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ggtaunht.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ptffwszq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xhpekzup.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijurjqsn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xaaftlhe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3pnfqyiwd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ayjtlbjo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qbbhgbaa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3mtrxzewx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ptobqxxt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3hkbzlrzx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wzxipqfa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qenpopqg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3udvixakr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxpefzww.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3osqjnioa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mxgqiucg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tliepsef.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ppsmrbdi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tyvazxqc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xeowgzkj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ujdzpzwy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pnxldovv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pucevdmf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fohzhtjw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oscajgun.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gzqtjwuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aucdqete.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dfgkrqbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhdfmiza.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nbcuxzfa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rcigpsnh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mbikoays.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ovdzkkbx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zasygcok.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3nnfigdhk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tdjmhkto.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qdcpfzmd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3feuepfjy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xxubmtkv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gnapbwpu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3sptvsamv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bninglqh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufhzmdme.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tborgabo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bvzeqkkz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cpctahlz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3iuyedxlz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rrstwleb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mpfgvexu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wczgakwy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lqpcawnu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gcjzrlxd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jjsccuam.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tnhrhmep.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3itvpwmkm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3icmsapel.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kwaoklhi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hliynvwx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wktsbhtr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3uaipdmyy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rhtrxgxp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eplymgdc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jxrjluhu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3iawuhmyu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vhlkthge.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jljlersl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ryhqewyf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bmfgyrrv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xbezkbli.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rtswstxv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xwwvfvjs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3moxfacjc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jvhhyiay.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ufqpeplx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3gwwognjr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kgoqulhs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3exwwlqor.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3chmbehbp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3auujzbpd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nrkiltho.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hynmagxz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ozrirmwn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fhwygvrq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jtdazwwj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3mliyiqhm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mvubjqry.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qodstrsa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hrvviqed.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3nytyxohr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zryczddb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xmsigcuq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vvlxqvqa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mprdaewi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3quqqibqy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ctdzoiov.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cjtvdjgw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fcicgpbb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wtpkkzco.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ovjqzzji.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nrqwncmt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vegibitm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3usmkyipi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mwejfsus.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nrkgptar.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sldldpkr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3abarorun.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3egerzqkv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dxjfvgkw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wmcgwdtf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3aqvtohgg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bpggcwwc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xfybzmsx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3esvphoxn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kmytpfqu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fyeoamhb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vkbbkqxs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qdilupnw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qrplcpiy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3rcbysryv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ffrwfkqp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fqndkieo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gnlyyccc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cgrkpjsi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rpeshwil.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hnkgdzbe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dxorrkag.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pcjokvsn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3sabkrctc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gwcjimvz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mjihhbkj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3phsfnaxz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3onhagvnz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dclrvshx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tvcbevvf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dbafidbt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wbdwpbib.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qkqtaskg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3gsluqzip.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ivvzcber.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgqjcenv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3besykboz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nhyjnhsl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eaxovufv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dijrnmag.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3butopqdr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jmooewin.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nklfxamk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vkfhrdrj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hkgrvswj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vlrdoifn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvyagkyh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jannqxxn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dlpqxxmm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3sfxgubiz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sfrneyac.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qbdmblze.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvugedmr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3oabagdlk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3vwcbhgam.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3owyhoyfl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bdvrgomd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wterzyva.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkonolrv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3nqhjbgxx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vteyshsw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3aayjbaku.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3eecwstvm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gwetgtwf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qgnshpct.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hgywunbi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nnlccduj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xyepqjwz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ipzfwyaq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qwjqzghv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3chrusnjg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3anpcwzfo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dgibgjvh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jickrwvb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jbnckehv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jrifnhut.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wrtzhrbx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ljmaqaxv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vwfxzptv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3cjhtjaxl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pqogehjh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3asgpsteb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jxcodbxs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fidghxjt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jimdcdrd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rybcjebq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ygbsklmq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wyinirnb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3kvvfurym.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lxibnbtw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jnbxyyta.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zcfwnmcs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ncyajyfo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bmtnjayf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ovdujmtf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pfubqhzn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mzumrhrn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jzlagokg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3njgdkdrz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qqfqzdwr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgphiseh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cqwpqpoh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mmrvjeug.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hezqtxzw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qeokahti.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3avhcvrjm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ughvawhl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ykimdngc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3clsdtdmj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gmjwbbqn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rpqvooed.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3visfwdkt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wwbmjazl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rxahkoox.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dgwwdazi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxypsis.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zvqmbyfb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iwtsexhs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dwgzcwqf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lsbrywoj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mbkjgmba.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3egfxjmha.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ikykztdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwwvforu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3zfnkrlcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqadclho.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3hxnyycak.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hwplslkc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bvbdszpd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ethdtxdl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ilvopnsj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mhepisgc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hkpighxp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpavzwfd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bugdkets.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qnoeqhdc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3plyrjcij.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbxhxzps.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3obzgpksi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dfzrlwjy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3foxejoxw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nncvukvu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3umwhrroj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmdwlxoa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xoyoflmi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3suwqmvas.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jgsoryqj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kjslyajt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vydkxfls.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3qzsfyrjs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bcauforv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ttsrcirb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xvfzmpge.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3eqwhpioe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3drsfbpmd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gdzxpled.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ttfyaxvh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wwdcrbgs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3npqhqlfl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rscksjnl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ksuzfehz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3msctfhgo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3odsyykme.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xengayfz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yrgthini.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plsflpwe.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3llojoygz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3utbsaaqk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cwtftkqm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3viejgxmz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zdgjwrhe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozrhlwyh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqoaqtpz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ancutqiv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzfpvqfc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gcpmnfjc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3liljcskk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tojtubfr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzhesrku.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bhslqpyk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3biprpvet.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3usskmbpq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3utbvksyu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xbsbltxo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jgucokeg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3dozbuuwo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vgtzrmfq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mevpykcx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3avnyhfyg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3akorylpk.html


<!-- 参考信息 -->