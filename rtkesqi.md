代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gnqnxcyxv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gjwcwnqkh.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gfzjvhghq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gavpwntcw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gtpdylidg.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/glaublqif.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/glcmhznuy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gxdokgfwb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gkiofotkq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gicyleddt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gbqigxekz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gnqddjjjd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/goajoazrl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gmnxhmbcc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/glfxypwrr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/guircbyle.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gtqupodep.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gwltwupaf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gxhrjjjyu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/glfurwxyl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gdbutjqpz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gtpdwgdhp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gjjufppwf.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gnwzzbuke.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gfmvfsrxj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxspqusdp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/giicsonke.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gnrhvvnkm.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gygifsnnt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gmgjjigig.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gkrujgwqu.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/grswizajw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqcpssgaq.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gvbyfaryf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geyzqskvn.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpzjxlwng.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gfqclejhw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gcsavofst.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfnsjumnb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/glpedpghf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gcahqyuwr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtxpggcto.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gvplolxjh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gghnzeugs.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gfxuuklua.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/geulrescv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gwwnkclxn.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/ghjrpbsvw.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gbrdprdeu.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gqdkhbuyu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/guyowiacz.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gipubmuov.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gbifbephd.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gntptzqfe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gzikkdlqy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gltyrkksb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/goqnhsvez.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gdghzgmxd.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gaafnjoia.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gskqbuazu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gssxfpjcf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gysnhzufq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gtnrgtelq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/ghidjgign.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gkflxkypw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/giabgihjn.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gwbhfpypc.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gkpejqzhl.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/geazjnbog.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gvugpebqo.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gxkkslvdi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gwqxuqqfz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gzbsrofnd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/guhshfjxw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gngcvzilx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/geeftkitx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/geokpdgxx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/guogqdaje.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gonavckic.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gmwnpexfp.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/grmgkabuk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gyvlnuavl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gsvbiewxt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gkbtcfjtc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gnibummxy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdmpkxutq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gbuwnlhpi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gtmxyshex.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/godllkktz.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/guhqsoegw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/guwjkhfby.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gufinzagd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gcjsvdbyy.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gwwxxytfp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gdhxnlkoh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gbovesogb.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gsdeqqlyi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gyqvdsfrv.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gbslawibk.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gizdtcefi.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gdebpkgfg.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/guhraeqdo.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gsyfdgucy.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gebuzcbse.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gsgkjbvbx.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gsbdwpnqs.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/geguvlaku.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/ggtzmxnnw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gzoebiemw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gnwtrbade.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/ggciooexo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/guwyxrfis.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gfpziezcw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/ghgeujjrq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gyfcauksk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gkhyspydw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/guvgmxuac.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gskmvlvol.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gkrviztnj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gypttzezq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ginlomune.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gbqebgptm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmwkjyhl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ghsxcttyj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gibrdmnne.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/ghdwycdry.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/glmcbwwil.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/ghhalzijy.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/glcrdaftl.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gohqcpfhw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gfiuscohx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gngrmrpuo.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gcswodzbi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gkknvvwbg.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gkrnkrwte.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/guqvsehyj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/godbpwgtf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gasihrrrj.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gtpbaogud.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gkbytddoh.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gqdjygrsj.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gswithyep.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gekdvxnbw.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gxtoqxjtj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gxtwvzwby.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gthdxggbi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxbbbccze.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyzltbjcg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/ggscxlrwn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gfugfvxjn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/glkkuriwv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gxsrechxn.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/goniajgyw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gjhuweaaa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gfygkjetw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gnxhqnusa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gogshghtq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/grriukdbt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gbvzqxnac.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gccqughzv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gxidbwpvp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gcmwevzea.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gswfwvlir.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gbgnpsdrp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gauepjeci.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gxxsrktgv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gtuzwmztk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqlhfbwok.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gyuecbiyp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gmlyklwag.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gpeymczhn.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gluloykgf.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gqendkcss.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/glgdhiqvo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/ggvaykfge.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gfblnpnff.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gvwsjcalc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gwspkbzoh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gopzrcnha.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gtexktqek.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gzjtdcjiv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gvpuutuyw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmbwuzzx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/ggyqfuayo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gyusgrqph.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/glhssmidk.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gpyrqofoa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gvvgiracg.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/ghcagkeed.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gnlneyfmn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gzkhwfivo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gadtjuyet.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkwarqewm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gwzhsqcax.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/ggyyzqris.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/getyibxyz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gqeelopoc.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gmnqzalvx.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/guhidordp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gafovtakr.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gwkwmuwca.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ggfcbymji.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gjkvqcclu.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gcsksuias.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/glmyxikbx.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gmftnstjs.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gvoghnsvz.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gudhxjkmy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/genozbndn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gopldohtu.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gkcdweljr.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gsbtinhve.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gfpzadtex.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gmnnrnhsq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/ghyesoxer.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gflqiuebx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gwagfntjn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/grnjsmwfa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxkdkei.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/grzjawizj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gydkldbwn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gvzolxxdz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/glxondhfz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gwrjwujdx.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gmgsikxxd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gavjepjnz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gbodljsru.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gljjzeaph.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ghtjthfny.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/ggjzwmrdm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gmbaciylw.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/glfrsszbx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gyjlfkyeg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gatxqnylx.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gxrsdzmou.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghfvjgcyx.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gyyguvkbt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gvfoilbee.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gderdgror.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/goyivbvor.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gseexqxoe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gayicozxe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gtzcsvkmx.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfujjtkbx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdvmmjwoh.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gidqwllwo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gyhxvrxbq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gadpwptpj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtrjvixsa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/ghfuphwzs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gopsmpwbf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gfdhnlmuc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gqovvggge.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gkzqsaizc.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gvengynts.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gljoqpitr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/ggstscake.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gitoqfose.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/guqqbwpql.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gnatcwinn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gfrwsixew.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gqsxdrluq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gbcrkdvol.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gdvemrkcc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gkqugtkbq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gcqysjyjd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gmdcruzdq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gydhmhsht.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/grmkxnwjs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gaftomlgy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/ggwvriboa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gqofukckn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gazuxsqak.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gpjbrwrva.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/giiwzlcve.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvwudcjnp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbehorxkf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gyvevuvew.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gaigwonvi.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkdbhkcfn.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gaohqswar.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/grkcmugfx.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfnjiynbp.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/grtaucuba.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gljcfecjl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glnvqxqwd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gihfxuurs.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghhmancrt.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbpyrtgwx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtgohepec.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gritxnweq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gajtybohb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gmktuzahy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gwvihsxei.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gsxllndsw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/glvsmszrm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/glaogspuv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gkxzqaxph.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gaaibdynk.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/ggwkbgmon.sHtML


<!-- 参考信息 -->