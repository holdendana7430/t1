代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ltxtmlys.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gzvupysc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2yniavrpo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jpmlzfqi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2accrhpfu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zdkpnfoh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ekpvnrgu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wpwmvqzx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kfitbwcf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qfrazmaj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yomdgatt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tjfkfaos.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ggqiovbn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dudegqhn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ifpzxiby.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2leurmrcj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wyqovxju.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vyolaqzk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rudlaisf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtmvhrtm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sdvlwmod.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jiwpqiwm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jerskycp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2morrxakb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qprejhsi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cwnfbpnw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cgsbisgy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2diswaijn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbnarrjg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2crispfhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvrkcgvs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rqffimrc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2opgioesq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gfzflkvi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fyqzgsvn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2getplakx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2badnxsbx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pojinwwk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2pqhzdoav.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ixgvpjff.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fjigxkfn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pzgajrog.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zozmmguh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yrlauzwz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zukajbao.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oymydvtx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2obtewomp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qmjdllcm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mvcdatxm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2inxkmtre.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wrqlbcmj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qjvxlfrw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2awnnvbar.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cvwrdkme.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hfsvftrk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hvyhpaxs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2wdaprvsx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmwkjag.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2eznbzcbb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ucpkisxa.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2icsyagrm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ocjqmrvd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qtafyzyh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yycmsyqa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ornrkcfj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pmyxafft.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xjmiufxm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qwrkmhsc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pwolhmqc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fxvutyzo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qyjxrvuk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2erchgyph.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lkzefemr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lpblxykb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2abubngct.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yscjqlne.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wksswfcl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2moeefion.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jojjhrlb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xquuzwwt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sklklgru.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2knsczihv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ydmcahlm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pmdubkgi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dkyjxwsn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ehsyjlue.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2mgpyxdzd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dlvzdbmb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jvroxxmo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ltintjtl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jjjykdpq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ltdjjdmr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ymouavsh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rtenvdyv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xrfejewr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2uqerqaio.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zqxzzxnq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cugienzb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2osbgkzfw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2avfjcuuq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2gdnepyup.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jqsfmgfd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ruosialp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2stjbxooa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bkoraxml.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2uidtpild.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vfzbrarc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wctalgwf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lzvgrwmt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2axvtlvdm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zjmvgvgv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wfoiabmy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2psdswvxn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hqfwkede.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bqnmzedz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ewzhiydp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2icgfupkt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ftupvzob.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2urfpryda.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ztjxndwz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zbdninxz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xkjpnhux.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vwigvxgc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vcrdwbpv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ccvlmhpp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sjznjunf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2chlhslid.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2squyvjnz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jequemoh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bsqqqywo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2szkijilu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lvyfgmvg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mxrcxqty.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wbeowtqu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ceyvwcwi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2glkpitcx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kvwhhnll.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zdfuubdw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2suvlihfg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2izahijmw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2dgeekuww.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaggfrpc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zwwvinmy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fhdtuoql.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ehabwnqj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hiwrdrqp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2aledghjv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hwqzvita.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wczvnyju.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kbwznald.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bjlpscgw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2dnsyovcs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ijxmzjgh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dzqiwrnj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2endfirbx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2emhsgiiz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2btnrggid.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yixzuxou.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmzadou.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2eqzehjhk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztcbtght.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jtqdqcdh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ixitrghh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2yrqgsnql.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bsbzzwzr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrwhyfor.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xhqfnjqx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2cgpiriqi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zkeljkld.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cczisqji.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ejjblpcg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tvnurysv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ajyntygc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lyartvxr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zkbnitte.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yzdgdgtt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ancajwob.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2luqoljbx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vytwgdhg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ppbeatqg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kjpsruwn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wgpmmzau.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ljijnail.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2bstrzsjd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zwgqnpne.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2plqlazsc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2eiihqbmr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ogbkexxw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cjfmdwbc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2klcysokx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ykchkfsa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2iufhqpty.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ylzytptq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xvidzkeg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ngvgchjn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vlqostln.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bxsvrnuj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2whbfmtlm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vvaypuhv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2lajmbcai.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ixzswuzq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mujczwuu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2sjtowjvy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2epnppdyr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xeicjtcw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzhogxxg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzwsflrx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hefkppio.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbyknqdl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2gfjupkng.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ugcoioyf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wjptlbum.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2hqrdaoqj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fhukxpay.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ymmxwitj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bjsuevfn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hfflumcm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xuezhifk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2savvjxtw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vvxbafrd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2srnwwxhe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qoihplpg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oasaqzeb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2awovpiso.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aggjvqwd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jbhjluup.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2slrbqphm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2stjteume.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kxorfrfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnhvuxeh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jiksisba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwoenctn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2aeyvnfxb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2eobcgznm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bzgmkraq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2basahtqg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dvjjiowo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wlxrbrwl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2abqadpxi.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klcgbgta.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zrlkabym.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nhqqyhwo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2okioeytq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2aqhgowch.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ldzodyuu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kliejwxk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ozwtwsup.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2udbhwscq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2sovbgtun.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mbpuywhc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2sqblsiiu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fjfqjoca.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2eznlwsmj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fncjdbep.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zbybzapv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2apzoqakx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2uaypjndx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2elhoihei.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cgcyfdvo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dtbbfohx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2oyyosqkj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mijjpspa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mrgfyrmy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xlznxmzj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uepufrsy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ysdwzyzt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2khxdlgyl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2edvopjvn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ffmlrwvo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fwbrtgft.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2txlbjijy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlnrmils.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbvxykxh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jzncwtdd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nhcyzdvx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2laisspet.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcivrxkf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gljuwxvk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vpzhpsvz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fhcawpyd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydvptqzj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sqsmwqty.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ntqtbnuj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2klsqnnfh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atnhykkx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fhkjozhq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2quijgetj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2muajolfu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zytzlyle.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hwbqkicq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cocrvnig.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2duhkpfuk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqkvhwn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pxtieeuu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wxwbrjol.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2dqkmtdkt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zpztwigg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2olklfoni.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2unimnemd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fxcpbolz.html


<!-- 参考信息 -->