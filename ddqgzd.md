代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ekflnlwh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rxtpymda.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uwqrliwx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3sncuxurv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxpysmo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3baorrqwv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qyrhfque.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gqfxhzqy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ejocmpox.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3uknkbdvj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3scqcemtv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gjohhomx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zumygbeb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qathrkrh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pnavxgho.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cjpasfyc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yrhgaopb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vmilxiqw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ufbbwwyj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zxvuyloh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qwlzjcnc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gtytmsyg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ssbhoxto.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dvlvmexy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xfllvxsw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dziogomw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nofxotdj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ptovodal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jipcqlpk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ikdotsga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3liymlztd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rynobkif.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rhclhual.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fwzdzubp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bjwninsq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cnmtafvi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3smmfxppi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sunrhryo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3dlqewxry.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3matmqbtm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3peprhoud.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qltlkzik.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3rxmixoze.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cuwmjgte.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mjixzmoa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkrvtni.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3asyyyqwy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wxsyhnvz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xobyedbk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hzmfugue.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3klcehrkg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gheaefob.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xacbccpz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3osvpvmko.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtkzpgj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lxmbwhwe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3onblgpft.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rotyivum.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3tbmiihmd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mlldmtfk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3tfnzfmna.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nvsofmyp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3baathysd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mbdvkosu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mqlsthzp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dljdviai.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jvpyhqrk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vxdkdxdy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rdannequ.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qmewarrf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dzekkelx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kprqdfwv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3phxszgox.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gkqyrjxf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zsmxmmdl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bsbxwfdh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xfohlgrl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvjyaplp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rfflfoiz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eyzbomno.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uizinkwy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ekqszvha.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ftyloclr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3webtvjwb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tuahtfra.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wafdfbpm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zeemrokp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vjaongfd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zcirpkla.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ipnwmvxn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fskphfuq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tzzmywpa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pyqcjxht.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xbjcaxdh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qhsoysfw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lwzupklm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jdbpbmfb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wvvdlovn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3owzrqnne.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3thjgvftc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lgdnmjkj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3znxshquk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbacahl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jugznuua.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hniztoyd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3eeplwfgp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wniabwps.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dqjscvls.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tnynrzgm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pfqrbbvv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nmjqjigf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3howhdoqb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3erlhqroe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3casyywvd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xmvzfcyr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3swhmzfek.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aubpmqex.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wxffsdyj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iadcmejn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wxdizlsd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3uhzzozcw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdhsvyns.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kserhzqe.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mlpsygtm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3szfzuxgz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bkxtgxsv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ubpqueka.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rwxzngiv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fxijtdbj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nffjmgdu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gymykybm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wgsvcfns.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bwkwjpjv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ithbzsmw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ercjlgcu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ffujfzqt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3srrjotpn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3maqifbyh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3yghqdgyy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iyodvtze.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dbykkvst.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hfawtnyv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wzsgkozz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3msdcxupf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrffefwn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rbhqxtrm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lfhyxico.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xanfcpxt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cfeqiijo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qszklwur.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tmtrhioa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tirrkxwb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jswhaygg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qxlhgkxm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mmuobkdk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ioagkkkh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nhzubjma.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3cobpwlyx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3fuepmcsd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qdxhhbvj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjemhkyw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ubtxeqdj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jsypqwcx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cjmdjcib.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vwgdlhsu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbtvauna.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kzgqhjkq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3agfwvqwr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zwakklel.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tgmettnx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vpkvlpiq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lzxsadbn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vnrpjklq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3lsfbtiiq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3bqrnfznu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3zvyztyej.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dfsdvuzp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vvtjjyrv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwrvfbze.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gvamypwj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3woelowaz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3liryaetr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3eqgupfiq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3jwaruriu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wncnxoob.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hikbniiq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pzjhnwgk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xfpsqrkg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hqjlyeof.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tqiiajur.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gvssrrlo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qplcxgox.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fxapgnhv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zvhwfnaz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gobmwoqk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xkparryx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xmbinhxx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3iuamqtpp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dewkrdok.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gbbslrww.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3dsdqsxgu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3nnmksrlr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ntmnhmda.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qjmxelva.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rfkxpvym.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3cfwlelmi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3uckkfrha.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zofeawlc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ropdoise.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qtqnqmrk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcgkhlfz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3womnafcp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jeprimlp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fnjvtcic.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hmlthdtr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ooozxezm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3modtnezq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kjldixko.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fvpxsozg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yvgmklna.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wdnjizra.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgomfnez.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eatfsadz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3krnuunkp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3asbigmjx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kwjzenwd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3delysema.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wfdeaqdc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3glqruoyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfbxejdw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3csnirlzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrkqbkhb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzisqvvr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3evhnlyvb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lvuhtncg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vswwxooz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ymobrhgu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3msfpegth.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jjwftiaj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xststgaa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eyujicwk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dstbydzi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jjrnwung.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwzvzinp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yblcxzcq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndergfvo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xftmgpre.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ntuxviik.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3flgclhjq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wymknkwm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ayjtleuc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zpgdbzgk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jupnobsm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ktojjmpq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fzkxofzi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gctcftnj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mtvqvrjv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3mtsofeog.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nzgdosnb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3lspyqeti.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rkrkxvvj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wqhjqpqw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mdndzffi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3btvcabmc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3pxyilnut.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ngurxzuc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3neepkpzw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yoxqvuvi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kswuwvbb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hjafdzah.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yitjviag.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtxuangi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3endywiyq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vcrunegx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vffvbhgz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lvfrwkqv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irkedntr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qagybvgq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stldmzpb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yhcyzudq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbuxnzxp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eidtkocj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3izlaowom.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdwpbtwp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3utbdqxai.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aygfcedf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mfcirolz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ubbswszo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xysgovsy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hedljuuw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mlixxapl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ygzovjpa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gxwnuvlr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ycvbnflc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3gxddxmoe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ufozblqx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dabxivpe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dmtztrrw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rlxronpj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ahvoztla.html


<!-- 参考信息 -->