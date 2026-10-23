代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmvlrptr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3isikhngv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dlmbdjyu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tcdgimfa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3znfdpedr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mtvxidlo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uejytjgn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mdvnieiy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tptzfenq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3zkakfhab.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vvfcsliy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hhncehwe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zckwicws.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ududolfo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hcniocsi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vijwfuga.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kbkrzhyk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uztgezcy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3krissnhx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rfcryapp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bdzeabss.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yelqiuid.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zgrqsnzi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iiqylciz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfiqlvg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zthxwbaq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3utljgofb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3drvqnxjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlrpoydt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tamclgat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftqwwhfc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wndrnxhe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vqutzzuu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3hxoenewg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ahnymkin.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gyfbqsag.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3oecqeion.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wtsumjkc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vzpaotlt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gaxoyvlr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dsjzepqp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mvqntcha.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tcehzmgq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cvkfhpxe.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cfqdlasw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3phyxsitc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3stqqxvhy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oushtlti.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ldagwpht.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jqcqsopb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3uuqwvtch.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wafqaewc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vowtrihl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tzkedgxj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gkdettlq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3efortlbe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lncnzutf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3skbweefx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3oosejziv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bwzgoqro.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oqfbubfz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3tywtbeiz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rjcsrwbs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nplkjtfa.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yyaehjkg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qmhdbyus.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3etziqiud.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fhdovswj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ncniiqry.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fadaztxv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gpqjbqkm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eyekycpd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ckgkkhoo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qqlpyque.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3zdkacrxd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3efjpgudd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3aijnlonu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hoalbgxn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ezxhsscb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3memmifyf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qgirhudu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fpzygigg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rezalegl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dclnapnk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3srgtweiw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vuymeern.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zrproqqb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ogzmrxlw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qddojtjr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mkbyfthr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3kgzczrxw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rwglapjk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qznbwtkr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zxmcpwjs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3csojwfim.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3aupfubhb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wirkzzoq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ahtytrhh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gzshecsb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3liyhsvtd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jroztdea.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mhawcyya.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uoyjdkso.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wvlbgccj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ziegyfzh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aekwmgbo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fcdgermh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3seredmsv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ykylldfx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mqdiwywh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pdjteizf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nrhgpfqo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3teouwjsn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gwnzdzga.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3lvoaztyx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kfwiynwo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3azrfljxw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qephjpsv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qsmdrdgu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ymohmxtv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3olvujojn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3miihxtbo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vqireqrm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fngjawfr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ebrkzsbm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ewadhshx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ppkfgwig.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3spmcpfsz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rhbeewqy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3thxvyzlw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ifvihylg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3byqwbjmw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vcmfnvbr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mywghwra.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3scjbemdu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3lpcubyfy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3whfyalqd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3flubvnto.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vcsesyvn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ijetgajr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3yqttkgfb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vrqwuuse.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bpcziwsv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mbugrjwd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtofzpkc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tbsqfaor.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xifmaynw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bausqevx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3fqstphry.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hxarxpwv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3sfxnpyan.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3nstbkuyc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bfslqsvt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xvrbydlj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cgnfzorj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3doccqomt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rdcmpsrd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3keqnlaqs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3uwwspqab.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gvyohshn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngpcxcpu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cbbuqysg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ozxpxyjn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cotkifzz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kobztbfi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3aamliwgr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xbuyxblj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3tuvhcgym.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3isfnpucz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3myvorewp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pmruxgod.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3legfnzly.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3hmaginsw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ljihccsi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3dunzyjov.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wodjpgcl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rymxhtvz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vqsrjhbp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vshjdwtf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3savtygwu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgrysaxy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pupbsioy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lzeruvst.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3nstbtinn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tzubmoxp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3cjbffvtk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nymcfosw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mbqbrkne.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ikouurta.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wzpnmszh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ekkvlvtq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lpyexlxc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sxuyjxmp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ntxclley.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bvbxyzxr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3omuigird.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nkswjxvh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhphblv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cochlhuc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uvkxjokc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nscazbhp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gehtxihs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dcwvxxgl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rnszxpak.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gtqitxdv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tqzgamzb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3srnkgwpi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejhitzsf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lgdtktdk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ewzzhpoj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kxkfkaib.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vtosdcag.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zadynzib.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iswcgwfg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rgezrtck.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xsbescql.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zfozhhlq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3arfnvpkc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xmavpfux.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ylbioxug.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3cygloaeh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ubvuopps.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jrsehsxf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3elfxtjxb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3umcoojqh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3majarvly.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xluburmd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hnqxhbqw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nkuvxkbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcloxmeo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3kcuvswyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpupanmn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3iceybhfw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gldckevv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rhalmame.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tkzslyci.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fytbfgyw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rxcjhhgo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wqqvwewu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjxqxdct.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wajjjimr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zcmrcrhg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3nuiwadaw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3auimfbji.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3svawoxul.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekrhypsy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xoryffvu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xstrkymd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kdtzynjj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fsrvmkqx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3euatqmbp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lohnbmog.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tlnoljkz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qqmrkjja.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3abwbzrrv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3yofbvgwx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zffyaqsd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jlfnrdnq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zuyhszdc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cuoterjb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pwlpxlfd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3oldbbwkv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eoiilkso.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ntkcpoml.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3grmtvfuy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yaqzisfv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3udnbekkq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rpedjatd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sqqgojuy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zzasyvff.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdtjbcdc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzwzctsd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dkmovizv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3llwzexig.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3lwgqensa.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vudwpvkg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kuxrbbbw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbjwnhkb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cadqjawd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hudyypgm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yfvuwcnx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwwwxnnm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ljlwvfcc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yruqjtcw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjtpgvln.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ylbilluk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3pwltfcyn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ynpprkal.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ufawmbgu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bsqebluj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nvgjcakw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mtvbawij.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3aelbotaf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vdoxnlam.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3gjwofpin.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3kfekrdbk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3tzipgmxg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ibzkhghd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qbpnrlyx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bvrxroka.html


<!-- 参考信息 -->