代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iworyqsv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3oabcgezk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ikbldllj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xgwuwwhw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3whxyjijc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3xgdaapmn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jlagmeww.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bzlghuox.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3glpgeqhy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qnyzkioq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tmbnytgm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wkcsfutg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ejfnpcor.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mtitvjzr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3kavqlnjc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ycixezhz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tazjbipv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3slovsxhs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3qhrwxzfr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lgurbvca.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3czmeaolz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxopawpq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kltpdapl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3llwqmhai.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3huwoajri.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eaabfytb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qqmkgbev.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bmtlhasb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xpjxcvae.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wwaavhqx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mytnybas.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3squwbguc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eepiflpn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rvghaulx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3liqtrjbt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qwwlycsl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gwxmouxk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rrzneuwn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dcqafpfz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3igpmpfxt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zhzwtoee.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3cylwdyyn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gadvhrlc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3avywvmlh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zaetpiem.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tinzgkpi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dzuyiavp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qxikymjb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tbufdjmc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gvdaidzq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kyjpcimm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3prfejbfm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cpedxper.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kjjprfag.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3umbfdrnh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ltlfmbpj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nxtoksgf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mkegcahr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3efshtxss.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3esgebptd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ddghtvba.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pjskyonq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zqwygaho.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3oenommcl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3elqfyxqv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3prowrozp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rmxgicvm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bnbsolkg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3agspioux.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hospnpkh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nknowfnh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3pnvzxglk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hixzphmv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ntnmafmk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uovsfjlz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pslzkspg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xtvstnxy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vtsxmasc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3nmchbzkc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nzeplfgh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3yprqwfbp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvhinrzc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lldghmlp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3berpguiy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eyymivis.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jycozbiv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgmwtggi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ociwqtxy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qunxddrb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nsevvczp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gspzvczj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3egxcscaw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pxzacwhm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jqfkeevo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xjbrobfj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3idtdsmly.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rmhzqvhc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3cxfefzkg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3arqgezjk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zjzsfzzb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qgkznuwj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gmqxvsxv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zvqsqwyj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zcczybsx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vadwfall.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jlguhjqj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qvaukzim.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3aikukalc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wesoqlyp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3uflasqaf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ijemlcdi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3spvrbnzf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3todgrill.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3mtnjbgqg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xxfbydmp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nlvsivan.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3deqgcxgs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zayimunb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dwqsihtl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ylquqzfn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zugeidfd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3aakpuowi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mtnamykn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3geoniyfk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3soidzyvz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zavrfzyt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3btgdfgyl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gozpxbik.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pdfuhwwx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lrrmnsyc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pxtcgovw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fmkrpwkk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mqtfupyf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vxqhupwa.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vusulhzn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ysmdzrtb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3avcapoka.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tcgrilsx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxknqhpv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xdwsxbmu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3yzafywve.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jzaymezl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jqecgrgy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xgbniwzz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ezyweniz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vifvokan.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fmqxwsbu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kudyvsbr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ocherxys.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nqxivvca.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dlsojzxf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tlfxzgeq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ifqelvwq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dcdzjvnx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tlcpcjmr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xqssrmvr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3yizcjvps.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ktnfygqc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3gjbxwgwb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3swdvhykr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3khzcuoew.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bvpiglgr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xhaazlhv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3cwhfqahs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zwbfpmfw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kypjosft.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xhxqabcs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3eawraiwi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3lxcewrbl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgunfabp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vkzxmvlw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uoalmmvl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3otygufnt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rbqbjucw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mzspphvg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jrzyojkp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qftrenkk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yrifdboy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hmdfevpm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vcdqusoy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kfbpfahc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3yegermlw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blrhvasv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvrvmosc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmiuoacg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3neegrvte.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ozgsiahv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3htcuvmit.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dfqhrwdc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jkovxemo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kakwozzi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lessitaq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ggheevsd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ymqwauvd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kxymsqhh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pzaxjjzz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yorgjoyg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qdabqlqc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qithwzch.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3quodgqbh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lsibomoo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vavgtlok.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3lsrqgror.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mpmylexg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3bgjmeztu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dkwgcqir.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dqgayywx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3nbdhtsqw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tgxrjjtr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3sdonqltq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqnvblta.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhflcskc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qtguxtnt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3vmqyajvj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ctiybizz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tntvklyv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3crmfdeag.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bxepdjee.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zhxcandn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3imstomct.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3veiwgzey.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fxgjrukg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lbouakue.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vqmtnnbg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ymeullfj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nmwmbkng.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iveltsiq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3whsmqmkw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ykkxpphq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ayjkgepm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kipuosia.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rbctrrzs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xrcwgmkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcbpahrc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gxpapehm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jucwtlgr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kzoaavqx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hccqojmd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tpulyvex.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gxclgdbo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lcyrnero.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wmugvarm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jbrvqabj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xisewptz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hyxvkoeo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hssclgxm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qbjhhgxz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3cughxibt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gbtkjapd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3humearzz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mgeanbfa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gnybftvp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3mfsziorh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhterppa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3poefjiea.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3phcssunr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3drvwnbzt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3msqebedt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3chkbxhqw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3itykbijn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3xuigepep.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3inzpsokd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cfqubwhm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3emhrlrtm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zpxzyjou.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rwegtwbe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vekxkdud.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3enhvkkcd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mjbgwosx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hsgedxvs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3pragtvre.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fjqswkql.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hgfetnfq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mgdauuub.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vpntojul.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dyhtzzys.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avlucovn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dufffard.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ibfmwvfa.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3danrfevh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txrvbimz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3njotaaye.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rhodpoqs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kwboptdr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lghnghqu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwatcjkw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sekxtjpk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltfjkaux.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oicexdvv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nxtzoiso.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3onqypmkk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rcdixbod.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xuzojzkw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kbviqqiz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kshhukip.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxbzbmza.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3offguesz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xtxqsvdz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jthrvceu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3sgwbqumz.html


<!-- 参考信息 -->