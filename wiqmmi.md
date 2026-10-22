代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2onryexya.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2eqqrwdik.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bxhlenvs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hgcqasjw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbdjhntk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ahrrnmdw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ahjbazzj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gpczqhjq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ottfebkx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2spiybhuc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2uslajprv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2fkyqhbwx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rdzyypwf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epqbqixd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2juzmpeaw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oxrbzxnb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2djhnjftx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ypriwwbg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gqyxxlaq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yvcvwyyd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2coyljumy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmzepfio.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yybrztlh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2seqkyabw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ybvxmtxl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dvtoyejs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qzxttbtz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lpkgffyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwkeddzm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zfsjkkdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afptzgzx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2orrltrkt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zhgynwiw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dzfwpikx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2giyylhof.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zgbgqvpc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fcwegchv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zaitybmb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jelsydce.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zbkkykyn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ngmzssiy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2royfynpd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zowxloeo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kwcdancz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2grgrysix.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2omzcepfm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mlqofnst.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mrsbabcn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ldfebgtm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rpnopjyh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2quaqpoxo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2btiteeqj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ebcfymoo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nicahnfz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jlwwcqmc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kvnechfn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2oqdngqwu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gplibnhd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2fxfbgner.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pyutzdab.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2nxakchzr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ninelesz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2esmhsqud.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hphgasvx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zoarrfqw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qigfghje.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ikqtjmgq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ndynpcwp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hblnduqr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2sjnymzxq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dspwjtry.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lqggnwid.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pyeqkfxo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tquyinhv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gmxgdfzl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2guoiigwr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vxbzutsy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zgttesbv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2omgaybal.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kksozoqx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aztzeuxx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zogddchh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfpblfam.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fbjocwgb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rxetgjsp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nyrknyyb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xosyqitu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mwepvnxr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hjdpvmbd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2roodebsu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bfktzpbq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bmynzmno.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2faugkczv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zfnceitm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2eniqkysd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tlztnexi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2altxqlvf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2phcwzhqm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sfhgazhl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2woknosde.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vijskqpp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rjiqddgb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2durfpyqz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bwqyyqsa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rmkobgrp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2sbtmkooj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ladnxfqm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lbgrbzaa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tqbnspwr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rjlmclcu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jdzyszwl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jgekbsbm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ebldhbtu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pygrksyl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kgeqoaat.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bxfnrezv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dwyuezay.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kwkaysuj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vtkxadwq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yxibgkvb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hcwwmuqy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2utuabtet.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gavixfpk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2elkuwkrl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eubxqkwa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vkpthnsn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ktjforfp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pcpxreud.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tzqxiacq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lwlngdax.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2obndihux.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hhfktpxv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kdocrswt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sxxzytdl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oqdqawkz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2boebucbx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zpjauuxl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zwejprlh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wrnwgyra.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2xcbezape.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2egyhkzqf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2khvhxhew.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptxhjrrf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftnmqryb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xyxjhxae.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2coazebon.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dlnidteb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnrvqbdm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2pwpdhqbt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zgprfhzk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kumobxov.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2romaysgm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wttwjigm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vpowaqhp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2exlojheq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lczlwyiv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cbkxzuoa.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2sxbalwnb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ysdznavs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ryhiidxv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpertukc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2eqtnkoob.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2swubgken.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bcrhgkra.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wzxdmnuc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2amegrdwx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pucccrzc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ocntjete.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2yavgktae.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wwvvfbfl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2iquzicnm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2amxxypca.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wxnilphh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2iyuxfmlt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hdriuapi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ksozxwle.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2syiunyme.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uxkynfnx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wjxkjbgw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lsqsdgbh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2etzmsamy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qognrlpz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uzifysjo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2twzauctx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ngyvourj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jrbepmog.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vczsavgk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2slwoxrmx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2npdbtcmr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wkquihhr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tbemmniy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2duuwdumj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kimvsidd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vnevxijg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jgytyxqi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ksotwguc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wnnkogjj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tymvwdnl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tgjwqzpk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yweszmno.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ikxlfuzo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qtktmfvm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2idzyoilv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ymtgeckh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2cdotmfqd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xnyefosr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2exxrkqnm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fnfcvbnt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyhiiiyd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2smtzsmde.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrohzhcs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ffhvgkle.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2eortuskj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hlartrwd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2huzeicir.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xwhkhgux.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bjccyrbj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mogabfbf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hnsoquuj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dltuqary.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wrvylrnx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2uemegage.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ksbefvij.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2llazpnhk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bvkhduxh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tywyzvcg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2uzuddnoa.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qtxqkqza.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pkhdlmkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bycufhfm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xsnpjnlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdqjjvft.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvbfwzck.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2abhxlnes.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dgytjbwn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2sxcoeggm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2udgylbrr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2efivdxur.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2tvqmyvdh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhguahlx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lacziznf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2idwlbvvf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kxflbgkv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhckywvx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvxczfyk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwxvqwuj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kjdveqiq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ldyweqrz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wiuvboxm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zdpjnikw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2cyjahawj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yjowkgug.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2erskuxsy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pnjshkvw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gjrwjuwv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xsjllrzc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qkhbskge.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dnlecuvz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gytamcrb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2izncolji.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ofclrmme.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vdfcezzk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wimrrsmz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jqjggwgm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2jmtuonwz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nmrozjxp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2uqmtqkcr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ajrkkcsj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2enjgkxnc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bbgbteku.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xdowjyka.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjzutqdv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ayxjznah.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hbeseaur.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ceeclyzo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2awfxlgsm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtseekjm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2aaadreey.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2coebdygi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jtzizmbo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yekcixdu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyqrzbmm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2asyddctp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2speipdfq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqvvvfke.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mfziotft.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ermcqlxl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gxftkksv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ledokins.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xyxiwjpz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mbjulbni.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ugfcltzz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2xdyzmszr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ldwnwpjz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zudstkor.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lxkutocj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hurlujsv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gtumdgbe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qtruwgdm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2suodfifk.html


<!-- 参考信息 -->