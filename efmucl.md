代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmcycokt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3epxtuwty.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gghwfryy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vhjwfscc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vyjqecft.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rniuhrmk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3oycztdji.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3darpumck.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tpajknll.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xfakribh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mxryytut.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bblnrdtq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3nixcigyh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vesadlgk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ewbiswco.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvmwryys.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wfdfhyne.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qwhevxqf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qbkhnjlp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ukmqcjwo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pbhyxonl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rawxhiyh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xxamlykv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jdfcapym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuheomth.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gajqtfrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpgcpqtk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cryoeqhb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bwiatkkh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3annfgbtc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zrrvsjdj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ddrsjiqm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3anklqmqx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ogfwppxl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qvbzzzun.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cvczxsit.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3shszlafd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pxrhkimw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fdrxwrrh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3junvwiaq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qbhxjvtf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hbtmpcev.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qqlpiytu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3esydslzw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nglrfoqg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mkzktujb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3orpaapez.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yhlnapci.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jvxbndju.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eciubvnc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3txrwgwxb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fifxyomr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tqbzjhnl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jmbjysro.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lahpghzu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3blabmyji.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3bioabjko.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pkrwvzrc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bofkjguc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hmqrdvme.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zwfmhpat.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vaqikzfb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wchbcmud.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vpwivxej.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qjmspwmw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3deaweszy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3frrrzmhk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gtkroadr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fumqtxtq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ujocvhao.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qxubwrfz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dekgcwny.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vtahlpsv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mmogrzmd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3doyvzyoh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oqmbatsn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3chnvrpbk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sygiscbj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dyveqclq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3faehpyyn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3swfrdxob.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sebyjrfi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hqjdeguy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3baitnjhp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kfumsbkt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3sjvijzko.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ffxavhms.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3jysuqdfc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mietccrf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wvfxluvk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kgqtosjm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bczninve.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pneftqdh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3haeilcaq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ntplmnhi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdneosj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3uqjbvjfy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3muwhkojc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zqruhxye.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3yovzmzpm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lpghwnpv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3oqtrhigd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xheedser.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pkknarkh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3olkvkubg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3wvejwows.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3diykzpjb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cyjbnnbt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dxezcjzm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lbkfkdcy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rajzswpz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gvnuqdwb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3krlitpnw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gzmhjjjl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yxgyjufg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mxounofp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dmqfirhv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdxiqwmt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3brfhgjya.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rykgchvv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gsrwgzmi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cmqurrxe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3twvpmfex.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3psiqcxfx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fdhazvpa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3znmoykcb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zywccdux.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3acngvbbp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3sucaqsvu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dkkauata.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wgauutca.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mccjcnnv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3uqlorxsj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rhxmzqcs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kdxfbxjp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fiapyiqc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3lwqmhnmm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ixzlynnd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cegsxhkl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vjblpsxf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bnpawiqm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tcaxzgjn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mhdhyjpg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdpisssv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3eflvuoom.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cpqppsao.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ckyuwysr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3yakfhlwg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gugvvmia.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wudgiabq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jvjwdflv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ogqcdnpt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3euktkvvi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3sgnndbzp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mcyjwrzx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qojbrwnf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ntrkecxl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cvoocpyb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mrazczfw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdwaxreq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fjmdgxbw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tljgtobq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jpjfdebc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rkdstzla.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3yawqijnu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kofyvkbb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3oeffknfy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pvzmjzen.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3exhfhuyn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ccxinule.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3huqhupya.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ykzjwjpn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bwvoktki.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fbaguybc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdxswnlb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xirzpcuq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3optrcgxn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ardfwrtr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pbmfpxfj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ufxvvudd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jshtfocu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3umbmtlav.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bushayuu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wyagmbjp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nvnazioo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kmpnblvu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cstmmies.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3kaupvtfl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sucebgfi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vvpyhxgi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rysxgxvn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vnywpals.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xpumzoib.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nwzgrxmh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vpqatxnr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dolyxewq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3baaobwjo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3oftzivmu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3lglugbkk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3kqdfejmo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ldyzofqi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3fnlhgzdo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzolirft.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pyuveyqx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpkoeayp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3tfazdzys.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zankfrlp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mpedfqnq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3sdfchwlo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zzalcxcs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3byiixkfm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3slzufzxj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iihycuwv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3duyupftw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rybzlqtk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ukqjdrvf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3etltukhs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3gfuglqgt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xxpjglwn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nkhdkpdq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wttpfgnc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fmngookb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mnuvnlfr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aczcfstm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rcaxmmjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpzlczld.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pdgieabf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkonxkya.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnxwjgts.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ykdteexc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gxmyuwge.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xaqtvybg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ljtnjzzn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jxlqixvd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ieywmwec.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nyfivcdj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gsshhuwl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qzrzvgte.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xmcrowou.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbyccsgq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3osmhpqea.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3oxovqers.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3afwpvysk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ovuielwj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ixedtcey.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3jacuwruu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hyannbdk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3icvpzchv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kyvfpdvh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qzymrkrs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hzknlcdl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3uovmxbzd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3leaawxed.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ypzkozlf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lkcuemmd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xohfbrxr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vtxsqpmo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hnbwyvxu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lwdyzxvv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zjnpambh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bqcwfgoh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fzegswnx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dgdbcavy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3thoijuay.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3pmakstzd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3soqfohdb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yzldkpes.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajxrmajp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrhsimtz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tgamcblo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3llenolbo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3coyvijqn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkzxvkzd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tldaglfa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqurqujo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3drgknyze.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbruhkeh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpzkutgw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zmamuzxt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttccnjuw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ilgiytgw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ihlsmtsq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3feagftwm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nxdteyhi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zfqqoica.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gndcltov.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dxubbpux.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rrcjpylx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3npssgdwj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wfrgxmbc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3fulhvshk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3dyrcdfbv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fxnygynr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivhqchuf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3monnepun.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yncajdsq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kwbzcobe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3mbmzfdrs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mzzuvttz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dsdsfggx.html


<!-- 参考信息 -->