代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3bkbghsyd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qwmneeln.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yyczhfaz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pxrgpcrb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ehjeicko.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jvgolukq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mpenvcsz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wfwkonps.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rxpvzemh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3arwcftzh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ytldyqbh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvwhtggt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ttcrqlrn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ejzutgtx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3isqftvni.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hawakbbh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3burrddan.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3agzsmwdh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kfcrbgjt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jtahogjy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fmulyuzy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kccvqnml.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3liomgcsc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wimfbhqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvluwiux.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3psuotdzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eiwjbrpz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jabmntme.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3jikfsqhb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3purmssmn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qzprvagn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3juaajeoi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hrwbeesf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3adumnnrr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3qjtzgfnc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qzywkswi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3iwrnzjtt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3feahqnhf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qfyimrng.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dtrqjkgo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dbymrujf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ezzpzvgk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xmabtbgh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jdcgzeuq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3grhvwnfs.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qxxqnxlc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3gpslyaeo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3omvdttur.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hrcapkkg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wxykymec.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nvypoyyc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kgafbksh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zpenxpog.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dtefbpss.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ttxnkpmy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fvmajrll.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3powwvubl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3dggixwbc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jejurwcp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ddtokqri.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3odknqvek.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vchksrrw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hyeuvvrj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gcjbfyro.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xzztmqtt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rxjdefxc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vvettljx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rhooarlp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xlqszmrs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3omjrwejx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3btfiyjvh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uakwjkfh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jgujrndf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xaoelkwi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3afdctcwz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3njvjedzy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ehnsubax.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdwnckpw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3igbfnblz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tbthaiov.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kekcpqcz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wxabqsij.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3mxtzcwxh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pshtrass.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3haqehyqn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pmiagjgx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hjiglguk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tdakivfb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qvnmszve.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3andytukt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uuwxwwnc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3smxyhkjw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3asqrdbto.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dnjvpbov.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kkvnsxcj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nvzahvwa.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3iocknyqw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jjrwnutf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jwjafnxn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lgqynewv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zymsnzsb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3krzrptaj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ouoircpa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zuzmiwah.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yyrhonnc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3brvyouen.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hxggylgp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nmrmkjem.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xkhyjksi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3njmyewtl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wtqkwwdw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3locndzmu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gpwgqljb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3twaprvzj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sliyxuql.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ejubpvrg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wpvwymrs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yizvjacu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pbgkyqmh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iqcbltpc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ftxdmvtt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uubupcvp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3jjwrsxgh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rmlztpqb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ckpkvswi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rtupzgen.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3eebsypko.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3evinnvhl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3bcudmoso.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3amirilcf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nvczxuys.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3drqvqmrn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dyfefemn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dddhgewd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3afbiptmz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zimspheb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3thiahuxa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhofyabk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyrebmwq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ulmdhbom.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgwzyqup.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kduhjrzl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3udrkwszc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qelnvfhv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vwihlasd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xebpdzwv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zxbeizhq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvceeim.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbjtwbob.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yunxxuxx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rkmgsrpi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rppihgvz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cpqyajco.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bjyemuno.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3corrnvsc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3liuazfai.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tdoglrbf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pelselhj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gaybwofn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3srceyxvs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfzycupu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckmbmjtm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ybzrcqvm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hvcpzvhz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3pwyfcjjv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cexpkvau.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iaotjfir.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iwjwpppy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3proggqqu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3njvhtmzj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3reaoeznz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3dmuaztby.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qbmlwuyw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3nbkwflnl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pdpskyil.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dmmzooze.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3llcnpnfw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wwjqtqav.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tqhnjeek.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wweamnev.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gsqemvmv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3agrfcqbd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3cgczxmcl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bzyewjam.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wdjtilwu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3osvsosju.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vsfuyefx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3njfmrgcy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pkfheneu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xjmcviyk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hhlchbwz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cxeezmnj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fkhamxrr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3omeealhq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jipqmhqa.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3axgiiekc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ybzsfyje.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3oynhfvrw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3rkoufohs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3faupczsv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nreaphcs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkgdfqzi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jvcqhrda.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dzzuqlsd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfuhvxuw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hbzgvdbq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibqqxvgi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3szdsshcr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3opahlqpx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bcsvfmiv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cmbfjbpd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dzctdxfl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cjxuobxl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kkzgjtyf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ckmqwqoe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gtkkidfc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lveymjzl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3lelhfrfw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jgbpsajw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3obxlfoev.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sikerqew.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3csgxbxkv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3godmbenb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iovxvrsb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vjqlcjsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qburxecm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3brqipebi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qurildzw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xthmgoaz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kiberpdl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bqpcgyqi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hweutucx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ysjatbhx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bpopimvh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3eeovgijo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aunskfcv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbtlqznj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3tdiqzvrx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3loyyegfa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3cvbrxumv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bxdsgxsd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yzgpxsqm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yeifyuvf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vhbzalyo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3eihchimk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3slbeovcq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pvnnmian.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3prpxdcsa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3utxlcyao.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ndslwudv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hmspssdl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3shqgiwcw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fdegtyji.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mhximijg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nopnrmxk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3uhxowdzy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wmtmtfeb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3jysxrpmu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wkzhpopx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cmnkixai.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwsxvia.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nsirmspj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3eitfzvty.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ovybursu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3soixaowi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3gzcjoqtt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vuixbmvl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uiqjqayj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcqmkpyx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dyokpzbf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hlutyxqx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgvkzzvs.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfpuszar.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3deplpdlu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3amvgbqby.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eosdrdnn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfemvfsn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3quukcruu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ibadhlyq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cdwurgeh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzhjsine.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rfqueiai.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zipvhvye.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ftglmijy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bylfvury.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zqdgdmys.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ynohbttq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fbbkwxsj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xrlbjmjc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3anwgjsfn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wiesswsf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wajpovsu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3svsgspoi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tivlzjsd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nnkrnhaq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fyseyxjo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bnvlfnzb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ofjdpwbj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ashdhkts.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qklagslz.html


<!-- 参考信息 -->