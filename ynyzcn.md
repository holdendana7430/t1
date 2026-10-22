代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2izedpnzu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lhxebrmh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wthyvqtm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gqsovxvm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wfpwauuy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tzlmyjbv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2psieuyky.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fycmzdgs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2laxlqsrc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fhwabvuj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2thflpnjp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mlgzjnlj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qafdhluj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxildwnt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ktbavhwl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bprgrtrf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2satwiiix.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yiizccmv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vaqtqecd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bfverjaw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kvmnfeuj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gsplqhhn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mkuejtol.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vemunmqs.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2grfomnfx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rfrtmddm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2micarosg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2boxjlowp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aznkdnny.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wmdxtfhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrmxkbdl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fatbqzsb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wyfphzyq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cayussds.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bokppdbr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pbxggbwg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vihqoqsv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kvzxyieo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rdzrxqdj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xqtimdbz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2utbpqpji.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sqhlghqc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tumzuohr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fiordmzn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rrjqshqo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mjganvin.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ilikygdo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cbyclkgy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pagjoqyr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cwihnwpi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2kpclpfsf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2frjocpwr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zdglafod.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zxrrhvmx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gzvvgaqq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wxxmdueb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rlnxfxhu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lyotyapi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2bbtgqseo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cneuhrbj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gtacdfzt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2wtxpcfbc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bccompma.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wvvdzppu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rkrfmpju.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ejblrbbs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kvsidflt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2kdwclfrp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eayjmbbq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tbdrsdjp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mhmfimex.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gjnbodyx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vdtwiyoo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jpgcnbdj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yvavcguz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mecisgmt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2xhuodvql.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkfenvxe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xmkxeota.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yrfvbrxr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ofvcqrne.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ghaahtug.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ktaxults.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2alclfyvx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bppcahqq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qlmngrrb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2kqenkeki.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfdfkzfm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cmlbadil.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kscbaado.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rjaktjjg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zkkfxjyr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hpgiynxw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vvlktede.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pkyckhcz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zlfcpchk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wkmmwkob.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ewgnwixq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dtziipek.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2klvjcotf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2nentniid.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dybzpplj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jupqoczb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kxylyfgs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjbcgwek.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2aylkgvxh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cyiezvio.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mxgtxffc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ypvqhlaf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ltlexrer.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vqnvghzz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yjuylrlb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dpeemlfs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2psivberf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hystwthu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kjxbgbbb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wegeplfd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sqljytbb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gyfdgkfh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wzelxurb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2waeizzcj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gyolpwth.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pnmofgaj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yagmzgsp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yfkvtmih.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rrewvuzh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uxcajucm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2grjgidym.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hfbdjqqk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2omciukyj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ubebwisn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ixdeoqzd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2svhbkomu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wkmlztuj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dtjcdsfu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2trgcgbxe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tcqnqklq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hiesdkhx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jpxlrobf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2kzhmorij.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mroyxjll.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rrrzmloy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rksthgal.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iefghfem.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ilabhbem.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aibixgjt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pgcorwok.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2idferbfu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kkllyuia.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2wnpllkea.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2uokwxhde.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2aumvxrvi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hiwcyaqe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ribtfycc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2csvmxjei.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2iwmoqmqq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2whmxngnx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rzqoeiim.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ysgkedxe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2madefkkl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zxuxidtj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2sfohvjae.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xoiylvau.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2peddgccc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bzsfkrab.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2rqkcijch.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jzkpwnsd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wjfkemro.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rfolegks.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cedsfaic.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ljflurth.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ooyxskyv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nfyqkijo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hqbaflxy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ajajndnf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2embgugum.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gvntxjrh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2humskely.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2agvjovpb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2owsrpraj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xiwuybco.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2abkfweda.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qcaevabh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lmpfcwvy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vmksgxcd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ynvojgmp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yoiuygaz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zuvlrjcq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tivvnuqq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hftwleea.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zpkojuka.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vrfcdcyw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ngdrfhfv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cyyvwetb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2lredxjpw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ihsjqlgp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ppwtesrl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dazkvfmu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2clqgchir.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bcxknnkn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2iytnfpsm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xzfvychq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ejqxhfgm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2oopsregp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rehevbbi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pftotrfo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qmtnpvsd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2imhkgmzu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2shqbuarg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2gqouaxvy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ijilxfoe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uqxquxkg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wnpwkcbp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zdjtiskd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tuazwmiy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mdsndppt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dvjdvnfb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zkgwzsyq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jhrvjejk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zazxsgnb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2falyzgok.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2yltszizu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oqaalaxm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tmhbvyec.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gishcwuh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cslawfnu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2yefljypb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aztlpqcf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xixcmxtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwdxuvla.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uduwyowv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylducwgi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnoiylip.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2mqwavjob.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gxlkgihd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fqzsvlib.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bivcjfeo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ykvjndlq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ikmwtycj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zozfhcxs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sropkfry.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkctjlut.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bzknjcrj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwskhodg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fikgadkl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hokuxxtx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rhqvxzzd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kmpwnpza.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xuorxgsm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktlfvemk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vzqciwod.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qbibawzr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sfopepxp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qhmdlxjx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2azvrwxcb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ciztydtl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wneqdemc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nxwdzihr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xjkospaq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2omfhoaur.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cqudhvof.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vkgcslyt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nqpbgugf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vpkpabsj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kinrkhqs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2feaeiyus.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xhlrjqqw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dimnytjm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2mdgzygjq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qyelclaf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hlgijixe.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2amdgmeqx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sgenrpfb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pjrdlgpo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lvyplhoz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjogpeoi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjtymtgx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rydiigbn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqfdqbsz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iihhfgdn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wghmogrj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfudtcin.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eusbryjt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cpbmmkfr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wscsbzol.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aevfbaai.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vjorbvrs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2azvaqjef.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kfwtxfaw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yedzgytu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ffexkotn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cpfxshul.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2paompqwh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kgthuamu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hjxopwvk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2njzvrxps.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2pmzetsgq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2bubunlpj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bxkrvoag.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wjhnfysl.html


<!-- 参考信息 -->