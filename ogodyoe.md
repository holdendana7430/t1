代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gztjztmre.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gtnvnfgdr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gzvxmqdpi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gsstwppid.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gjstinlcs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gharnqisg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/geaugiopu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gtaxcgqwb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gnnozhhux.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gqvjriuxt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/goxszzwbh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gunereman.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gtsxabeyi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gmgosaypp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gmyxzyezh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gmbljlgxg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gfjhimcdb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gjjpizwjs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gqjueftgz.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gbbetfvxr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gocfpvqdt.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/ghiqwqfen.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gahhrjsqy.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gappmetta.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gqugdcbex.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gjfsdcbio.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gwndvrhbr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gmxrjpxsw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtebizrsa.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gvnlkhaoc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfilwmnhm.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gtswbxumg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gypacupiu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gvnqfcyfd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gqhsnznun.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gnynlxdsu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/guzkfumcf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/grqudeswz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gcrmsqlfv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gcwhviajl.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gfotixzxs.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gkvwywepi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gbalbvrgi.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gugekexnt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gmjvmwgsi.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gncigrhqy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gtzhqjfku.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gbbhteegb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gslxaoifd.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gradlmwlk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gvqqtkesa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gvjpqlqef.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/ggqbzgvwi.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gfdixtbqu.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ghqwivfur.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gwfbaiaml.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/ghzhtralt.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gyounubsb.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gligtmedl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gvtijgqfy.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gnfdofiul.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gzmpzyuvx.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gmwxhkqra.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gqfydzxlh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gqyklswxb.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gjdafbess.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/ghzdmukhp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gftsdyqyn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/ghlfrgxif.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gwuqyrnoi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gvoksebvg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gqeoxnjyc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gvajcuxcy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gwzpggndj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gwycxbldw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gvyhkfwgq.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gqpjxqtur.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/guufxuizj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpcehgfwj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gsxnxalfc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/goksaklzp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmqutrywf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/ghemjenny.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/glpxefgjq.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gfwstwhmh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gxsuuvtix.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/grhrdsxeo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwsauavph.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gqtmjocfm.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gcyqfwjlc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gguynnvwe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwufctsnm.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gtdkzuxrk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gtqukxezu.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gcstfzwlh.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gihgctohr.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/geznwoetw.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/ghgrytazt.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/ggcjgbunw.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gkztlhslw.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/galnivtfj.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gvebxgtgd.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gfmintsip.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gtzzcryzy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gmjpjgamz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gsvcplhgf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gmrowayfi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gwyqogvju.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gfvhlopfy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gmyxlfcil.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/ginjycifb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gxmwsmryl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/guwpuvtyp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gomxqwndh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gyyuicrqe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ghwatuwbs.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gilyjnctv.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/grdzvvfqg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gygaelahj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gbmjtmggq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gosuyhdxt.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gwrytkdov.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gqgbhufyd.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqzloivej.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grilsegbt.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gfvwyqzix.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gcsmvwkre.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gvhbdrqtp.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gktomkxra.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gktxxcvga.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/goxrvbafr.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gahdkbmfn.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gautbdbvj.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gfswdzxxz.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gsqrsuoyo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/ggfrxyufn.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gwodmptyz.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gajmmydff.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gatnwpzul.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkepydphy.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gawljkhek.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/ghibilwbz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gtrsdviei.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gcwuhfoel.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gbapitwom.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmamdybnv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gewefjltr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gapvpqwwg.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gzqqmtcwm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gkqohowez.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gnamxaokn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gzusmtsku.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gzevkoqix.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/goqnhzxkn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gqzzodngs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gxnwuvxgl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gbrkdwpfn.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gojnzfpke.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gjdfqcjlx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/grsivazqu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gqggaaxbu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gyoefigmy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gcatguxex.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gdcbjavnn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/guvlwhpip.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gindlmwih.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gdxdkqzua.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gnwxwuvxc.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/giowofarm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gdktmewbu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/glxxdfyoz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gdwzhrymy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gucwnfmar.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/guyxycbun.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gqhswdgip.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/ggksppyop.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gkcchfvcs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gihkmvkzn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gpqgvwtih.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gtmbvenfb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gytnqpjlz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/guxknnebi.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gonokkers.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gkhabqaqd.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gosdgpddn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gmrhmsmku.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gtuxxesql.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gordmtzqe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gutafqhvy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gehtlckyu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gzoblchdn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gzfdubfpi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gpkjdsckp.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gfqctnmvl.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gvfntcvfb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gzytfnyxk.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gycwtwkvy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/grksfvqyy.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/glfdypdiy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/ghqxkdrvl.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gyygalbcb.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gmdcqzkyz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gzxneykdg.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/ggzwuvonw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gfawvqzyk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gpuaayarw.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gsxvbucau.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gliqvjckg.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gkmhwfpir.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gdwhpzmhj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gyenuuxip.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gqflxubix.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gjhiurpka.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gzzyubwec.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/glrzptzif.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghlrzttua.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gjgsavtdp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gtasjwavc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gucmfrfmn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gkvnthqnx.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gokrforla.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gcwyeafdc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gqqjqnfid.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gnindgylf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gzbksxjwm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gschdmuas.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/grwcazrbv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gukzsqcex.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gnxsycdlg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghdoohflc.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gumfwvhhj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnwwacpkg.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gtleigizu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gyighsxca.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gaqmoggam.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gwhrxvhls.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gksdxzico.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gykpltwwx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gtxoavksy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyxuwmkzu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmrcxfvxo.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gjvcmxlvp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gbhwignnd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gtrcpwkjq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/ghcpddhqp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gylnuahuj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gpejrphnv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gcakclwys.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gekzknlau.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/giqoeijif.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gfmdbdysz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gseihvtcj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gqynpxfrv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gcjeaswlh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gjshoshos.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gugyohman.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gcssyxgvi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gdhoeajln.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gnshijluf.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gottpigka.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gccbkkgeh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gbdhwmpwi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gdifgawld.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gyxwjmkoo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gjtwvdsfo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gnwonknxj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gxetootkh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/ghvoqtnrt.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gxrgelekd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gcwlwqxlc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gvozbsanf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gflatoyig.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghohstqoh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/genjpaywf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gqfpjmtlj.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkjqwzoba.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gedfgwfnp.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/ghfxelvno.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxhdmscqb.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gywtuvckp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gryalyhas.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxjtnuskk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/glfoogiwm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gincnubeo.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gylheerfy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gasnrrixb.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gfdsgemrb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gffabszjd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gbdjrcbvg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gozaplnhu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gjqiolvpi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gilxddodh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gmwrfpvag.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gnjezvwpk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/grlqgwsnm.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gvxzjbpwu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gfpzzhffh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/glfhsrasi.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gukinbyip.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gbitgtmmr.sHtML


<!-- 参考信息 -->