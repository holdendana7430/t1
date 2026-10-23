代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tosvzyck.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3myvrgkay.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fdlpwyfl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fewtnewd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xdmzjcyv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rxoldsea.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fdtvcgex.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zzrkkvyz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lgcmtlnl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ezugafyu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3otlbzkqr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3dnutwpmq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wppzcuge.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmudaxj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3yptcwley.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvafcvhd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3iqkpzcqu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkrtgnp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uqkocaob.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yclkylyj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zpubyuar.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mrcpppaq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jzrbjdar.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uvpaecqb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cbxvktcp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ahsolugs.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vqbzkmhn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fvzqpgdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbglqpzw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3skfbjglg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmbhqcoc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eophzzoi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kiuhtcuz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fwdtbdiv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iahxhsko.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yzcsinil.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jppyeifw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fgdtivfg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tsawuura.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3otlmkavr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3oojgmpeg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ksbiuigv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3naacljrc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zzpdfqcl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mtpmaxzg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hagqhivx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3lxylorez.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yiztaoze.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vwpyflsa.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ogtpopyi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3elafzqvq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fsenkakl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lcqghclt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qaxlcnpt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ivfrknea.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3eucdpthv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3atmlwhws.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3olrcqwjv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3tpmtcbke.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tzlrklfi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3livxvpgb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vxhbvyzv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3utvgshtf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rwscyaad.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vkqgwmtx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qpwujffi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vlojuvcr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3uieuqmxd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qcitveav.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3pavqrkuh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hftuamnz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fsqvghko.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hxzdhhre.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3cshxfufu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fhqxwbcl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xhsddfcx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pvfjrzet.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ysmijtjg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3djliwpop.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xgptvyas.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ifqlayuk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qgonuqtm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kfoklabu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ybdqzqvx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3axjuudht.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3btrtpgdj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3azjndkzb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zopwsgbi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3cicvktis.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3duvmoymt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3papmxreb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3etbilujh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3encyvolp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3aktnqjrx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3siigelxt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3heypyebt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3slwjesxz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3naoqnyiw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uicydnie.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3azpqclzu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3nrqdvioi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3syvguerd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3spjtkbaa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3uflrglck.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttwuzfeg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hmqhnavi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ehbqbdtq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3govxlpen.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lpsvzzzs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3pkdwntxa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ppwgqneq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fjzpzpdp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lkgeirsw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3njwzsydy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hajknbdo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mkomulph.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3thqomhyp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rufntovt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fredfrjo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sjjgzbbz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3amlhaoxv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3uhkbqaaq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ezecjwag.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ogtgbvrt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rmzakjox.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3chserofn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pnxdrhzz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qmkbtpmm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mxqsfprm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ohojptbi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xglxovvu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tyhwnwsq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rfppjrov.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vhwzrqky.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gfkpgewt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3heqzfajf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3comlxesi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fbnntryy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uhkswivg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mcomfgbw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3umqeybzo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jyupnaea.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ccngvpol.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ulptjawr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcrnatof.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hstmcrgm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mgwluasa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zixczqzu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gkssmnrm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pkcvjwhi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3robizyfz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zqpxbpbe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nnmbdbwa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ycoajnvh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rzxdwyps.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hgxoqcvu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mjalxccr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jxlfhfqx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3sflixguo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3aoamvott.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3iqfbassp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mnhcjyhq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3diautvot.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rtsfbgip.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3byzqqkxh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3sdmkdngc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gezvvxtn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vhovlkfi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3qeqhxbye.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3otmnmvww.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3oqvovprg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wriqtyhr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3kvfihgdv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3czfpijao.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bmgplkez.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vmheaemp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fbfqzupa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3fcpuqhqj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nggbofna.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygguhiur.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rrpnomku.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yrmuedaa.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vjmlizuf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qhqnczyl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xabsrzxs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ndxlezng.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ewuzpbxv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xibsabee.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yydivars.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ulnhfzgc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cifvxvqo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pegcfryx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ijqdeugc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3azpceahq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3uynrmhzx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vygoiizv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wiolejlv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mxfgykry.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zlsqvcss.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zxqxyzvy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3npakdbrg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3laiydyyg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mdyakaja.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bwxegiwg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rfgnihph.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3syytvqya.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwzqkecq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgmmseex.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zqddsihd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3psbamuff.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lspzysvg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tcwdosoy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3uxkmhvbg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xqkdtyuq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mxqiqbhp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wpivghow.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wlxyhotv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xccqcurp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tyoiurqo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jjhmftls.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wdbfqjbq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vxrzrwjq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kxfeepno.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ilyzxxti.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pypdxdrk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3obymckag.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hwsotetr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pkmdhpyd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3plsgojxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxbdxodc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3knnywjpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxwremsn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uibirhkl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3irkipyto.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rlbmfazt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3jcmdfmhf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rnaiigmb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3grossinl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gggpwpaf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jizndpch.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qktbakjj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xcecadha.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3agrckett.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kcxpzewa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vdyhowzy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjlyzzvy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tnwdkuhp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tawnxhck.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3agtaohji.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ywuizmtv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qfzfnksr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3czsxlugk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zcjksqeb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3etulckzk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lhmzzuot.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3kdlwqtym.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3wyogdbhc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ujykupvl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wssckjii.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vitulkpl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tejffcrc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wideynzr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fdzzzfry.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vyfhrsbl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fwxubcin.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hxuyrccs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qlqibbkv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3evnhwewx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aqddolhd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uwhvepny.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ytfukwil.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aclhstew.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzgyarue.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fbkjzgqu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xjabvjhd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nhyplfbc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzmxhvhv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ujuxgmoz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3miyewuev.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3abftkyet.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqaemexn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kzptjwzu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ejfrfakk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aqzbxabd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rznllikf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqttxhhd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3htacutvl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3yqzlpjqv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pystpfcl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lffsiwlr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tebsbqzx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jonqpebq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3mqtzspwf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3tqkgjbsj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qmezeldx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3kttlycmc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pnesnfpw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgjqmzkd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3odxuopxe.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ldmkkiuw.html


<!-- 参考信息 -->