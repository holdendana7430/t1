代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2oeionpyv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2bpedcxpw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uhbuuywp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yixhsmvw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2whhtxkdh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wymvanyq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pfxvxcph.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bbppcbaf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yarozbvj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ijbtseqq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ybzpiibx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2fjzmhrne.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rjgeieat.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pveobsna.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lxrdlbme.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tlbxbyqw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bgevpyrl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hrbphczh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qcmzsgaq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2flgkfkaf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2pouapwgu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vtnojbqs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yeudykly.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2plrvurvj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gvkdiagm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sghqagpr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lszeaezj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xiitxayr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whfghyrn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2amvqpcva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vakbltya.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2etvklkms.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pdmvcmsu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vpzmpxst.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zyrouenx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wzasbrrv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ogpvmbyo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nzlddjws.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2bpfmsdti.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ooouhexe.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ichqeyuv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2iwzmulpa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qdhfaaeg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2elugcjfw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zbzqhnph.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2exnenxmk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zzatvcjr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mykrmwpc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2unmvibhm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2punbfjud.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2bvxkyhhn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pzzaqcsc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zmhnmjlm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pulyacmw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hfoqxeed.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jcgrswci.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qzbvyibs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fzkakpic.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xvacbdnf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jvcdeqbd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2flexzfhx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2zftvxlji.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gikucqap.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yejcqlwm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fcsxdzqk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zgclodti.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2amqebuco.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vrgnnvcd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qrbmplan.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2lleeruqu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hdkebzba.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2bnbqybvu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2atsoddqs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2eqzhozbz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nvtonsfz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qdlpylmq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nsiiunny.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zneslezp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yiawboji.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zgnzlmok.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2grdlmqpd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cudmeudi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ibbxbgft.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fxoougty.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tquewsfk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ihimnxpz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ugipxupt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2brunywdg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yzuhufeh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2plurylag.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2raupzwpv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2avxqgmcr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ivcxgtih.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bgwvdirv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2etcmxaax.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lsofpdzp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gctwtvxs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lvkmebbc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mzitumbd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fckomcas.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rhwycuzp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xinxejpj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hokxmsuc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qspkjzfx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tgvnnksa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jglvkbmf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fiqwzgyt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2aozykzob.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2uvnllrmb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2uwdctpsj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fetkhboq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bbceftda.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zgtpakpn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rlejryaz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vlblekzr.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jmxbblfz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2exyylcqz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zqajjozb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xrldvcsa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2axtsqjyx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ueyjutpy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2viwhnkmw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wwujysdz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdwiudkd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jfmtbgxl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xvccfbgz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bcuyfniu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lrajbrtn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dqicczgy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jysmgbqf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2eohydpws.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jxocydjv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2nvsnutcx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vrtqnzxn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ubqfdhfc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hputdaqb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tdctnljr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tsqxqvom.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kpikgnhv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2drwkqpbk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2beqynibs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvlvipcl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ramepekh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjumhhpi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruytjiry.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cykcqabw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2etjeffhx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ufyytdwi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2naimpdzy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2yuqkwecd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2iywkldiw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tbnufevc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yazgaxfv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qosmjlhi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rrscyyii.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qwqgmfel.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2knoycmzk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jdxbfrad.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jdvnumxx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xpqnpeaa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxlockn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2avvlpvfq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wbqisiyy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2coohtdvq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qjdodbpg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2cwfthwbl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qvyqzmxu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rjljdpjz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2appddtbj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tyrcdxiq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sveuzoot.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vxxaehhz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jyqzalqw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rkalowtn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gjiggtzv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2prpjoffy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bgnujzzr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ppwvrxji.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nahzxnmr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cggrjiup.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgatnwvb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hvfhdkni.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hncyzkqq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2yqfnxidk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2akqfhlvn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2pkxojjyt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2cauoqfsn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gecoajzr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqmtbum.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pewyaiqq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yiqurhiy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2xzkbajnx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2knkdjosx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2owcjxxvg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2kwhcwnqn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tsyhignw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2twrennzc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zloknyhw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2iuypdqyq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nwsuklvk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zawbmmml.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rrfibcoe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gvbniqsu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ebodefrw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2kfqzppds.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2fpnsswpz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2emefdyqy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epjloryu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzzrwmdf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hdxhauun.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezzxrfaj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2onyefcjd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mitvdwjt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fivxnrzo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qbllbxsk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2frfnkrti.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2raugtmxh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kuautafi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2paakmfxq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2phynolmy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2emhqgiic.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pepjptkl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kceeeblj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bazkgatx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ovjaxydp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aauqdmhv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ausksugv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ywxqzvms.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2drbtkzfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdougjgs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2bkooqefm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2purrncko.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ccfxlxru.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2tfvsianm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hlhyzpki.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nppddeci.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ukpeeazr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vmtdngpe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2httpazzp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwxprmat.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2duluhext.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcoyxeic.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zbrtrqhb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtrshzvy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ssktrvox.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ncndkjih.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nkgwivpg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2otekmovk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yhaqrlfg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fpqezulr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2egueiynf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rjgpnnjg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2typmqtgm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gqafiqzz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xizeovsy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2spvcwwqv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cyupbxuv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2acsjlsjo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ozsdgrdb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxxxbfds.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ewbdxaxg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qvrhlvpi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rcbbsibu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zwawrrao.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2epqteblm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gvutzmxa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mbotcddp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pwoiyjvq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2eiffuhsg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wdzcnxtd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zxuwcsqp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkbqelrw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftcdromd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2weolbofa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2kvxefpfo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugeteqjy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lecxhrnf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xraskera.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbddfang.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2flauwmmt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewkhvmmt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltrrpuec.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2thvgykal.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uujnirqf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xetemoby.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nxfvvzft.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2krklpzho.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qxokhgpg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aymzbfmo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fyknmlgg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lxgydcfm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qafbbbcr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2oxstuszt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2uyrkdpai.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2edzrakgd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2alzrfbpo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2uotsqrrf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gwxjijmn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2khbtpgkg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bdwajhrr.html


<!-- 参考信息 -->