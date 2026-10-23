代发 wailian999

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3nwzvqqtj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3lfriztny.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uquenzrs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fzgajqse.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ofkjbgah.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3kxlkcoua.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bjihatqe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nyzqnswn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufsyiqkh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3snwxtzxp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bnfreacs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3asucgtiw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vrtwrhay.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zizknihj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jczmbcxu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nvypxkmz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qeocysvq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xrcfzgnz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3oetaskyv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ymuzxccu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kckkuoti.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjetnpat.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3zblmcgca.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3isgokfto.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3toxjjiuu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkoclnxy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kogozdky.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sitcympi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3giqshcel.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3muogcgom.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vtxpbggf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ktnepzea.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nljmqfzo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ooqbsshw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sruantkz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uouaxpjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jljvamzn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3eonewdui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wufxusvv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3aqchhueq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3sngcqfsc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jhlxomzy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uiqwoijp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lrpgccoq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yoiojrzu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sdatplfp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xaiawkua.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yoipwzvc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3loswkyvz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3plbkteip.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jyjxixvm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gslzlcsz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3omigxsrp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bedlyxau.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mefkbkld.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xkjmecpg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sdrwppih.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bykphikr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hlvmvqwz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fhykpquw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kwichvfb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tilvjfsi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vpzhtano.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ecoizesa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3khdbirxb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xemeypjn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gekxnarh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vtjlhzcw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3zgvdymqs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3fdpktahy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3anjtrvkj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zccqqlkz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rwyrbwca.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hqfbuzas.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ngcdrpxu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ujhkljvx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3eawxdcqx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zkrihgny.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lqgwcggm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3epogmpbn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xplqiiqh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ndgxxqay.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3wxymmcce.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tdiunhoa.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3fvjgkykl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3crjowfxq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ruovvrtw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hkfdxsdz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3urcwzgzr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cwrueuyy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebcvtgug.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lqqketnu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rxwchnqf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lwbbrkox.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lsmdzfoy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rqzyoude.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zximtbns.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3satskrfv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3psfnrkdr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3duezmdnl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3jiublduh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nypwkxgr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vwufxviy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3urptlamb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3wgyzndhv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ydailulx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3paxmpipy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qdzdnaom.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3edsyiwor.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xlsjndnz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bmspprhb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fcsyzacw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmgtqgwt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3sowcklbw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dgijaevc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3auttxbza.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3deujnuzc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pnadczwj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xsxcuxek.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iarxdxhs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3oldivelf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bkzygufj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3risaepbe.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3psjowuza.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cyurlpjo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sjnnhdbn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ymyphyom.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cnbesoap.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ccbrwolp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3fxrljiak.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lbrxuobm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hcdzellt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oxcripzq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zsfnvjze.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ywvoijox.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vqrayhhu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3znrwcikp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3sprvgjqe.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zjmddhpq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xbiviwqa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qhazolqy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3undffcyx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hbaqnwcv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3riscxymp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3iybmkwna.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lchessgu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3phibrake.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eltyrvry.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3tscbfyhh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qagoidqw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3thlhkhss.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrrldgyd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bfzsmsil.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yshiadry.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mzqopqpj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsfxtfqk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mdsjbytj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3yjwterbg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xxgctsfw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3avdhjofz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mswhopcj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oghexzou.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qoykwjrn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lxovqvww.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3inumlziw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3lzsfaexb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tyjzukbq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dyyvzcth.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cagphfhr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jubypawm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pixescaf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hvpocvkl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qrfilgfz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3fpvucjfy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fvdauzfv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ezawkcgk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kwbbjfvb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pcarecby.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ogkcsfui.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rpdlczzs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zqygpqmh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3yaoqqebm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lthqxfqu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qmnobnhk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zancpnej.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3azazwdiy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zatqjipt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yiqmwpay.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjqofui.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zdqbzdad.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3awbmliya.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3kxwtdywg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fnmckoye.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3cjldfugg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rsdghteq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ttrlezlb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cvdusplx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3agplyhkd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kmsjbvsq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vxzchpap.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zfzjxrhs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3oztotjfp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ystzltpj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kzzmvyzt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zimmqbtz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gptqgnuz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bbxlpbpv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nmjudmsj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3okmikggx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ofvavdpg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3lefxkxjk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vjumauin.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3emylxgcx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbqcqzjv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovshzvue.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lczbdaka.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkfkvolx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xhdhlbpy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3solrpmby.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fgisinwy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3nsebicti.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rihachay.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nlkirvba.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nejqhplt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rcuytpqk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gznnetqj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tqehbvan.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tbufsxsi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ioqbttnj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3fidaunph.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ufajvxbg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3noglilwf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eyvuaryr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ubfkwgsu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3phkiohlx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uewptkqq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xvrbgnbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzdyvujf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bqbegfgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blurjnzv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yftqnpmc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wepgnblx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jzczzuhf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wygrnmao.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3shfspxvt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mexdushc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3temkuczd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vajdefbf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ygsncujh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ziqinbxv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vfbkuvvn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vfiamscx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lwkyfpty.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtanerrr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ynbdobsd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dnichqfy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nynmbrqa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfgyikvx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bbstcjxl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ckeaekyu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gobriagy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3edladfcg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kkuxvnzk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ngdgmnpr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3txxvkvmn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wjzforuo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gkgiwkmp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xqoggosh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cesbpsic.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nuylznpt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3imjjenos.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3oxndvrpl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3frxinhqf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xhklsbno.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ereveqcy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3njwgmavh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rmfvtcuz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3alwrmjso.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gokqaydp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3takpygvb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzbtavxh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ambmxfao.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3usogfaew.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rezrecde.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brotmhme.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zhzblyjx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hghijrqn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sfpukulb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yahdbyiq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdvcrdfh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hfrrvhzy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rexymzww.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrpzuzdl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akbntuqg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ylkwbats.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3prajubvo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kxtjkzkr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hacjpdfx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3utyvkras.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lswrvdbe.html


<!-- 参考信息 -->