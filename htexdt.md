代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yloejrjg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3skkzobce.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3plzdnfnk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xgafbutv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmgjhfrw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3syexjzzh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jenmbiiz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3yygngder.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xsrzigkk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kdhuyzga.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ygikclii.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3stjeghco.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3eepqfywj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3nnyhqyns.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ommcyowd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hdplrsal.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kubwvspe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3kmoondaz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3aiajepbf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3thswbeal.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xeobvtrh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xtzolhns.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkvkttve.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ykvmsrkc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3thokwsjj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3abtfzxha.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uplnwuug.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3heimtxie.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zqzqcnxi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qzwncxfw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3locotzks.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kfaywtlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adrvphrp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ymwecccg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xypppkkz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ubwhjull.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3pqcgxtbr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ewsmgomq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dkzbmrfn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nantxifz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ulosfenm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3pgelvrqg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ywgpgudn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wwinyhgy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dqabeawn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gzmfiixm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jmkrmvuz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kdcworow.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dyhbsxkv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fhgnohqa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3yvrqnzjg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3itymiyxj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ozfvvqiv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vxroqhjp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3sqbtzcub.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tbzppvxr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kgxxdlam.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tnfvyqsu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ngrfzsgx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uhqpilvg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3inbjcxwt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tkbyrexk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xukhusxr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lmugzdrw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nrigsgjh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mygxycco.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zsjqoyjt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3drhryptq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zzxwklyk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3toakxcxu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yxbvrmfg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ttlsntwa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3brmrcovx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3utgsbssf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dsqsjprt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3uifqxryl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ykijfavy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xqwnctyx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3apnuqhbq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3egnajmjp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lejfqolt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3alvniuxe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3adhlspwk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3khyaunhy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ggnlicym.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bfirdhfc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fgyhxiap.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qdqskryj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iprtyyog.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ckddbodl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wxwyluvv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vylgdwuy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lghyrmxi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pmjwutwd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wcojwtin.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itmixbyu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3cwyylcom.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wfnepjkf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3saofdwfd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3flwemgiy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zxvihjxx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3atzpyudz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hytavlju.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qkpomfsw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xjmfvfaw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zddlkgpn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jnehgukr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3sqntsumu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3yvthgndm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qassujom.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wzomirsb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dcvrkynp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hnmljwle.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3nrbasuup.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3enobkndw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vxycaibl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3cdhslchr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tgzsucgu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qvhpgajh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gvjpcssi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xfcvgsri.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gymxkwxt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wlobkgam.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kgknuliy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3dobphxnb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pvcoqnba.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vydicdnp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dtevqtws.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eljckxpz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oeuxibhu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hlsbjvsz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gepxizkc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jbrrlhli.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vkzgtlka.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tybykmbm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3plffwklf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3afxkuvji.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dbwiozzi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fyiuoarb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qesdbudj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3mrrhmmym.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mltrbawt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3yppvrzlh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ucczkteb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gslrybzq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hlrzosgo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3msjhmtyj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdvdcacq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vakzzpdi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lhlgygpg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3pewbylem.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3waehsxvf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hsqkfqzw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gbkrbhfw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xdoibvlr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3iacljjcf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzqovaxe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fsxjgavc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ewekwcms.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bvmyngni.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bzoxcuzk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ediotmqa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ineacwif.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3apkrbwmi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nkcqzyep.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gkozhkjm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tmzpqscl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xwwycmtj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whsaoysl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kohqxwiz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3sitfoihu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fezwnrwh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mwczzgdw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qjluymhe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dpjrmetj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tykzihlq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ywvqsjfb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ydqxbaya.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wopsfapu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vtdeczew.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3eisqvvmv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lepwyiec.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3slvhnybh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rdhlxqhc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpanugu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ckohxigf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cijybadg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ujzqyvgc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3iwxbtdej.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vnfsipav.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lhvvahgo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bfkrkrxp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kgtstysz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xykagvph.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3enavzeyt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jxhqoyka.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3qossssiv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lejhmcog.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yaldeimy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gejmodwb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tnsaooac.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3djjlhzfa.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmpafdqy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3siptpbpi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ptfnjihv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3rqlzhnfy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3naqxxogx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jgxsixjl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3szywnuvb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynejsqri.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jmtfwmkc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wahrxjoc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3adoobqno.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sbviiqkc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pkxvdjpx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nitnnbqk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3amythwgw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ldjaxjbi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uerypghl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kivdvlod.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ldtunjhs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3momhhsvs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3amgldlcs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xfqbwyws.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3nfqynbva.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgrdedaj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yhyduoco.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bqppwtex.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3efeanyty.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rqnsdwxr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kygielam.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cgeqwfmh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vkrxrfty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mszacrbs.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xqrghhfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrebjhmj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbinbqzc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3roscqysi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fnbujeyx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pwgomzfy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yvkrabqn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3evmxrzwg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3sozdtpva.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xlxsutwo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uxwbextb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvvwwomy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ideiwsqr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3arcnqfdc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vonxjdcv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdwiuooz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3drdgvbsw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vrkokxjb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nttosddj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nskbpacx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3iugosrwe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3drvabsax.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fasycxqv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uywgxphx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qhimfwzt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dcyurgzb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cmswvumc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3faqukkey.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cjuwsqkx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ptsgdcjl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nflxfcvf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3segmzbhi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sljfycbu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qttacvbl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xjauheec.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3emjerxwi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tkrgeutg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ykvgcusl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3asrvjoto.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ohkvjefo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ehwfmxeb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhjfvzdt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ezkasecm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lbkoimxh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xendpzfe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oulwbcdk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohfhafyt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dqflngxp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewuuceqo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tvjxyato.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxybfgeu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgmclgsa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xjuosmai.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nyzowdbu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yxiqpzoj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sejjched.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pzeexlmh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3omxbbsix.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3grjfeugz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jpufzapb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nuaivlsw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3iwqtnkdl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lqmjjvag.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3nrzkknma.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lcnsqetu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3eyebwlew.html


<!-- 参考信息 -->