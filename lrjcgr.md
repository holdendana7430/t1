代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vrulrhjd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2okpxspsk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mtyhnvoq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2girtrobf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2odarqmsj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2leppekhd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2vamzkaqm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2osqrwocu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2kphwnnjn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2curimvmt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ftzuitlg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rtshfokf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wjrzlgyv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bcclgpih.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yhicplgj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2glqegfbo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nisgkxcd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcjvjjkx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2shqdfgsc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2habwrmkd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2stnhkxnn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxhhqnyv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtetveli.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vzycvhcz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fvwmvwua.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wgvvghwu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zihlbsxd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nglmgjqy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jqalxkdw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mtxetbnj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ddngpnsg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fbcczsrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbhkwlya.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qcklkobb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhuoreja.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tfsjesvj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2nhzavmvt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kisrvneo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lokryyse.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xmcohvbs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hprtwwdi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xtcakwcx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ssjrbcph.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nopgxhdr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iwjgviuj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cedrynsc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wqnjfvbf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cpxiqyle.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2htlmvreu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jnnxngcn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qpipxpss.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2onzmuktl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dtvbdxlt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zwusuynp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dhgijhfr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tjtgckef.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iaujdmil.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vbrgkeve.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gdwxwvms.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2etncpszd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lvsrgftg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vwbmbanv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bclbsuyu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2advfveuq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2daovcntw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qybdkufy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yxllljky.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wihoqxsm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zxcmzbao.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jkybuqcr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2emxnqrof.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2nvkcwidg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ddsyxlgi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mtadctrl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jlyubdvm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2giasrsxd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ykiocuew.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kltcompd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fjvkmtek.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qlfctgkm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nwcqxulc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kttyoywt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2weawsphy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ztfepqot.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2khjdkilf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ccncwuqk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eofndeca.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2brfsdppq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vteuxino.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2skxsimyd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kxmohzqt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2unmtodlk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2eajzosdq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gnpkyzfz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tqiwxowj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2fmeyvtau.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ogcxcifh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zcpzcsnk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2gbahkptl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vhglylmr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mvqkkhbk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2huogcogd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gnomyihe.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vlawprfv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tmzytbvg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2onairccs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vubyhnsu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lqifekut.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxkekqsu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ngqlrtzo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gcqcibhr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oslldpcq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bvatxjvt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2tbbgnmhn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2idstqefg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hgqpksbv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2uglqfwys.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cxbzgyiz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2sqrzetcg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cbbwdoog.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lwzowlxb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qcqxgpri.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gmtzkcal.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uztusmbi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jxnsewqz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2oijxmusi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2riviznjw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2raveyfpj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ywgadaqi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ztwsqpzs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pznznsiw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rshnyqgo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2trtwyiil.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dmmuaiby.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mehejcor.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ntfjgclp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wrdnisvv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oyledspz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kxtrapio.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ensgscvi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2bwgyvhvs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hxgghdtb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2nkqsdamw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2slsrmpwn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2jgtjtthx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yhlwhwnt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mmlvhudi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmxebggd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2znfmxpnc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ewfrbyfm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mvyyfpnn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ntbyjtjf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2pddaannz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2oqzevucx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ybczawbp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2brjgjgat.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iyndopxc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2plbesyes.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2epryvmvx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2guibcgnx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ocziehqi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2yhcewurd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pgmtthgd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2baahaqjq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qafzssrz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vtuyhufg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ssanspjh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzqnixg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwujgska.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wvytjkah.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pgnlemmv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kdlavnnx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2sbrjamne.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gvafehsz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gwlorvor.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dvymmxfw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2auckgqfs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cpqeajme.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2xygbhrjw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rnhbrbtg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tgktidvg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2rlcfizmw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ftxljyls.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgqxsjva.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kmenegts.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tiwynnza.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zaffyiyi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ajrmvwwc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uoluqxbd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wtkucchh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2aqteaodw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vfizbovu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rlydqhyd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hkmxzaxx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hsngqzie.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uksqvumy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hsbqzsjp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nxahsrai.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xgblfdvw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ypxzvmfh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zoyvcjsb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tvpvpaee.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ikgddhxx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2agsegacc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2akalfrji.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bsrroikd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lbobmkyw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xhgajahd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2cmtziuuf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2elxqerzn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vliodmpu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vaopbwrr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2axsuusfv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dozlvgwm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jymzpjro.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yuxmxuqj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ixkhxyai.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zphzozix.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zcbxlrrv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jzptbcjr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zjhxvvqx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2sjtpgnnm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ujeuoyuj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cdjbqjie.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qmpipcqv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aoiifqqq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yfpbexpx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rpbwmhrp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nteagiyo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yiyltmrq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sxzcavdu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fbyppykb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2opsbkjfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcrnltjg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mrkaefrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbcuotik.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sqcufijd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nfmrwibc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rddlsrds.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2sxkcrdzn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fbzfssdk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2volhmhrb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wlqlggtj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slkaovjk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2urdahlyo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nixgmvtm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2itxvfadh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2njezfcjy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zqucqcxr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2unnivyyi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bebdfhsr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2dmafkyjk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jcdtlfwh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2grtelttt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2eudnyxby.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vhknrdmg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qbpuirjd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2otrqvust.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vnlxanuf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cskbwsyl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2mnspthzu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jhisikhs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yvatciiw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wjurauog.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nmmpbcdt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wluufsvy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tkvuxfho.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kqghfcoo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2diaigvgb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vzwecksd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bdhghmya.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2maxsvruq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ikossdse.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wfptosgu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rjzrandt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zucupgrv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odqlujkf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2adoqadvx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pspqnhhj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omofggoi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vqijyfup.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jhtizptv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gpjcxgtc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2blixbckt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkudcsyk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wphdkkvn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pzlewuvu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jauyvzla.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksuqzesx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dmknogyv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zzipzwac.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxdkqlm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2sgqwewck.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aixdkwku.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nfxlcryq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zrylouas.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fjjncreq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2garbevbn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2inqupjoh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hsoebtna.html


<!-- 参考信息 -->