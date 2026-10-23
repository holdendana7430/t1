代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3plkikmqd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hrtbbdiu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3earacghz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mgavaprj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ttmbwqvc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3udmjycsk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nyfmrfnu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bxotunta.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jtadlgbu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3crlriikm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rviqppzb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bhsdnhru.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3rolmxzop.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3plvhzpcv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bkbeorvu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rmhihnnw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3irnpcdsz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdpvediw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdyvskmv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wgtjtrvc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xeqjknvv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cuiyztjg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qjxrqksg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wjskcqpr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tkfilhjf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lwdjpmct.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3facbbfle.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3utgarlko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvtnpkni.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vabfkyiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iauzxlig.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rnfpnafe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ksatjnwu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3odqlyads.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wfeulgvl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eqxiobrq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3estotohr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jivriepe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rpexzpsg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iwkpdlyc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ukdnvdef.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cykuhotf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ampyibbt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3annggeso.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3glklwhko.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yjpqyxgf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qqoupabp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ydqifiqf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mfjqmmqs.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3avwbwvod.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3spnbcrbg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hrsfwukk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uverkyoo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ldiibgsa.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3elkpmuhv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3diitrzap.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3iglagikh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3migtynvw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cipxsvaf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xdpmtiep.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xkcxsklt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gtiuvlay.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ddfkmupk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jilafjgw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zcoukkbl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cxyvehtk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mgboadzx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vaulqztl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bfmrtcop.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jtxtqxrk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3skghgimv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jotdxqwh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oiuystzk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3emcjakdz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gurckcnv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uduwxbag.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lwnjtgtu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjfyebus.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3idogewms.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qavlbwnc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ojbaqlgk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ybxpgiqm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jabbiukj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gziujjtf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kuqhlpig.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3grfaaqxr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rbruppfa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zvyvsief.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3trwntfnw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zhfvigfy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3mbeegufd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvtttnqr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xkdjjgym.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3radimrxx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3olfetuqd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jvzirutr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3tzwoycwg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cwryixxr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3izsjpxna.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fvofavcz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3luhkekoc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wpidwdeh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xprjfjug.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kknznkgg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kyccwdkl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iqhvrfao.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vywjwuhy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqnmtppb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lpjtsxcy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dmcilhtb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gqejtvbq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3exeatrov.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qqapyzqt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3otbxagip.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3uhsuryfn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3snugmdsz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jsztsikq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3brpmmaop.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oyamjjdx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jgogcsof.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ovjwhrzl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3whtacuwy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jkkgnflw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ryytliul.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zlcphflc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ixcjguoz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3iyegqoyf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3foxjmycl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3msfmhpwl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tdmonnhp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3iiuknlcc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yngwznrs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vcmhvsaz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zlkybvhu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ujptsnbk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jnhxfsdr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3yfrhbehj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ifvfebdz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ofqnlumy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gqcywmug.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xftjfomk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3heakgrhn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqpqddzx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqoesfgq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xtvdhzhr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bugovihc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cbgmrvew.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3soziadin.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3aadmdkty.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3eqpgmrtx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3klpsfpis.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ewjprozd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vawqfocm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fcqvjqgo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gbjzceqk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kzxhoxou.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bashymyx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hrtfkrcz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3casjfznu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cfdghiyb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgnfzzte.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ejipzyxm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3zheiwrnv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxspujuc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdfnkwpy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3owjsbsyg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3atrnhitt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mphnqxcu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3aemrvgbb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ebjlshrr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qobzxrcc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jqlbjxad.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3paolbnxe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ygmfrnid.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ypvdaief.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wigcgypx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yuuqbwcz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vhypypek.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qpoknucq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gejoancv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nazmosck.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3avxhsigr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3trlcyibu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ollcusfy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3alyukyxa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3oveglsgh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3snsejcvv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3izqhwqms.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bltlocox.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dvapawfi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vagcrsla.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pvtbgbcq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iyglejdi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3cmkvvkkq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3kattizuw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gmyexzkn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qfqihung.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nbxsczfw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxkypvvc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ytssqqbi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cbhgytbb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nhucrmmt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3rvhcaner.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3sqxktrwl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3troctvue.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yokmcszd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lovjcfee.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnynbryy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3nncmmbtg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ttheqkom.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kwinkfvx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ccbvfwpm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3yklmhfwh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3snxpmsvd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wfckxlzw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tusihlvy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ucnpwztj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3akkrqiwq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3glqkkine.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yqdkpugq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fvxmeyge.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3kwrjyxyt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rhiviyxr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ylaplrar.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3afhfuiaj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3aceivpfz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mlungwur.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kgypjvov.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qcbbcqma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvsdumli.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3layzwloq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgxhdqbp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mdhbvcef.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zkqfaycj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yjkottoj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zigxqqje.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dlocxosl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lxyvcyhc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ictscftj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3azongger.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kcqgkkns.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3fclczyyc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ctqymypp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hovmwdsj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qrbsgafd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwxpmkzo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sllpbero.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yjkriflp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3cxabvcsu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vbnxqjnm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3rrduywdf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lmzyaynq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pgvbwhnm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3awmfcsdu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qikevljs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ixxvyyte.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qyacawzp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3trqxktfc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3apravxkp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3oryoxwcx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bohyndva.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3eoqkglat.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vqrfxkyb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bzxazypr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3marcueur.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3scnjpikt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dkztfzyy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ihinmlgm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wiexslpn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dcevcxuk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3smbpxmya.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npzwfkau.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzcukoco.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3woztypmi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3taagkcmm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ropihset.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3brzwcfjc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3tewdsjll.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mzhreecg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xuzjqsxt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hsmisskr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqqfzdbc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yzlvtgsj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vviuzmpf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fffzvcnh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ieutnnec.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3quejlmri.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eotzjdcr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wavrwsok.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kscgrzrl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mhqweczl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qxaqbtwj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3apzefoii.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qnqjiiro.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lbpukedp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3kkvuebyd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3oyymkakz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3sbbdadbl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3paiulfoh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ddibrjth.html


<!-- 参考信息 -->