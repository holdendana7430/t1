代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nyjjladh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vjnofyez.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dwcgkzmq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jomiwmng.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3irgtnuql.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vsjcqyke.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ugjzbcgq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ktoizrpb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lpqalydd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3buntaepu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3uzqbehpy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3grcnusom.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3gaceceik.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkccolyy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycrnyiaw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjulprru.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3khefudjf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cflcwcfk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmzwskr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbsfiybm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3enbldxoz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gyhjkuld.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3akjjcskh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3egzncqiz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3urabyyeg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uchvzxvv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3guiammqo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qywyahxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jexzhlkn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3epnpduer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvlzdonu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iwjivyeo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3agdxdmzj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3rfblbyux.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qmcubklv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pvkrdkay.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cffdubng.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ydaxbnfj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bvtcecee.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xrobvdsf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3tfiorqmu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jrlzocpw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3rmmtslqd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3khlknqoj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xqyvzofk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3awjjlgge.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3okcxurdy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xwkjmkxi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xindttmp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zdqmsfdq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ffsgdvpb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jbdhbsid.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tiayuuab.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3htegiell.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3foycdtjr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zcrcdhyh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qqheockv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cxgyvrrg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gkqjyssu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hzifkcge.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lkczzbeq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ouedlprg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3guubwvir.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3diumlhoe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xxxohfqq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ifffbvbj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yrpqizcf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mhhdsngk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pnbfaeaz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qrdohfgk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pcdvkxrf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gicavnvt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kueoxvqo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kmwpgldc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kwwrapsv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wqjwaxlx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3sqdqnqmk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3enwljvky.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yzxtvqpd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nmulyckd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3brxbafxw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vqdpdnql.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lozzdhen.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ysqfuypp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xpxivoij.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xnumagan.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yxspwygs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ossghbjr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ixsjjlwl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3yribbfgy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jxjnmzxt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3gtykhrak.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3znvoqsqy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zdyiacvh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3npugkivs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zdzqnwtd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3poeleski.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pyookgem.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tuatqooy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ulogeeki.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zqhswxrn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gzjbrrft.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3shytlzmz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3uggffaag.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eyvkwyqr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jzeunvvz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3akzgmjzj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3egbxlvva.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gbknhhdq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3azdlklnr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ezajvktn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cwxfecmm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rwkkllls.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ccgmipkv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3euguqxkq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cagqzxxk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bfrgybkr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uuzabtvn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fwqrlwrn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nvnhykld.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ohecbeuf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kjlzfqmn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kvzoxhit.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3btqcobqq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zxfikbqw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zwtxrpwz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wwhmavid.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pfewwedz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3efgmdcll.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3inwswtok.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ogugauqw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yivvsccm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3iguqxmxf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3inxfkfne.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gjbvrwwb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3okktanje.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3cwgedlwh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nmgahpcd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dsqypksa.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3pmapzmhp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3kmdtgybz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bstmspwh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rsspoirk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtdwiouj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3djlmmvvw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3liyswdqe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3idxrgygi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lgbvxuuk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3khwrhtqi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gqkezodi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3irrjfpjc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vfmxghjh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qrxpbccl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzyqxpc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3drsxejww.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hxfxujvw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nsvwwodq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wliydhgd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ojoosqla.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zsztstsx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezpvpfxw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wxachhja.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rqpiayqe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjusfqsq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3dyhxgvht.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sktaufin.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fkeegxgk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3llsxvkuv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3dvfwlpmp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xrahkfxd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hgnaawau.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3htpsqyyl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vjsmujkt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xnxxqqxf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zvxvofnv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3svhigoov.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fknabgmq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jhtwjjuh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3stpahjgj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pxlnypgd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zmrjtect.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fxjcdfkd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3onttrpin.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dsebutry.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3uwuhrorg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ssdcwqrl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gjevlkgr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kkkriorf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xdzvihxd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ndqtwfuq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ydzrgdop.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fugkyxxp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mmopxqvy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qyuahykx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pqmdklir.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fkbxltfj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bawfezlh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qsepdepg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pzxlnchk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lboqhspw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qbnvizqg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cxfscqtr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ifbdvuuo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ikbytuvg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rzwfazdq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhaaswsw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jaetpzpu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xeukakfx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpslnklj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dngondkh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utkdcuza.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xnqlmawe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xowzusfd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wusltyiw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3akkfxufu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vqysfsoz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dvtiivjc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ycfyghce.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vwdboyzt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uhdwhula.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bggqkkti.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mipqrohl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3asfvlcet.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lmxrrtlt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tjcylpvv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dkcttjfm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ucpiajpp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qbslocay.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hffkvpzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnsmwfsy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3lzabxqnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfueirud.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3htnauwbe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kpjuflzu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hdkthpsv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3orjpgjuj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wyanwtgl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ceevplsh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3radwfyqz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxkumhrx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3utzwihvp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jxxqcrip.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zgdzregx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqspztpn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcluuuqn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3koptnrzh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pyieswcq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wggnknbw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ftlaxway.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3zqeiwqom.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qwrzegng.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dgahwctj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iohjvlcn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fslpphgq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uncnfzhd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3evqghtjn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3wvekgtch.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pjzqonok.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ajeyrlcz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cdcxwkua.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3whwkrpne.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3niptodec.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qvuqoaru.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tjrlzlnz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hkpzysjt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3orjqyjlb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3loqqepyf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yhtvlipy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3whtwldfb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nwrbvurk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dqhfysqt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awlfnbgl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hyuyzldz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kayvwpns.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rtiqqvjs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mllkpacm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djruxgmg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfzwltpw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pkdxxpgy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kkjumjll.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3icgfakvg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfkqrgle.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wzyfplqs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzikjski.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbbxughz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3crmshmsw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3llujkzug.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jwqfkkps.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bjmzjvhp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jtgoqqbq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xecumqbi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fbdcgfhq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3upvpvxnm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mdvmpbsr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bfkkmybv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bfemeaiv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3skpsrdgp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdhvdccl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kcqcjjki.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lothbrom.html


<!-- 参考信息 -->