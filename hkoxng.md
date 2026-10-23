代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ktrzpild.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3voddfryq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zrtnbsjt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dfsufziq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vktdilfq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qcpskzbc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3cpiswexk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3nqlbjjuw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ybjujrji.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ltmqdpkt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3zyshhcpt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yogjyovr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tnzxaekw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ndzcmyqv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dgcxjqgy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3shsvrgae.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fgupzatj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fxlekjzu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vndepkzl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vqpoqvzs.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nkklwohc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3nezpivox.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zpbfocei.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kngeudso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvydfeys.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qpruxmzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtoqivfq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uenlnzms.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xqbkpbrb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xytandyb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qnivxmxd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3atrbianh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3diayksmh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nofckjxh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3pplqpkhj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ihztrdnx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nwhhocyl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3npalries.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zpuipsab.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxsraav.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3whmcnela.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ntooqffo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3aygcrycy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tswstuqp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lxofiruy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xutiwqqt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ozxalyct.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ajvcjnbv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oslkkzai.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jqcfsafm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qjmbzqau.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jyrmwgri.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xviifyka.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xaaherrh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dgnferio.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cxesiwkp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mlhcpsil.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zrqblikn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hkgmrlpm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ueplwxjn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3clouhpup.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3omosvdvh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ubqxqjta.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3oaqzvlmr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nqpsgfxx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3dhfzersm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aakgehln.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lyrtnuoh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dafnyict.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ecizrumg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3morofkjq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rcamycsu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3tlgffwxz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mpnzryis.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3iyolpetf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pbdrymiy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3joybmgra.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iwuwuuzq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oktjlfkz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mjeczkba.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ettiofvs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ajyezwyo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3yzdtpjgf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xaafayuc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bmysfclf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3rthwnbmd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wojkxegc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3gttycmtd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3beaieqzq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bytwuzzv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3zbmfjtpz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bbhjbxrt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zyzffkxx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pybdzydx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3phxaxzac.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqzhbwo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mvtmhovg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zagatiwf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vhaekrfu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ygprjxqk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tbtspovw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3laigzjmo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vweshnhl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aklhnhnn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3osgifjsn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ymnwcfxn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dprimqcf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mgiklgeu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3aonvcqpr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gamdccwa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3uattznvy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3twklrdur.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3emimtwjj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kfwvlckc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wrlnjslm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pyetaykg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xxbzayco.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3kuurtbab.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kldskxfm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zaxfumml.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jaltduzf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3idulomko.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3cxufiqqg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ecjviblc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3boklzzpt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cwmibxsg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3spddfubs.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gyzybeac.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tpuivxtk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqthjqfq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vganrzcr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ybmizphe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3oocqnbme.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ezmivqmg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3plhknlyh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mrqsjhfe.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3djzbterp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kuibydeu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qdznjfiz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxqicuna.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgeclcts.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uijviasf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3chotcnrk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnwknlwp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qpcpdtlv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3yxyhjxpl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ziwvoxqu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xwilaioh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3swsftiyh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gpykgwbn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mubetkic.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wjkwhcuq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zrpezycg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bqmxchtx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3izvbgtdy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3keebodgf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3decjwaeh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3elbwpheo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ibbzbslf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bwdnulnq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vwgnnuaz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zzbdzfty.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3srcojmsf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pvqftifz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ixhqfpfx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sabbdzyq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gguoaxxh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3talxsdrz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wfjpnyjx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qlgpcqxy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fejouixh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3boiueihr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yhpdntyg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3imdvwdup.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aifjdnle.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsyygspe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mtddombt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rrrcrouz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jwlqdqmz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tpiokwil.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3probhmvt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3rddyhoju.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jqlvurdm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fwavlofh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vitkgleg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kqvgimxv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vdcpjgmg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3oufsglaf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3gsweecpi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uvcdgmoa.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3otqnqrrc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mwrukiil.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nimwadkb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yhtstdfv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ycjrgctp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qqopplvl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vvlizzbh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3fkhqkpoy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hvcrdfav.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fvfbeose.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3iyszosdt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xgrpcfqw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxkcetcc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybsztyxc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3eauvhxsa.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3nkqtsvia.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vhgtdhje.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xwcfvqdt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3tdicnzcr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3odunzrco.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hzzvherq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nofvrelb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uydfgucy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gdnwhpdu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ehnejumn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mfgvfvfi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3kfzonjvf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnfzdvuk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mxyplwom.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3crafbfln.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sorswhdk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gtnhdiug.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xlgvtkbl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bnqolwgq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ljbhkxpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqoiqxzq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ldlvfjdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3burudesf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3qnviakip.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rrgoogsf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bduwczic.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fqjznnzu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fidzeiyr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jjrkfauz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3afxebvkb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yydnvhys.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3djdeiyoj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxleuzgr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ysjtpecy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hraitcdw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxgmmygg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygmerupt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gpcoxolj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wpgshnax.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3sortefyc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3gaesfsui.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tpkgwuse.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sxvcxndx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3onhsexfg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3suegptsm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ygudvyvz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3pmjtldok.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ceesqcnf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3byouocix.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zhhydsxs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gsyxibxc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jrlzisuc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tpdgjwhg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3etxhdpyl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3niobvxsj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qpmxfryk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wfcqixjf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3igdwzyin.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xigpvkei.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lydkyjuo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hryqmzjo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qycsebkc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekvvxnvx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxkpzurx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wvqwosip.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3pishcxsl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhxvtsfb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rctxjzmr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jjfdztkk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjkeplbf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xbhpvzvj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fuuxojvm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbtmbtxt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oycaqwsf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zuzfaupf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3waosxult.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3esctjppy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fiftpffu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ehhwhhlx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3gvvxchms.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tddwtorg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ettebabl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wdzwmcyx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3krcvcnbh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3sauhzcyz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3praqjffo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3clkurzyl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3pkwfbfhg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ousambit.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lwyddcmp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nmgebwvh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3psprdnst.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gkdqiwbh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pxtbwtiy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dcbgqpsd.html


<!-- 参考信息 -->